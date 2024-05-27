# Comparing `tmp/aa_forum-2.2.1.tar.gz` & `tmp/aa_forum-2.3.0.tar.gz`

## Comparing `aa_forum-2.2.1.tar` & `aa_forum-2.3.0.tar`

### file list

```diff
@@ -1,221 +1,221 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/__init__.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/admin.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/app_settings.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/apps.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/auth_hooks.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/constants.py
--rw-r--r--   0        0        0    19631 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/forms.py
--rw-r--r--   0        0        0     8652 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/managers.py
--rw-r--r--   0        0        0    30251 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/models.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/signals.py
--rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/urls.py
--rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/helper/discord_messages.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/helper/eve_images.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/helper/forms.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/helper/pagination.py
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/helper/text.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/helper/user.py
--rw-r--r--   0        0        0    39481 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/django.pot
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39697 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    28897 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    52203 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    44964 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    40657 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39666 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39532 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3826 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    41206 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39560 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/pl_PL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39856 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/pl_PL/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    33968 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    58064 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39693 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/sk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    40504 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39847 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0001_initial.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0002_default_settings.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0003_board_discord_webhook.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0004_board_use_webhook_for_replies.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0005_announcement_boards.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0006_reset_default_settings.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0007_change_settings_to_singleton.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0008_populate_default_settings.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0009_add_related_names.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0010_better_setting_names.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0011_userprofile.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0012_personal_messages.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0013_personal_messages_migrate_zero_fix.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0014_userprofile_discord_dm_on_new_personal_message.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0015_alter_board_use_webhook_for_replies.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0016_fix_quotation_marks.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0017_ckeditor5_and_dashboard_widgets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/scripts/__init__.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/scripts/drop_tables.sql
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/scripts/fake_messages.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/LICENSE
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-cs.json
--rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-de.json
--rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-en.json
--rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-es.json
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-fr.json
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-it.json
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-ja.json
--rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-ko.json
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-nl.json
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-pl.json
--rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-ru.json
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-sk.json
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-uk.json
--rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-zh.json
--rw-r--r--   0        0        0    13668 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/css/aa-forum.css
--rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/css/aa-forum.min.css
--rw-r--r--   0        0        0    16294 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/css/aa-forum.min.css.map
--rw-r--r--   0        0        0     7385 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.js
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js.map
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.js
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.min.js
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.min.js.map
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.js
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js.map
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.js
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js.map
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.js
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js.map
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.js
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js.map
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/LICENSE.md
--rw-r--r--   0        0        0    18931 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.css
--rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.min.css
--rw-r--r--   0        0        0   167106 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.js
--rw-r--r--   0        0        0    76775 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.min.js
--rw-r--r--   0        0        0   156955 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.js
--rw-r--r--   0        0        0    73170 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.min.js
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/LICENSE
--rw-r--r--   0        0        0    34395 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.css
--rw-r--r--   0        0        0    29738 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css
--rw-r--r--   0        0        0    38867 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css.map
--rw-r--r--   0        0        0    34280 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.js
--rw-r--r--   0        0        0    22226 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.min.js
--rw-r--r--   0        0        0     9711 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.css
--rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.min.css
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/base.html
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/aa-forum-admin-js.html
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/aa-forum-bootstrap-js.html
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/aa-forum-ckeditor-js.html
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/aa-forum-css.html
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/aa-forum-dashboard-widgets-js.html
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/aa-forum-oembed-js.html
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/aa-forum-personal-messages-js.html
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/ckeditor5-css.html
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/ckeditor5-js.html
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/select2-css.html
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/select2-js.html
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/sumoselect-css.html
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/sumoselect-js.html
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/svg/aa-forum-icons.svg
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/administration/delete-board.html
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/administration/delete-category.html
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/breadcrumb.html
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/menu.html
--rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/board-loop.html
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/categories.html
--rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/category-loop.html
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/new-category.html
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/settings-form.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/form/required-field-hint.html
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/forum-index.html
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/board-index.html
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/board.html
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/no-access.html
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/pagination.html
--rw-r--r--   0        0        0     5965 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/topic.html
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/message.html
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html
--rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/reply.html
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/menu/menu-admin.html
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/menu/menu-user.html
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html
--rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/profile/form.html
--rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/search/pagination.html
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/search/search-form.html
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/search/search-result.html
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/widgets/unread-topics.html
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/administration/categories-and-boards.html
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/administration/forum-settings.html
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/board.html
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/index.html
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/modify-message.html
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/modify-topic.html
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/new-topic.html
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/topic.html
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/unread-topics.html
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/personal-messages/inbox.html
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/personal-messages/new-message.html
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/personal-messages/reply-message.html
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/profile/index.html
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/search/results.html
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/widgets/dashboard-widgets.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templatetags/__init__.py
--rw-r--r--   0        0        0     9950 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templatetags/aa_forum.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/__init__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_app_settings.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_auth_hooks.py
--rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_helpers.py
--rw-r--r--   0        0        0    74867 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_integration.py
--rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_managers.py
--rw-r--r--   0        0        0    36507 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_models.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_signals.py
--rw-r--r--   0        0        0    29431 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_templatetags.py
--rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_views_admin.py
--rw-r--r--   0        0        0    51417 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_views_forum.py
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/utils.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/views/__init__.py
--rw-r--r--   0        0        0    18371 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/views/admin.py
--rw-r--r--   0        0        0    44779 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/views/forum.py
--rw-r--r--   0        0        0    13162 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/views/personal_messages.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/views/profile.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/views/search.py
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/views/widgets.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_forum-2.2.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_forum-2.2.1/LICENSE
--rw-r--r--   0        0        0    20310 2020-02-02 00:00:00.000000 aa_forum-2.2.1/README.md
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 aa_forum-2.2.1/pyproject.toml
--rw-r--r--   0        0        0    63005 2020-02-02 00:00:00.000000 aa_forum-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/__init__.py
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/admin.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/app_settings.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/apps.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/auth_hooks.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/constants.py
+-rw-r--r--   0        0        0    19631 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/forms.py
+-rw-r--r--   0        0        0     8652 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/managers.py
+-rw-r--r--   0        0        0    30251 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/models.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/signals.py
+-rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/urls.py
+-rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/helper/discord_messages.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/helper/eve_images.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/helper/forms.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/helper/pagination.py
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/helper/text.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/helper/user.py
+-rw-r--r--   0        0        0    39594 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/django.pot
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39810 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    28897 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    52379 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    45077 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40770 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39779 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39645 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3826 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    41325 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39673 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39969 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    33968 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    58270 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39806 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40617 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39960 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/0002_default_settings.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/0003_board_discord_webhook.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/0004_board_use_webhook_for_replies.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/0005_announcement_boards.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/0006_reset_default_settings.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/0007_change_settings_to_singleton.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/0008_populate_default_settings.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/0009_add_related_names.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/0010_better_setting_names.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/0011_userprofile.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/0012_personal_messages.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/0013_personal_messages_migrate_zero_fix.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/0014_userprofile_discord_dm_on_new_personal_message.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/0015_alter_board_use_webhook_for_replies.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/0016_fix_quotation_marks.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/0017_ckeditor5_and_dashboard_widgets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/migrations/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/scripts/__init__.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/scripts/drop_tables.sql
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/scripts/fake_messages.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/search/stopwords/LICENSE
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-cs.json
+-rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-de.json
+-rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-en.json
+-rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-es.json
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-fr.json
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-it.json
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-ja.json
+-rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-ko.json
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-nl.json
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-pl.json
+-rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-ru.json
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-sk.json
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-uk.json
+-rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-zh.json
+-rw-r--r--   0        0        0    13918 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/css/aa-forum.css
+-rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/css/aa-forum.min.css
+-rw-r--r--   0        0        0    16567 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/css/aa-forum.min.css.map
+-rw-r--r--   0        0        0     7385 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.js
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js.map
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.js
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.min.js
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.min.js.map
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.js
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js.map
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.js
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js.map
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.js
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js.map
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.js
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js.map
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/LICENSE.md
+-rw-r--r--   0        0        0    18931 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.css
+-rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.min.css
+-rw-r--r--   0        0        0   167106 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.js
+-rw-r--r--   0        0        0    76775 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.min.js
+-rw-r--r--   0        0        0   156955 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.js
+-rw-r--r--   0        0        0    73170 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.min.js
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/LICENSE
+-rw-r--r--   0        0        0    34395 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.css
+-rw-r--r--   0        0        0    29738 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css
+-rw-r--r--   0        0        0    38867 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css.map
+-rw-r--r--   0        0        0    34280 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.js
+-rw-r--r--   0        0        0    22226 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.min.js
+-rw-r--r--   0        0        0     9711 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.css
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.min.css
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/base.html
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/bundles/aa-forum-admin-js.html
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/bundles/aa-forum-bootstrap-js.html
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/bundles/aa-forum-ckeditor-js.html
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/bundles/aa-forum-css.html
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/bundles/aa-forum-dashboard-widgets-js.html
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/bundles/aa-forum-oembed-js.html
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/bundles/aa-forum-personal-messages-js.html
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/bundles/ckeditor5-css.html
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/bundles/ckeditor5-js.html
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/bundles/select2-css.html
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/bundles/select2-js.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/bundles/sumoselect-css.html
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/bundles/sumoselect-js.html
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/bundles/svg/aa-forum-icons.svg
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/modals/administration/delete-board.html
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/modals/administration/delete-category.html
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/breadcrumb.html
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/menu.html
+-rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/administration/board-loop.html
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/administration/categories.html
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/administration/category-loop.html
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/administration/new-category.html
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/administration/settings-form.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/form/required-field-hint.html
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/forum-index.html
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/board/board-index.html
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/board/board.html
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/board/no-access.html
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/board/pagination.html
+-rw-r--r--   0        0        0     6093 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/board/topic.html
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/topic/message.html
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html
+-rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/topic/reply.html
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/menu/menu-admin.html
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/menu/menu-user.html
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html
+-rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html
+-rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/profile/form.html
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/search/pagination.html
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/search/search-form.html
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/search/search-result.html
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/widgets/unread-topics.html
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/view/administration/categories-and-boards.html
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/view/administration/forum-settings.html
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/view/forum/board.html
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/view/forum/index.html
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/view/forum/modify-message.html
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/view/forum/modify-topic.html
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/view/forum/new-topic.html
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/view/forum/topic.html
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/view/forum/unread-topics.html
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/view/personal-messages/inbox.html
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/view/personal-messages/new-message.html
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/view/personal-messages/reply-message.html
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/view/profile/index.html
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/view/search/results.html
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templates/aa_forum/view/widgets/dashboard-widgets.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templatetags/__init__.py
+-rw-r--r--   0        0        0     9950 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/templatetags/aa_forum.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/tests/__init__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/tests/test_app_settings.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/tests/test_helpers.py
+-rw-r--r--   0        0        0    74867 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/tests/test_integration.py
+-rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/tests/test_managers.py
+-rw-r--r--   0        0        0    36507 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/tests/test_models.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/tests/test_signals.py
+-rw-r--r--   0        0        0    29431 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/tests/test_templatetags.py
+-rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/tests/test_views_admin.py
+-rw-r--r--   0        0        0    51417 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/tests/test_views_forum.py
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/tests/utils.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/views/__init__.py
+-rw-r--r--   0        0        0    18371 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/views/admin.py
+-rw-r--r--   0        0        0    44779 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/views/forum.py
+-rw-r--r--   0        0        0    13162 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/views/personal_messages.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/views/profile.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/views/search.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 aa_forum-2.3.0/aa_forum/views/widgets.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_forum-2.3.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_forum-2.3.0/LICENSE
+-rw-r--r--   0        0        0    20306 2020-02-02 00:00:00.000000 aa_forum-2.3.0/README.md
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 aa_forum-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0    63003 2020-02-02 00:00:00.000000 aa_forum-2.3.0/PKG-INFO
```

### Comparing `aa_forum-2.2.1/aa_forum/admin.py` & `aa_forum-2.3.0/aa_forum/admin.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/app_settings.py` & `aa_forum-2.3.0/aa_forum/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/apps.py` & `aa_forum-2.3.0/aa_forum/apps.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/auth_hooks.py` & `aa_forum-2.3.0/aa_forum/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/constants.py` & `aa_forum-2.3.0/aa_forum/constants.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/forms.py` & `aa_forum-2.3.0/aa_forum/forms.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/managers.py` & `aa_forum-2.3.0/aa_forum/managers.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/models.py` & `aa_forum-2.3.0/aa_forum/models.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/signals.py` & `aa_forum-2.3.0/aa_forum/signals.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/urls.py` & `aa_forum-2.3.0/aa_forum/urls.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/helper/discord_messages.py` & `aa_forum-2.3.0/aa_forum/helper/discord_messages.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/helper/eve_images.py` & `aa_forum-2.3.0/aa_forum/helper/eve_images.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/helper/forms.py` & `aa_forum-2.3.0/aa_forum/helper/forms.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/helper/pagination.py` & `aa_forum-2.3.0/aa_forum/helper/pagination.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/helper/text.py` & `aa_forum-2.3.0/aa_forum/helper/text.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/helper/user.py` & `aa_forum-2.3.0/aa_forum/helper/user.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/locale/django.pot` & `aa_forum-2.3.0/aa_forum/locale/django.pot`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -313,96 +313,96 @@
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:625
+#: aa_forum/models.py:623
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:626
+#: aa_forum/models.py:624
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:805
+#: aa_forum/models.py:803
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:806
+#: aa_forum/models.py:804
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:946
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:947
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:1003
+#: aa_forum/models.py:1001
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:1004
+#: aa_forum/models.py:1002
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:1005
+#: aa_forum/models.py:1003
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:1010
+#: aa_forum/models.py:1008
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:1015
+#: aa_forum/models.py:1013
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:1020
+#: aa_forum/models.py:1018
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:1031
+#: aa_forum/models.py:1029
 msgid "setting"
 msgstr ""
 
-#: aa_forum/models.py:1032
+#: aa_forum/models.py:1030
 msgid "settings"
 msgstr ""
 
-#: aa_forum/models.py:1042
+#: aa_forum/models.py:1040
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
 #: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr ""
 
-#: aa_forum/models.py:1069
+#: aa_forum/models.py:1067
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:1070
+#: aa_forum/models.py:1068
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:1080
+#: aa_forum/models.py:1078
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
 #: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
@@ -482,21 +482,21 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:91
 msgid "Unlock/re-open topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:101
 msgid "Lock/close topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
@@ -532,15 +532,15 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:122
 msgid "Delete topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
@@ -696,15 +696,15 @@
 msgstr[1] ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
 msgid "New"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
@@ -803,40 +803,44 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:28
+msgid "Go to first unread message"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
 msgid "Last post"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:73
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:112
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
@@ -953,15 +957,15 @@
 msgid "User profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:5
 msgid "Forum: Unread topics"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
```

### Comparing `aa_forum-2.2.1/aa_forum/locale/cs/LC_MESSAGES/django.mo` & `aa_forum-2.3.0/aa_forum/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/locale/cs/LC_MESSAGES/django.po` & `aa_forum-2.3.0/aa_forum/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:06+0000\n"
-"Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Czech <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/cs/>\n"
-"Language: cs\n"
+"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-forum/it/>\n"
+"Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
-"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
@@ -43,15 +41,15 @@
 #: aa_forum/apps.py:20
 #, python-brace-format
 msgid "AA Forum v{__version__}"
 msgstr ""
 
 #: aa_forum/forms.py:42
 msgid "This field is mandatory"
-msgstr ""
+msgstr "Questo campo è obbligatorio"
 
 #: aa_forum/forms.py:116 aa_forum/forms.py:118 aa_forum/forms.py:169
 #: aa_forum/forms.py:171 aa_forum/forms.py:616
 #: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:25
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:25
 msgid "Subject"
 msgstr ""
@@ -315,96 +313,96 @@
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:625
+#: aa_forum/models.py:623
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:626
+#: aa_forum/models.py:624
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:805
+#: aa_forum/models.py:803
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:806
+#: aa_forum/models.py:804
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:946
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:947
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:1003
+#: aa_forum/models.py:1001
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:1004
+#: aa_forum/models.py:1002
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:1005
+#: aa_forum/models.py:1003
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:1010
+#: aa_forum/models.py:1008
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:1015
+#: aa_forum/models.py:1013
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:1020
+#: aa_forum/models.py:1018
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:1031
+#: aa_forum/models.py:1029
 msgid "setting"
 msgstr ""
 
-#: aa_forum/models.py:1032
+#: aa_forum/models.py:1030
 msgid "settings"
 msgstr ""
 
-#: aa_forum/models.py:1042
+#: aa_forum/models.py:1040
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
 #: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr ""
 
-#: aa_forum/models.py:1069
+#: aa_forum/models.py:1067
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:1070
+#: aa_forum/models.py:1068
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:1080
+#: aa_forum/models.py:1078
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
 #: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
@@ -484,21 +482,21 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:91
 msgid "Unlock/re-open topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:101
 msgid "Lock/close topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
@@ -534,15 +532,15 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:122
 msgid "Delete topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
@@ -681,34 +679,32 @@
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:6
 msgid "Fields marked with an asterisk (*) are mandatory"
-msgstr ""
+msgstr "I campi contrassegnati da un asterisco (*) sono obbligatori"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board-index.html:27
 msgid "No topics have been started in this board …"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
 msgstr[1] ""
-msgstr[2] ""
-msgstr[3] ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
 msgid "New"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
@@ -807,40 +803,44 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:28
+msgid "Go to first unread message"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
 msgid "Last post"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:73
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:112
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
@@ -957,15 +957,15 @@
 msgid "User profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:5
 msgid "Forum: Unread topics"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
 
@@ -1031,16 +1031,14 @@
 
 #: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
 msgstr[1] ""
-msgstr[2] ""
-msgstr[3] ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
 #: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
```

### Comparing `aa_forum-2.2.1/aa_forum/locale/de/LC_MESSAGES/django.mo` & `aa_forum-2.3.0/aa_forum/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/locale/de/LC_MESSAGES/django.po` & `aa_forum-2.3.0/aa_forum/locale/de/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 # Translators:
 # Peter Pfeufer, 2022
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:06+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: German <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/de/>\n"
+"Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-forum/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.5.3\n"
 
@@ -377,96 +377,96 @@
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 "<h4>Warnung!</h4><p>Es gibt bereits ein Thema mit genau demselben Namen in "
 "diesem Board.</p><p>Siehe hier: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 
-#: aa_forum/models.py:625
+#: aa_forum/models.py:623
 msgid "topic"
 msgstr "Thema"
 
-#: aa_forum/models.py:626
+#: aa_forum/models.py:624
 msgid "topics"
 msgstr "Themen"
 
-#: aa_forum/models.py:805
+#: aa_forum/models.py:803
 msgid "message"
 msgstr "Beitrag"
 
-#: aa_forum/models.py:806
+#: aa_forum/models.py:804
 msgid "messages"
 msgstr "Beträge"
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:946
 msgid "personal message"
 msgstr "Persönliche Nachricht"
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:947
 msgid "personal messages"
 msgstr "Persönliche Nachrichten"
 
-#: aa_forum/models.py:1003
+#: aa_forum/models.py:1001
 msgid "Messages per page"
 msgstr "Beiträge pro Seite"
 
-#: aa_forum/models.py:1004
+#: aa_forum/models.py:1002
 msgid "Topics per page"
 msgstr "Themen pro Seite"
 
-#: aa_forum/models.py:1005
+#: aa_forum/models.py:1003
 msgid "User signature length"
 msgstr "Länge der Benutzersignatur"
 
-#: aa_forum/models.py:1010
+#: aa_forum/models.py:1008
 msgid "Maximum number of messages per page in the topic view"
 msgstr "Maximale Anzahl von Beiträgen pro Seite in der Themenansicht"
 
-#: aa_forum/models.py:1015
+#: aa_forum/models.py:1013
 msgid "Maximum number of topics per page in the board view"
 msgstr "Maximale Anzahl von Themen pro Seite in der Board-Ansicht"
 
-#: aa_forum/models.py:1020
+#: aa_forum/models.py:1018
 msgid "Maximum length of a users signature"
 msgstr "Maximale Länge einer Benutzersignatur"
 
-#: aa_forum/models.py:1031
+#: aa_forum/models.py:1029
 msgid "setting"
 msgstr "Einstellung"
 
-#: aa_forum/models.py:1032
+#: aa_forum/models.py:1030
 msgid "settings"
 msgstr "Einstellungen"
 
-#: aa_forum/models.py:1042
+#: aa_forum/models.py:1040
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
 #: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr "Forumeinstellungen"
 
-#: aa_forum/models.py:1069
+#: aa_forum/models.py:1067
 msgid "user profile"
 msgstr "Benutzerprofil"
 
-#: aa_forum/models.py:1070
+#: aa_forum/models.py:1068
 msgid "user profiles"
 msgstr "Benutzerprofile"
 
-#: aa_forum/models.py:1080
+#: aa_forum/models.py:1078
 msgid "Forum user profile"
 msgstr "Benutzerprofil"
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
 #: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr "geschrieben:"
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr "Antwort"
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
@@ -548,21 +548,21 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr "Sperrstatus des Themas ändern"
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:91
 msgid "Unlock/re-open topic"
 msgstr "Thema entsperren/erneut öffnen"
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:101
 msgid "Lock/close topic"
 msgstr "Thema sperren/schließen"
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr "Möchtest Du dieses Thema wirklich entsperren/erneut öffnen?"
 
@@ -602,15 +602,15 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr "Sticky setzen"
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:122
 msgid "Delete topic"
 msgstr "Thema löschen"
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr "Möchtest Du dieses Thema wirklich löschen?"
 
@@ -783,15 +783,15 @@
 msgstr[1] "Dieses Board ist auf die folgenden Gruppen beschränkt:"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr "Untergeordnete Boards:"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
 msgid "New"
 msgstr "Neu"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr "Beiträge"
 
@@ -892,40 +892,46 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr "Letzter"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:28
+#, fuzzy
+#| msgid "Go to last message"
+msgid "Go to first unread message"
+msgstr "Gehe zum letzten Beitrag"
+
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
 msgid "Topic is always on top"
 msgstr "Das Thema steht immer oben"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
 msgid "Topic is locked"
 msgstr "Thema ist gesperrt"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
 msgid "Started by"
 msgstr "Begonnen bei"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
 msgid "Replies"
 msgstr "Antworten"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
 msgid "Last post"
 msgstr "Letzter Beitrag"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:73
 msgid "Go to last message"
 msgstr "Gehe zum letzten Beitrag"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:112
 msgid "Change topics sticky state"
 msgstr "Sticky-Status vom Thema ändern"
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr "Alle Themen als gelesen markieren"
@@ -1045,15 +1051,15 @@
 msgid "User profile"
 msgstr "Benutzerprofil"
 
 #: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr "Suche …"
 
-#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:5
 msgid "Forum: Unread topics"
 msgstr "Forum: Ungelesene Themen"
 
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr "Verwaltung (Kategorien und Boards)"
 
@@ -1169,31 +1175,31 @@
 msgid "<h4>Success!</h4><p>Settings updated.</p>"
 msgstr "<h4>Erfolg!</h4><p>Einstellungen aktualisiert.</p>"
 
 #: aa_forum/views/admin.py:597 aa_forum/views/personal_messages.py:122
 #: aa_forum/views/personal_messages.py:249 aa_forum/views/profile.py:70
 msgid "<h4>Error!</h4><p>Something went wrong, please check your input.</p>"
 msgstr ""
-"<h4>Fehler!</h4><p>Etwas ist schief gelaufen, bitte überprüfe Deine "
-"Eingabe.</p>"
+"<h4>Fehler!</h4><p>Etwas ist schief gelaufen, bitte überprüfe Deine Eingabe."
+"</p>"
 
 #: aa_forum/views/forum.py:232
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to visit does either not exist, "
 "or you don't have access to it.</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Das Board, das Du aufrufen willst, existiert entweder "
 "nicht oder Du hast keinen Zugriff darauf.</p>"
 
 #: aa_forum/views/forum.py:293
 msgid ""
 "<h4>Error!</h4><p>The category you were trying to post in does not exist.</p>"
 msgstr ""
-"<h4>Fehler!</h4><p>Die Kategorie, in der Du posten willst, existiert "
-"nicht.</p>"
+"<h4>Fehler!</h4><p>Die Kategorie, in der Du posten willst, existiert nicht.</"
+"p>"
 
 #: aa_forum/views/forum.py:320
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Das Board, in dem Du posten willst, existiert entweder "
```

### Comparing `aa_forum-2.2.1/aa_forum/locale/es/LC_MESSAGES/django.mo` & `aa_forum-2.3.0/aa_forum/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/locale/es/LC_MESSAGES/django.po` & `aa_forum-2.3.0/aa_forum/locale/es/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 # Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023, 2024.
 # Geovanny David Morales De la cruz <moralesgeovanny1996@gmail.com>, 2023, 2024.
 # Mak3rco <depormanuf1@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:06+0000\n"
 "Last-Translator: Mak3rco <depormanuf1@gmail.com>\n"
-"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/es/>\n"
+"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-forum/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.5.3\n"
 
@@ -399,98 +399,98 @@
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:625
+#: aa_forum/models.py:623
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:626
+#: aa_forum/models.py:624
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:805
+#: aa_forum/models.py:803
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:806
+#: aa_forum/models.py:804
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:946
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:947
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:1003
+#: aa_forum/models.py:1001
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:1004
+#: aa_forum/models.py:1002
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:1005
+#: aa_forum/models.py:1003
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:1010
+#: aa_forum/models.py:1008
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:1015
+#: aa_forum/models.py:1013
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:1020
+#: aa_forum/models.py:1018
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:1031
+#: aa_forum/models.py:1029
 msgid "setting"
 msgstr "ajuste"
 
-#: aa_forum/models.py:1032
+#: aa_forum/models.py:1030
 msgid "settings"
 msgstr "ajustes"
 
-#: aa_forum/models.py:1042
+#: aa_forum/models.py:1040
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
 #: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 #, fuzzy
 #| msgid "settings"
 msgid "Forum settings"
 msgstr "ajustes"
 
-#: aa_forum/models.py:1069
+#: aa_forum/models.py:1067
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:1070
+#: aa_forum/models.py:1068
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:1080
+#: aa_forum/models.py:1078
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
 #: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
@@ -574,21 +574,21 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:91
 msgid "Unlock/re-open topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:101
 msgid "Lock/close topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
@@ -624,15 +624,15 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:122
 #, fuzzy
 #| msgid "Delete"
 msgid "Delete topic"
 msgstr "Borrar"
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
@@ -794,15 +794,15 @@
 msgstr[1] ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
 msgid "New"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
@@ -901,40 +901,44 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:28
+msgid "Go to first unread message"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
 msgid "Last post"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:73
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:112
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
@@ -1059,15 +1063,15 @@
 msgid "User profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:5
 msgid "Forum: Unread topics"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
```

### Comparing `aa_forum-2.2.1/aa_forum/locale/fr_FR/LC_MESSAGES/django.mo` & `aa_forum-2.3.0/aa_forum/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/locale/fr_FR/LC_MESSAGES/django.po` & `aa_forum-2.3.0/aa_forum/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 # Matthias P <randomusernetcom@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:06+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/fr/>\n"
+"Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-forum/fr/>\n"
 "Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
 "X-Generator: Weblate 5.5.3\n"
 
@@ -324,96 +324,96 @@
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:625
+#: aa_forum/models.py:623
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:626
+#: aa_forum/models.py:624
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:805
+#: aa_forum/models.py:803
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:806
+#: aa_forum/models.py:804
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:946
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:947
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:1003
+#: aa_forum/models.py:1001
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:1004
+#: aa_forum/models.py:1002
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:1005
+#: aa_forum/models.py:1003
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:1010
+#: aa_forum/models.py:1008
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:1015
+#: aa_forum/models.py:1013
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:1020
+#: aa_forum/models.py:1018
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:1031
+#: aa_forum/models.py:1029
 msgid "setting"
 msgstr ""
 
-#: aa_forum/models.py:1032
+#: aa_forum/models.py:1030
 msgid "settings"
 msgstr ""
 
-#: aa_forum/models.py:1042
+#: aa_forum/models.py:1040
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
 #: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr ""
 
-#: aa_forum/models.py:1069
+#: aa_forum/models.py:1067
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:1070
+#: aa_forum/models.py:1068
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:1080
+#: aa_forum/models.py:1078
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
 #: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
@@ -493,21 +493,21 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:91
 msgid "Unlock/re-open topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:101
 msgid "Lock/close topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
@@ -543,15 +543,15 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:122
 msgid "Delete topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
@@ -709,15 +709,15 @@
 msgstr[1] ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
 msgid "New"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
@@ -816,40 +816,44 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:28
+msgid "Go to first unread message"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
 msgid "Last post"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:73
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:112
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
@@ -966,15 +970,15 @@
 msgid "User profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:5
 msgid "Forum: Unread topics"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
```

### Comparing `aa_forum-2.2.1/aa_forum/locale/it_IT/LC_MESSAGES/django.mo` & `aa_forum-2.3.0/aa_forum/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/locale/it_IT/LC_MESSAGES/django.po` & `aa_forum-2.3.0/aa_forum/locale/ja/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:06+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/it/>\n"
-"Language: it_IT\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-forum/ja/>\n"
+"Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
@@ -41,15 +42,15 @@
 #: aa_forum/apps.py:20
 #, python-brace-format
 msgid "AA Forum v{__version__}"
 msgstr ""
 
 #: aa_forum/forms.py:42
 msgid "This field is mandatory"
-msgstr "Questo campo è obbligatorio"
+msgstr ""
 
 #: aa_forum/forms.py:116 aa_forum/forms.py:118 aa_forum/forms.py:169
 #: aa_forum/forms.py:171 aa_forum/forms.py:616
 #: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:25
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:25
 msgid "Subject"
 msgstr ""
@@ -313,96 +314,96 @@
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:625
+#: aa_forum/models.py:623
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:626
+#: aa_forum/models.py:624
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:805
+#: aa_forum/models.py:803
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:806
+#: aa_forum/models.py:804
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:946
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:947
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:1003
+#: aa_forum/models.py:1001
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:1004
+#: aa_forum/models.py:1002
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:1005
+#: aa_forum/models.py:1003
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:1010
+#: aa_forum/models.py:1008
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:1015
+#: aa_forum/models.py:1013
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:1020
+#: aa_forum/models.py:1018
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:1031
+#: aa_forum/models.py:1029
 msgid "setting"
 msgstr ""
 
-#: aa_forum/models.py:1032
+#: aa_forum/models.py:1030
 msgid "settings"
 msgstr ""
 
-#: aa_forum/models.py:1042
+#: aa_forum/models.py:1040
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
 #: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr ""
 
-#: aa_forum/models.py:1069
+#: aa_forum/models.py:1067
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:1070
+#: aa_forum/models.py:1068
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:1080
+#: aa_forum/models.py:1078
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
 #: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
@@ -482,21 +483,21 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:91
 msgid "Unlock/re-open topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:101
 msgid "Lock/close topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
@@ -532,15 +533,15 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:122
 msgid "Delete topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
@@ -679,32 +680,31 @@
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:6
 msgid "Fields marked with an asterisk (*) are mandatory"
-msgstr "I campi contrassegnati da un asterisco (*) sono obbligatori"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board-index.html:27
 msgid "No topics have been started in this board …"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
-msgstr[1] ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
 msgid "New"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
@@ -803,40 +803,44 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:28
+msgid "Go to first unread message"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
 msgid "Last post"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:73
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:112
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
@@ -953,15 +957,15 @@
 msgid "User profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:5
 msgid "Forum: Unread topics"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
 
@@ -1026,15 +1030,14 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
-msgstr[1] ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
 #: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
```

### Comparing `aa_forum-2.2.1/aa_forum/locale/ja/LC_MESSAGES/django.po` & `aa_forum-2.3.0/aa_forum/locale/nl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:06+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/ja/>\n"
-"Language: ja\n"
+"Language-Team: Dutch <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-forum/nl/>\n"
+"Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
@@ -314,96 +314,96 @@
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:625
+#: aa_forum/models.py:623
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:626
+#: aa_forum/models.py:624
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:805
+#: aa_forum/models.py:803
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:806
+#: aa_forum/models.py:804
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:946
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:947
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:1003
+#: aa_forum/models.py:1001
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:1004
+#: aa_forum/models.py:1002
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:1005
+#: aa_forum/models.py:1003
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:1010
+#: aa_forum/models.py:1008
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:1015
+#: aa_forum/models.py:1013
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:1020
+#: aa_forum/models.py:1018
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:1031
+#: aa_forum/models.py:1029
 msgid "setting"
 msgstr ""
 
-#: aa_forum/models.py:1032
+#: aa_forum/models.py:1030
 msgid "settings"
 msgstr ""
 
-#: aa_forum/models.py:1042
+#: aa_forum/models.py:1040
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
 #: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr ""
 
-#: aa_forum/models.py:1069
+#: aa_forum/models.py:1067
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:1070
+#: aa_forum/models.py:1068
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:1080
+#: aa_forum/models.py:1078
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
 #: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
@@ -483,21 +483,21 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:91
 msgid "Unlock/re-open topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:101
 msgid "Lock/close topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
@@ -533,15 +533,15 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:122
 msgid "Delete topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
@@ -690,21 +690,22 @@
 msgid "No topics have been started in this board …"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
+msgstr[1] ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
 msgid "New"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
@@ -803,40 +804,44 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:28
+msgid "Go to first unread message"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
 msgid "Last post"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:73
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:112
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
@@ -953,15 +958,15 @@
 msgid "User profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:5
 msgid "Forum: Unread topics"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
 
@@ -1026,14 +1031,15 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
+msgstr[1] ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
 #: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
```

### Comparing `aa_forum-2.2.1/aa_forum/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_forum-2.3.0/aa_forum/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/locale/ko_KR/LC_MESSAGES/django.po` & `aa_forum-2.3.0/aa_forum/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 # Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
 # Mind of the Raven <okanieva@gmail.com>, 2024.
 # Rodpold Shard <rodpold@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:06+0000\n"
 "Last-Translator: Rodpold Shard <rodpold@gmail.com>\n"
-"Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/ko/>\n"
+"Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-forum/ko/>\n"
 "Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: Weblate 5.5.3\n"
 
@@ -75,16 +75,16 @@
 msgstr "게시판"
 
 #: aa_forum/forms.py:198
 msgid ""
 "Boards to be created with this category (One board per line). These boards "
 "will have no group restrictions, so you have to add them later where needed."
 msgstr ""
-"이 카테고리로(한 줄당 한 게시판) 게시판이 생성됩니다. 이 게시판은 그룹 "
-"제한이 없기 때문에 필요하면 나중에 추가할 수 있습니다."
+"이 카테고리로(한 줄당 한 게시판) 게시판이 생성됩니다. 이 게시판은 그룹 제한"
+"이 없기 때문에 필요하면 나중에 추가할 수 있습니다."
 
 #: aa_forum/forms.py:251
 msgid "Board name"
 msgstr "게시판 이름"
 
 #: aa_forum/forms.py:255
 msgid "Description"
@@ -100,16 +100,16 @@
 
 #: aa_forum/forms.py:269
 msgid ""
 "This will restrict access to this board to the selected groups. If no groups "
 "are selected, everyone who can access the forum can also access this board. "
 "(This setting is optional)"
 msgstr ""
-"이렇게 진행할 경우 게시판 접근 권한이 선택한 그룹으로 제한됩니다. 선택하지 "
-"않을 경우 모든 사람이 이 게시판에 접근할 수 있습니다. (선택사항)"
+"이렇게 진행할 경우 게시판 접근 권한이 선택한 그룹으로 제한됩니다. 선택하지 않"
+"을 경우 모든 사람이 이 게시판에 접근할 수 있습니다. (선택사항)"
 
 #: aa_forum/forms.py:277
 msgid "Discord webhook (optional)"
 msgstr ""
 
 #: aa_forum/forms.py:279
 msgid ""
@@ -122,15 +122,16 @@
 msgstr ""
 
 #: aa_forum/forms.py:294
 msgid ""
 "When activated every reply to any topic in this board will be posted to the "
 "defined Discord channel. (Child boards are excluded) Chose wisely! (Default: "
 "NO)"
-msgstr "활성화할 경우 이 게시판 내 모든 게시글의 모든 답변이 정의된 디스코드 채널에 "
+msgstr ""
+"활성화할 경우 이 게시판 내 모든 게시글의 모든 답변이 정의된 디스코드 채널에 "
 "게시됩니다. (기본값:꺼짐)"
 
 #: aa_forum/forms.py:302
 msgid "Mark board as \"Announcement Board\""
 msgstr "선택된 게시글을 공지사항으로 등록"
 
 #: aa_forum/forms.py:304
@@ -325,98 +326,98 @@
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:625
+#: aa_forum/models.py:623
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:626
+#: aa_forum/models.py:624
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:805
+#: aa_forum/models.py:803
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:806
+#: aa_forum/models.py:804
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:946
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:947
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:1003
+#: aa_forum/models.py:1001
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:1004
+#: aa_forum/models.py:1002
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:1005
+#: aa_forum/models.py:1003
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:1010
+#: aa_forum/models.py:1008
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:1015
+#: aa_forum/models.py:1013
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:1020
+#: aa_forum/models.py:1018
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:1031
+#: aa_forum/models.py:1029
 msgid "setting"
 msgstr "설정"
 
-#: aa_forum/models.py:1032
+#: aa_forum/models.py:1030
 msgid "settings"
 msgstr "설정"
 
-#: aa_forum/models.py:1042
+#: aa_forum/models.py:1040
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
 #: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 #, fuzzy
 #| msgid "settings"
 msgid "Forum settings"
 msgstr "설정"
 
-#: aa_forum/models.py:1069
+#: aa_forum/models.py:1067
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:1070
+#: aa_forum/models.py:1068
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:1080
+#: aa_forum/models.py:1078
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
 #: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
@@ -500,21 +501,21 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:91
 msgid "Unlock/re-open topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:101
 msgid "Lock/close topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
@@ -550,15 +551,15 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:122
 #, fuzzy
 #| msgid "Delete"
 msgid "Delete topic"
 msgstr "삭제"
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
@@ -715,15 +716,15 @@
 msgstr[0] ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
 msgid "New"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
@@ -822,40 +823,44 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr "마지막"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:28
+msgid "Go to first unread message"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
 msgid "Last post"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:73
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:112
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
@@ -869,16 +874,17 @@
 msgstr "편집일:"
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:14
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:15
 msgid ""
 "Note: You are not on the last page of this topic and may miss the most "
 "recent replies."
-msgstr "참고 : 현재 이 게시글의 마지막 페이지에 있지 않음으로 최신 답글을 놓칠 수 "
-"있습니다."
+msgstr ""
+"참고 : 현재 이 게시글의 마지막 페이지에 있지 않음으로 최신 답글을 놓칠 수 있"
+"습니다."
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:27
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:21
 msgid "Modify"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:7
@@ -977,15 +983,15 @@
 msgid "User profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr "검색 …"
 
-#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:5
 msgid "Forum: Unread topics"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
```

### Comparing `aa_forum-2.2.1/aa_forum/locale/nl/LC_MESSAGES/django.po` & `aa_forum-2.3.0/aa_forum/locale/sk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:06+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Dutch <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/nl/>\n"
-"Language: nl\n"
+"Language-Team: Slovak <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-forum/sk/>\n"
+"Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
@@ -314,96 +315,96 @@
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:625
+#: aa_forum/models.py:623
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:626
+#: aa_forum/models.py:624
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:805
+#: aa_forum/models.py:803
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:806
+#: aa_forum/models.py:804
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:946
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:947
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:1003
+#: aa_forum/models.py:1001
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:1004
+#: aa_forum/models.py:1002
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:1005
+#: aa_forum/models.py:1003
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:1010
+#: aa_forum/models.py:1008
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:1015
+#: aa_forum/models.py:1013
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:1020
+#: aa_forum/models.py:1018
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:1031
+#: aa_forum/models.py:1029
 msgid "setting"
 msgstr ""
 
-#: aa_forum/models.py:1032
+#: aa_forum/models.py:1030
 msgid "settings"
 msgstr ""
 
-#: aa_forum/models.py:1042
+#: aa_forum/models.py:1040
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
 #: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr ""
 
-#: aa_forum/models.py:1069
+#: aa_forum/models.py:1067
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:1070
+#: aa_forum/models.py:1068
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:1080
+#: aa_forum/models.py:1078
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
 #: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
@@ -483,21 +484,21 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:91
 msgid "Unlock/re-open topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:101
 msgid "Lock/close topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
@@ -533,15 +534,15 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:122
 msgid "Delete topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
@@ -691,21 +692,23 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
 msgid "New"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
@@ -804,40 +807,44 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:28
+msgid "Go to first unread message"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
 msgid "Last post"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:73
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:112
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
@@ -954,15 +961,15 @@
 msgid "User profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:5
 msgid "Forum: Unread topics"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
 
@@ -1028,14 +1035,16 @@
 
 #: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
 #: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
```

### Comparing `aa_forum-2.2.1/aa_forum/locale/pl_PL/LC_MESSAGES/django.mo` & `aa_forum-2.3.0/aa_forum/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/locale/pl_PL/LC_MESSAGES/django.po` & `aa_forum-2.3.0/aa_forum/locale/cs/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Peter Pfeufer <info@ppfeufer.de>, 2024.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:06+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Polish <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/pl/>\n"
-"Language: pl_PL\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Czech <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-forum/cs/>\n"
+"Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
-"|| n%100>=20) ? 1 : 2;\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
+"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
@@ -42,15 +43,15 @@
 #: aa_forum/apps.py:20
 #, python-brace-format
 msgid "AA Forum v{__version__}"
 msgstr ""
 
 #: aa_forum/forms.py:42
 msgid "This field is mandatory"
-msgstr "To pole jest wymagane"
+msgstr ""
 
 #: aa_forum/forms.py:116 aa_forum/forms.py:118 aa_forum/forms.py:169
 #: aa_forum/forms.py:171 aa_forum/forms.py:616
 #: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:25
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:25
 msgid "Subject"
 msgstr ""
@@ -314,96 +315,96 @@
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:625
+#: aa_forum/models.py:623
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:626
+#: aa_forum/models.py:624
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:805
+#: aa_forum/models.py:803
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:806
+#: aa_forum/models.py:804
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:946
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:947
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:1003
+#: aa_forum/models.py:1001
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:1004
+#: aa_forum/models.py:1002
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:1005
+#: aa_forum/models.py:1003
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:1010
+#: aa_forum/models.py:1008
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:1015
+#: aa_forum/models.py:1013
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:1020
+#: aa_forum/models.py:1018
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:1031
+#: aa_forum/models.py:1029
 msgid "setting"
 msgstr ""
 
-#: aa_forum/models.py:1032
+#: aa_forum/models.py:1030
 msgid "settings"
 msgstr ""
 
-#: aa_forum/models.py:1042
+#: aa_forum/models.py:1040
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
 #: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr ""
 
-#: aa_forum/models.py:1069
+#: aa_forum/models.py:1067
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:1070
+#: aa_forum/models.py:1068
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:1080
+#: aa_forum/models.py:1078
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
 #: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
@@ -461,15 +462,15 @@
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-board.html:32
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:32
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:32
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:31
 #: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:31
 msgid "Delete"
-msgstr "Usuń"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:3
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:8
 #: aa_forum/templates/aa_forum/partials/administration/category-loop.html:25
 msgid "Delete category"
 msgstr ""
 
@@ -483,21 +484,21 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:91
 msgid "Unlock/re-open topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:101
 msgid "Lock/close topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
@@ -533,15 +534,15 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:122
 msgid "Delete topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
@@ -673,42 +674,41 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
-"Chciałbyś pomóc w tłumaczeniu tej apki na Twój język bądź poprawić aktualne "
-"tłumaczenia?"
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "Dołącz do naszego zespołu tłumaczy!"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:6
 msgid "Fields marked with an asterisk (*) are mandatory"
-msgstr "Pola z gwiazdką (*) są wymagane"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board-index.html:27
 msgid "No topics have been started in this board …"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
+msgstr[3] ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
 msgid "New"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
@@ -807,40 +807,44 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:28
+msgid "Go to first unread message"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
 msgid "Last post"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:73
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:112
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
@@ -957,15 +961,15 @@
 msgid "User profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:5
 msgid "Forum: Unread topics"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
 
@@ -1032,14 +1036,15 @@
 #: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
+msgstr[3] ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
 #: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
```

### Comparing `aa_forum-2.2.1/aa_forum/locale/ru/LC_MESSAGES/django.mo` & `aa_forum-2.3.0/aa_forum/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/locale/ru/LC_MESSAGES/django.po` & `aa_forum-2.3.0/aa_forum/locale/ru/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 # Nikolay <nick.postnikov@gmail.com>, 2023, 2024.
 # Max <mark25@inbox.ru>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:06+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/ru/>\n"
+"Language-Team: Russian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-forum/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: Weblate 5.5.3\n"
@@ -355,100 +355,99 @@
 #: aa_forum/models.py:394
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
-"<h4>Предупреждение!</h4><p>На доске уже есть тема с таким же "
-"названием.</p><p>См.: <a href=\"{self.topic_url}\">{self._topic."
-"subject}</a></p>"
+"<h4>Предупреждение!</h4><p>На доске уже есть тема с таким же названием.</"
+"p><p>См.: <a href=\"{self.topic_url}\">{self._topic.subject}</a></p>"
 
-#: aa_forum/models.py:625
+#: aa_forum/models.py:623
 msgid "topic"
 msgstr "тема"
 
-#: aa_forum/models.py:626
+#: aa_forum/models.py:624
 msgid "topics"
 msgstr "темы"
 
-#: aa_forum/models.py:805
+#: aa_forum/models.py:803
 msgid "message"
 msgstr "сообщение"
 
-#: aa_forum/models.py:806
+#: aa_forum/models.py:804
 msgid "messages"
 msgstr "сообщения"
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:946
 msgid "personal message"
 msgstr "личное сообщение"
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:947
 msgid "personal messages"
 msgstr "личные сообщения"
 
-#: aa_forum/models.py:1003
+#: aa_forum/models.py:1001
 msgid "Messages per page"
 msgstr "Сообщений на странице"
 
-#: aa_forum/models.py:1004
+#: aa_forum/models.py:1002
 msgid "Topics per page"
 msgstr "Тем на странице"
 
-#: aa_forum/models.py:1005
+#: aa_forum/models.py:1003
 msgid "User signature length"
 msgstr "Длина подписи пользователя"
 
-#: aa_forum/models.py:1010
+#: aa_forum/models.py:1008
 msgid "Maximum number of messages per page in the topic view"
 msgstr "Максимальное количество сообщений на странице при просмотре темы"
 
-#: aa_forum/models.py:1015
+#: aa_forum/models.py:1013
 msgid "Maximum number of topics per page in the board view"
 msgstr "Максимальное количество тем на странице при просмотре доски"
 
-#: aa_forum/models.py:1020
+#: aa_forum/models.py:1018
 msgid "Maximum length of a users signature"
 msgstr "Максимальная длина подписи пользователя"
 
-#: aa_forum/models.py:1031
+#: aa_forum/models.py:1029
 msgid "setting"
 msgstr "настройка"
 
-#: aa_forum/models.py:1032
+#: aa_forum/models.py:1030
 msgid "settings"
 msgstr "настройки"
 
-#: aa_forum/models.py:1042
+#: aa_forum/models.py:1040
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
 #: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr "Настройки форума"
 
-#: aa_forum/models.py:1069
+#: aa_forum/models.py:1067
 msgid "user profile"
 msgstr "профиль пользователя"
 
-#: aa_forum/models.py:1070
+#: aa_forum/models.py:1068
 msgid "user profiles"
 msgstr "профили пользователей"
 
-#: aa_forum/models.py:1080
+#: aa_forum/models.py:1078
 msgid "Forum user profile"
 msgstr "профиль пользователя"
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
 #: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr "дата:"
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr "Ответить"
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
@@ -528,21 +527,21 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr "Изменить блокировку темы"
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:91
 msgid "Unlock/re-open topic"
 msgstr "Разблокировать/открыть тему"
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:101
 msgid "Lock/close topic"
 msgstr "Заблокировать/закрыть тему"
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr "Вы уверены что хотите разблокировать эту тему?"
 
@@ -580,15 +579,15 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr "Установить свойство «sticky»"
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:122
 msgid "Delete topic"
 msgstr "Удалить тему"
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr "Вы уверены, что хотите удалить эту тему?"
 
@@ -761,15 +760,15 @@
 msgstr[3] "К доске имеют доступ следующие группы:"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr "Дочерние доски:"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
 msgid "New"
 msgstr "Новый"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr "Сообщения"
 
@@ -868,40 +867,46 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr "Последний"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:28
+#, fuzzy
+#| msgid "Go to last message"
+msgid "Go to first unread message"
+msgstr "Перейти к последнему сообщению"
+
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
 msgid "Topic is always on top"
 msgstr "Тема всегда в начале"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
 msgid "Topic is locked"
 msgstr "Тема закрыта"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
 msgid "Started by"
 msgstr "Запущена"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
 msgid "Replies"
 msgstr "Ответы"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
 msgid "Last post"
 msgstr "Последнее сообщение"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:73
 msgid "Go to last message"
 msgstr "Перейти к последнему сообщению"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:112
 msgid "Change topics sticky state"
 msgstr "Изменить свойство Sticky для темы"
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr "Отметить все темы как прочитанные"
@@ -1020,15 +1025,15 @@
 msgid "User profile"
 msgstr "профиль пользователя"
 
 #: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr "Поиск…"
 
-#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:5
 #, fuzzy
 #| msgid "Unread topics"
 msgid "Forum: Unread topics"
 msgstr "Непрочитанные темы"
 
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
@@ -1161,16 +1166,16 @@
 "<h4>Ошибка!</h4><p>Доска, на которую вы пытаетесь попасть, не существует или "
 "Вам не доступна.</p>"
 
 #: aa_forum/views/forum.py:293
 msgid ""
 "<h4>Error!</h4><p>The category you were trying to post in does not exist.</p>"
 msgstr ""
-"<h4>Ошибка!</h4><p>Категория, в которую в попытались написать, не "
-"существует.</p>"
+"<h4>Ошибка!</h4><p>Категория, в которую в попытались написать, не существует."
+"</p>"
 
 #: aa_forum/views/forum.py:320
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 "<h4>Ошибка!</h4><p>Доска, на которую вы пытаетесь написать, не существует "
@@ -1303,16 +1308,16 @@
 "<h4>Успех!</h4><p>Сообщение удалено.</p><p>Это было стартовое сообщение "
 "темы, так что вся тема также удалена.</p>"
 
 #: aa_forum/views/personal_messages.py:110
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Message to {recipient_main_char} sent.</p>"
 msgstr ""
-"<h4>Успех!</h4><p>Сообщение пользователю {recipient_main_char} "
-"отправлено.</p>"
+"<h4>Успех!</h4><p>Сообщение пользователю {recipient_main_char} отправлено.</"
+"p>"
 
 #: aa_forum/views/personal_messages.py:202
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to reply to does either not "
 "exist or you are not the recipient.</p>"
 msgstr ""
 "<h4>Ошибка!</h4><p>Сообщение, на которое Вы пытаетесь ответить, не "
```

### Comparing `aa_forum-2.2.1/aa_forum/locale/sk/LC_MESSAGES/django.mo` & `aa_forum-2.3.0/aa_forum/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/locale/sk/LC_MESSAGES/django.po` & `aa_forum-2.3.0/aa_forum/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# Dehao Wu <wudehao2000@163.com>, 2024.
+# Peter Pfeufer <info@ppfeufer.de>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:06+0000\n"
-"Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Slovak <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/sk/>\n"
-"Language: sk\n"
+"Last-Translator: Dehao Wu <wudehao2000@163.com>\n"
+"Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-forum/zh_Hans/>\n"
+"Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
-">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
@@ -34,24 +33,24 @@
 #: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
 #: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
 #: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
 #: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
 #: aa_forum/templates/aa_forum/view/profile/index.html:8
 #: aa_forum/templates/aa_forum/view/search/results.html:7
 msgid "Forum"
-msgstr ""
+msgstr "论坛"
 
 #: aa_forum/apps.py:20
 #, python-brace-format
 msgid "AA Forum v{__version__}"
 msgstr ""
 
 #: aa_forum/forms.py:42
 msgid "This field is mandatory"
-msgstr ""
+msgstr "这个字段是必填的"
 
 #: aa_forum/forms.py:116 aa_forum/forms.py:118 aa_forum/forms.py:169
 #: aa_forum/forms.py:171 aa_forum/forms.py:616
 #: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:25
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:25
 msgid "Subject"
 msgstr ""
@@ -59,19 +58,19 @@
 #: aa_forum/forms.py:145 aa_forum/forms.py:422 aa_forum/forms.py:665
 #: aa_forum/forms.py:730
 msgid "You have forgotten the message!"
 msgstr ""
 
 #: aa_forum/forms.py:190 aa_forum/forms.py:228 aa_forum/forms.py:249
 msgid "Name"
-msgstr ""
+msgstr "名字"
 
 #: aa_forum/forms.py:192 aa_forum/forms.py:230
 msgid "Category name"
-msgstr ""
+msgstr "分类名称"
 
 #: aa_forum/forms.py:196 aa_forum/forms.py:207
 msgid "Boards"
 msgstr ""
 
 #: aa_forum/forms.py:198
 msgid ""
@@ -145,16 +144,18 @@
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so. This setting will not be inherited to child boards. (Hint: These "
 "restrictions only take effect when a board is marked as \"Announcement "
 "Board\", see checkbox above.)"
 msgstr ""
 
 #: aa_forum/forms.py:362
+#, fuzzy
+#| msgid "Close"
 msgid "Close topic"
-msgstr ""
+msgstr "关闭"
 
 #: aa_forum/forms.py:364
 msgid "If checked, this topic will be closed after posting this message."
 msgstr ""
 
 #: aa_forum/forms.py:370
 msgid "Reopen topic"
@@ -315,96 +316,96 @@
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:625
+#: aa_forum/models.py:623
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:626
+#: aa_forum/models.py:624
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:805
+#: aa_forum/models.py:803
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:806
+#: aa_forum/models.py:804
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:946
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:947
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:1003
+#: aa_forum/models.py:1001
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:1004
+#: aa_forum/models.py:1002
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:1005
+#: aa_forum/models.py:1003
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:1010
+#: aa_forum/models.py:1008
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:1015
+#: aa_forum/models.py:1013
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:1020
+#: aa_forum/models.py:1018
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:1031
+#: aa_forum/models.py:1029
 msgid "setting"
 msgstr ""
 
-#: aa_forum/models.py:1032
+#: aa_forum/models.py:1030
 msgid "settings"
 msgstr ""
 
-#: aa_forum/models.py:1042
+#: aa_forum/models.py:1040
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
 #: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr ""
 
-#: aa_forum/models.py:1069
+#: aa_forum/models.py:1067
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:1070
+#: aa_forum/models.py:1068
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:1080
+#: aa_forum/models.py:1078
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
 #: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
@@ -427,15 +428,15 @@
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:17
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:17
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:11
 #: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:11
 msgid "Close"
-msgstr ""
+msgstr "关闭"
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-board.html:16
 msgid "Are you sure you want to delete this board?"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-board.html:17
 msgid "This will also remove all topics and messages in this board."
@@ -454,23 +455,23 @@
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:31
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:31
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:27
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:26
 #: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:26
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:35
 msgid "Cancel"
-msgstr ""
+msgstr "取消"
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-board.html:32
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:32
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:32
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:31
 #: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:31
 msgid "Delete"
-msgstr ""
+msgstr "删除"
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:3
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:8
 #: aa_forum/templates/aa_forum/partials/administration/category-loop.html:25
 msgid "Delete category"
 msgstr ""
 
@@ -484,21 +485,21 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:91
 msgid "Unlock/re-open topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:101
 msgid "Lock/close topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
@@ -534,15 +535,15 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:122
 msgid "Delete topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
@@ -673,42 +674,39 @@
 msgid "Search for:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
-msgstr ""
+msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr ""
+msgstr "加入我们的翻译团队吧！"
 
 #: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:6
 msgid "Fields marked with an asterisk (*) are mandatory"
-msgstr ""
+msgstr "带有(*)星号符号的字段是必填的"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board-index.html:27
 msgid "No topics have been started in this board …"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
-msgstr[3] ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
 msgid "New"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
@@ -807,40 +805,44 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:28
+msgid "Go to first unread message"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
 msgid "Last post"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:73
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:112
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
@@ -957,15 +959,15 @@
 msgid "User profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:5
 msgid "Forum: Unread topics"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
 
@@ -1030,17 +1032,14 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
-msgstr[3] ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
 #: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
```

### Comparing `aa_forum-2.2.1/aa_forum/locale/uk/LC_MESSAGES/django.mo` & `aa_forum-2.3.0/aa_forum/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/locale/uk/LC_MESSAGES/django.po` & `aa_forum-2.3.0/aa_forum/locale/uk/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 # "Andrii M." <elfleg0las88@gmail.com>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:06+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/uk/>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-forum/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: Weblate 5.5.3\n"
@@ -323,96 +323,96 @@
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:625
+#: aa_forum/models.py:623
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:626
+#: aa_forum/models.py:624
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:805
+#: aa_forum/models.py:803
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:806
+#: aa_forum/models.py:804
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:946
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:947
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:1003
+#: aa_forum/models.py:1001
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:1004
+#: aa_forum/models.py:1002
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:1005
+#: aa_forum/models.py:1003
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:1010
+#: aa_forum/models.py:1008
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:1015
+#: aa_forum/models.py:1013
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:1020
+#: aa_forum/models.py:1018
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:1031
+#: aa_forum/models.py:1029
 msgid "setting"
 msgstr ""
 
-#: aa_forum/models.py:1032
+#: aa_forum/models.py:1030
 msgid "settings"
 msgstr ""
 
-#: aa_forum/models.py:1042
+#: aa_forum/models.py:1040
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
 #: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr ""
 
-#: aa_forum/models.py:1069
+#: aa_forum/models.py:1067
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:1070
+#: aa_forum/models.py:1068
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:1080
+#: aa_forum/models.py:1078
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
 #: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
@@ -496,21 +496,21 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:91
 msgid "Unlock/re-open topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:101
 msgid "Lock/close topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
@@ -546,15 +546,15 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:122
 #, fuzzy
 #| msgid "Delete"
 msgid "Delete topic"
 msgstr "Видалити"
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
@@ -716,15 +716,15 @@
 msgstr[3] ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
 msgid "New"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
@@ -823,40 +823,44 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:28
+msgid "Go to first unread message"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
 msgid "Last post"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:73
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:112
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
@@ -981,15 +985,15 @@
 msgid "User profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:5
 msgid "Forum: Unread topics"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
```

### Comparing `aa_forum-2.2.1/aa_forum/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_forum-2.3.0/aa_forum/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_forum-2.3.0/aa_forum/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Dehao Wu <wudehao2000@163.com>, 2024.
 # Peter Pfeufer <info@ppfeufer.de>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:06+0000\n"
-"Last-Translator: Dehao Wu <wudehao2000@163.com>\n"
-"Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/zh_Hans/>\n"
-"Language: zh_Hans\n"
+"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"Language-Team: Polish <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-forum/pl/>\n"
+"Language: pl_PL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2;\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
@@ -33,24 +33,24 @@
 #: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
 #: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
 #: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
 #: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
 #: aa_forum/templates/aa_forum/view/profile/index.html:8
 #: aa_forum/templates/aa_forum/view/search/results.html:7
 msgid "Forum"
-msgstr "论坛"
+msgstr ""
 
 #: aa_forum/apps.py:20
 #, python-brace-format
 msgid "AA Forum v{__version__}"
 msgstr ""
 
 #: aa_forum/forms.py:42
 msgid "This field is mandatory"
-msgstr "这个字段是必填的"
+msgstr "To pole jest wymagane"
 
 #: aa_forum/forms.py:116 aa_forum/forms.py:118 aa_forum/forms.py:169
 #: aa_forum/forms.py:171 aa_forum/forms.py:616
 #: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:25
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:25
 msgid "Subject"
 msgstr ""
@@ -58,19 +58,19 @@
 #: aa_forum/forms.py:145 aa_forum/forms.py:422 aa_forum/forms.py:665
 #: aa_forum/forms.py:730
 msgid "You have forgotten the message!"
 msgstr ""
 
 #: aa_forum/forms.py:190 aa_forum/forms.py:228 aa_forum/forms.py:249
 msgid "Name"
-msgstr "名字"
+msgstr ""
 
 #: aa_forum/forms.py:192 aa_forum/forms.py:230
 msgid "Category name"
-msgstr "分类名称"
+msgstr ""
 
 #: aa_forum/forms.py:196 aa_forum/forms.py:207
 msgid "Boards"
 msgstr ""
 
 #: aa_forum/forms.py:198
 msgid ""
@@ -144,18 +144,16 @@
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so. This setting will not be inherited to child boards. (Hint: These "
 "restrictions only take effect when a board is marked as \"Announcement "
 "Board\", see checkbox above.)"
 msgstr ""
 
 #: aa_forum/forms.py:362
-#, fuzzy
-#| msgid "Close"
 msgid "Close topic"
-msgstr "关闭"
+msgstr ""
 
 #: aa_forum/forms.py:364
 msgid "If checked, this topic will be closed after posting this message."
 msgstr ""
 
 #: aa_forum/forms.py:370
 msgid "Reopen topic"
@@ -316,96 +314,96 @@
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:625
+#: aa_forum/models.py:623
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:626
+#: aa_forum/models.py:624
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:805
+#: aa_forum/models.py:803
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:806
+#: aa_forum/models.py:804
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:946
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:947
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:1003
+#: aa_forum/models.py:1001
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:1004
+#: aa_forum/models.py:1002
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:1005
+#: aa_forum/models.py:1003
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:1010
+#: aa_forum/models.py:1008
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:1015
+#: aa_forum/models.py:1013
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:1020
+#: aa_forum/models.py:1018
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:1031
+#: aa_forum/models.py:1029
 msgid "setting"
 msgstr ""
 
-#: aa_forum/models.py:1032
+#: aa_forum/models.py:1030
 msgid "settings"
 msgstr ""
 
-#: aa_forum/models.py:1042
+#: aa_forum/models.py:1040
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
 #: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr ""
 
-#: aa_forum/models.py:1069
+#: aa_forum/models.py:1067
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:1070
+#: aa_forum/models.py:1068
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:1080
+#: aa_forum/models.py:1078
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
 #: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
@@ -428,15 +426,15 @@
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:17
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:17
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:11
 #: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:11
 msgid "Close"
-msgstr "关闭"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-board.html:16
 msgid "Are you sure you want to delete this board?"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-board.html:17
 msgid "This will also remove all topics and messages in this board."
@@ -455,23 +453,23 @@
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:31
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:31
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:27
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:26
 #: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:26
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:35
 msgid "Cancel"
-msgstr "取消"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-board.html:32
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:32
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:32
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:31
 #: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:31
 msgid "Delete"
-msgstr "删除"
+msgstr "Usuń"
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:3
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:8
 #: aa_forum/templates/aa_forum/partials/administration/category-loop.html:25
 msgid "Delete category"
 msgstr ""
 
@@ -485,21 +483,21 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:91
 msgid "Unlock/re-open topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:101
 msgid "Lock/close topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
@@ -535,15 +533,15 @@
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:122
 msgid "Delete topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
@@ -674,39 +672,43 @@
 msgid "Search for:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
-msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
+msgstr ""
+"Chciałbyś pomóc w tłumaczeniu tej apki na Twój język bądź poprawić aktualne "
+"tłumaczenia?"
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "加入我们的翻译团队吧！"
+msgstr "Dołącz do naszego zespołu tłumaczy!"
 
 #: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:6
 msgid "Fields marked with an asterisk (*) are mandatory"
-msgstr "带有(*)星号符号的字段是必填的"
+msgstr "Pola z gwiazdką (*) są wymagane"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board-index.html:27
 msgid "No topics have been started in this board …"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
 msgid "New"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
@@ -805,40 +807,44 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:28
+msgid "Go to first unread message"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
 msgid "Last post"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:73
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:112
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
@@ -955,15 +961,15 @@
 msgid "User profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:5
 msgid "Forum: Unread topics"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
 
@@ -1028,14 +1034,16 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
 #: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
```

### Comparing `aa_forum-2.2.1/aa_forum/migrations/0001_initial.py` & `aa_forum-2.3.0/aa_forum/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/migrations/0002_default_settings.py` & `aa_forum-2.3.0/aa_forum/migrations/0002_default_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/migrations/0004_board_use_webhook_for_replies.py` & `aa_forum-2.3.0/aa_forum/migrations/0004_board_use_webhook_for_replies.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/migrations/0005_announcement_boards.py` & `aa_forum-2.3.0/aa_forum/migrations/0005_announcement_boards.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/migrations/0006_reset_default_settings.py` & `aa_forum-2.3.0/aa_forum/migrations/0006_reset_default_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/migrations/0007_change_settings_to_singleton.py` & `aa_forum-2.3.0/aa_forum/migrations/0007_change_settings_to_singleton.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/migrations/0008_populate_default_settings.py` & `aa_forum-2.3.0/aa_forum/migrations/0008_populate_default_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/migrations/0009_add_related_names.py` & `aa_forum-2.3.0/aa_forum/migrations/0009_add_related_names.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/migrations/0010_better_setting_names.py` & `aa_forum-2.3.0/aa_forum/migrations/0010_better_setting_names.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/migrations/0011_userprofile.py` & `aa_forum-2.3.0/aa_forum/migrations/0011_userprofile.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/migrations/0012_personal_messages.py` & `aa_forum-2.3.0/aa_forum/migrations/0012_personal_messages.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/migrations/0013_personal_messages_migrate_zero_fix.py` & `aa_forum-2.3.0/aa_forum/migrations/0013_personal_messages_migrate_zero_fix.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/migrations/0015_alter_board_use_webhook_for_replies.py` & `aa_forum-2.3.0/aa_forum/migrations/0015_alter_board_use_webhook_for_replies.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/migrations/0016_fix_quotation_marks.py` & `aa_forum-2.3.0/aa_forum/migrations/0016_fix_quotation_marks.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/migrations/0017_ckeditor5_and_dashboard_widgets.py` & `aa_forum-2.3.0/aa_forum/migrations/0017_ckeditor5_and_dashboard_widgets.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/scripts/drop_tables.sql` & `aa_forum-2.3.0/aa_forum/scripts/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/scripts/fake_messages.py` & `aa_forum-2.3.0/aa_forum/scripts/fake_messages.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/search/stopwords/LICENSE` & `aa_forum-2.3.0/aa_forum/search/stopwords/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-cs.json` & `aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-cs.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-de.json` & `aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-de.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-en.json` & `aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-en.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-es.json` & `aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-es.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-fr.json` & `aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-fr.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-it.json` & `aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-it.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-ja.json` & `aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-ja.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-ko.json` & `aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-ko.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-nl.json` & `aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-nl.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-pl.json` & `aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-pl.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-ru.json` & `aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-ru.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-sk.json` & `aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-sk.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-uk.json` & `aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-uk.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-zh.json` & `aa_forum-2.3.0/aa_forum/search/stopwords/stopwords-zh.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/css/aa-forum.css` & `aa_forum-2.3.0/aa_forum/static/aa_forum/css/aa-forum.css`

 * *Files 2% similar despite different names*

```diff
@@ -417,14 +417,22 @@
     }
 
     .aa-forum .ck-content .image-style-side {
         margin-left: var(--ck-image-style-spacing);
     }
 }
 
+/* Dashboard widget
+------------------------------------------------------------------------------------- */
+@media all {
+    #aa-forum-dashboard-widget-unread-topics .card-aa-forum-category:last-child {
+        margin-bottom: 0 !important;
+    }
+}
+
 /*
 ----------------------------------------------------------------------------------------
                 Responsive (@media all and (min-width: 768px))
 ----------------------------------------------------------------------------------------
 */
 
 /* Category view (@media all and (min-width: 768px))
```

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/css/aa-forum.min.css` & `aa_forum-2.3.0/aa_forum/static/aa_forum/css/aa-forum.min.css`

 * *Files 4% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-:root{--bg-hover-transition:background-color 0.25s linear}@media all{.aa-forum .aa-forum-svg-wrapper{height:0;width:0}.aa-forum .aa-forum-body #aa-forum-form-search-results .input-group{margin-bottom:1rem}.aa-forum .aa-forum-ui-placeholder{outline:1px dashed rgb(0 0 0)}.aa-forum .boards-sortable,.aa-forum .categories-sortable{list-style-type:none}.aa-forum .boards-sortable>li:first-child{margin-top:1rem}.aa-forum [data-bs-toggle=collapse].collapsed .if-expanded{display:none}.aa-forum [data-bs-toggle=collapse]:not(.collapsed) .if-collapsed{display:none}.aa-forum .category-sortable{cursor:move}.aa-forum .aa-forum-breadcrumb ul{list-style-type:none;padding:0}.aa-forum .aa-forum-breadcrumb ul li{display:inline}.aa-forum .aa-forum-breadcrumb ul li:first-child{padding-left:0}.aa-forum .card-aa-forum-category .aa-forum-board{flex-direction:row;transition:var(--bg-hover-transition)}.aa-forum .card-aa-forum-category .aa-forum-board:last-child{margin-bottom:0}.aa-forum .card-aa-forum-category .aa-forum-board:hover{background:rgb(0 0 0/5%)}.aa-forum .card-aa-forum-category .aa-forum-board-image svg{height:65px;margin-top:-1rem;width:65px}.aa-forum .card-aa-forum-category .aa-forum-board-name{width:100%}.aa-forum .aa-forum-board-name p:last-child{margin:0}.aa-forum .aa-forum-board-group-restrictions{list-style-type:none;margin:0;padding:0}.aa-forum .aa-forum-board-last-post .img-last-post-avatar{float:left;height:55px;margin-right:1rem;width:55px}.aa-forum .aa-forum-board-last-post .last-post-information{overflow:hidden;text-overflow:ellipsis;white-space:nowrap;word-wrap:normal}.aa-forum .aa-forum-legend>span{display:flex;margin-right:5rem}.aa-forum .aa-forum-legend .aa-forum-legend-image svg{height:30px;width:30px}.aa-forum .aa-forum-legend .aa-forum-legend-text{display:inline-block}.aa-forum .aa-forum-legend span:last-child{margin-right:0}.aa-forum .aa-forum-topic-row .aa-forum-topic{align-content:center;align-items:center;display:flex;flex-direction:row;transition:var(--bg-hover-transition)}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name p:last-child,.aa-forum .aa-forum-topic-row:last-child .aa-forum-topic{margin-bottom:0}.aa-forum .aa-forum-topic-row .aa-forum-topic:hover{background:rgb(0 0 0/5%)}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image{width:40px}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image svg{height:35px;margin-top:-1rem;width:35px}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name{width:auto}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-stats{text-align:center;width:15%}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-last-post{width:25%}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-actions{width:70px}.aa-forum .aa-forum-topic-locked{background-color:rgb(185 199 219/25%)}.aa-forum .aa-forum-topic-sticky{background-color:rgb(255 220 104/25%)}.aa-forum .label-aa-forum-topic-new-message{font-size:55%}.aa-forum .label-aa-forum-child-board-new-message{font-size:55%;margin-left:.25rem;padding:.3em .6em;vertical-align:middle}.aa-forum .aa-forum-message-author .img-author-avatar{max-width:100%}.aa-forum .aa-forum-message-wrapper{width:auto}.aa-forum .aa-forum-message-body{border-top:1px solid rgb(236 240 241)}.aa-forum .aa-forum-message-body-author-signature{border-top:1px solid rgb(236 240 241);margin-top:3em}.aa-forum .aa-forum-message-body-last-edited{margin-top:5rem}.aa-forum .aa-forum-message-body img{height:auto!important;max-width:100%}.aa-forum .aa-forum-search-result-inner{align-items:flex-start;display:flex;flex-flow:row nowrap;place-content:flex-start flex-start}.aa-forum .aa-forum-search-results-total-number{font-size:2rem;font-weight:bolder;margin-bottom:2rem}.aa-forum .aa-forum-search-result-counter{font-size:3rem;font-weight:bolder;margin-right:1rem;min-width:50px;padding:1rem}.aa-forum .aa-forum-search-result-details{width:100%}.aa-forum .aa-forum-search-term-highlight{color:rgb(255 114 0)!important;font-size:1.1em;font-weight:700}.aa-forum .card-aa-forum-personal-messages-item{padding:1rem;transition:var(--bg-hover-transition)}.aa-forum .card-aa-forum-personal-messages-item:hover{background:rgb(0 0 0/5%)}.aa-forum .card-aa-forum-personal-messages-item-header{border-bottom:1px solid rgb(236 240 241);font-weight:700}.aa-forum .card-aa-forum-personal-messages-item-unread{font-weight:700}.aa-forum .aa-forum-personal-messages-message .card{margin-top:2rem}.aa-forum li.aa-forum-messages-sidebar-menu-item:has(a.active){background-color:var(--bs-secondary-bg-subtle)}.aa-forum li.aa-forum-messages-sidebar-menu-item>a.active{color:rgb(var(--bs-primary-rgb))}.aa-forum .aa-forum-lightbox-modal{align-items:center;display:flex!important;justify-content:center;z-index:-1}.aa-forum .aa-forum-lightbox-modal .modal-dialog{display:inline-block;height:auto!important;max-height:95%;max-width:95%;width:auto!important}.aa-forum .aa-forum-lightbox-modal.fade.in{z-index:1050}.aa-forum .btn-aa-forum-topic-moderation{background:0 0}.aa-forum .btn-aa-forum-topic-moderation.focus,.aa-forum .btn-aa-forum-topic-moderation:focus,.aa-forum .btn-aa-forum-topic-moderation:hover{color:inherit;outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}.aa-forum .btn-aa-forum-delete{color:rgb(255 0 0)}.aa-forum .SumoSelect p{border-radius:var(--bs-border-radius);height:auto}.aa-forum .SumoSelect{color:rgb(54 54 54);display:block}.aa-forum .SumoSelect>.CaptionCont>label>i{background-image:none}.aa-forum .SumoSelect>.CaptionCont>span.placeholder{background-color:transparent;color:rgb(62 68 76);opacity:1}.aa-forum .select2-container--bootstrap-5{max-width:100%!important}.aa-forum .ck-rounded-corners{--ck-border-radius:var(--bs-border-radius)}.aa-forum .ck-editor__editable{color:initial}.aa-forum .ck-word-count{color:var(--bs-secondary-color)!important;--bs-text-opacity:1}.aa-forum .ck-content .image{margin:.9em 0}.aa-forum .ck-content .image-style-align-center{margin-left:auto;margin-right:auto}.aa-forum .ck-content .image-style-align-left{margin-right:var(--ck-image-style-spacing)}.aa-forum .ck-content .image-style-align-right,.aa-forum .ck-content .image-style-side{margin-left:var(--ck-image-style-spacing)}}@media all and (min-width:768px){.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name,.aa-forum .card-aa-forum-category .aa-forum-board-name{width:60%}.aa-forum .card-aa-forum-category .aa-forum-board-stats{text-align:center;width:15%}.aa-forum .card-aa-forum-category .aa-forum-board-last-post{width:25%}.aa-forum .aa-forum-legend{display:flex}.aa-forum .aa-forum-message{align-items:flex-start;display:flex;flex-wrap:nowrap}.aa-forum .aa-forum-message-author figure{width:auto}.aa-forum .aa-forum-message-author{min-width:150px;width:150px}.aa-forum .aa-forum-message-wrapper{width:100%}}@media all and (min-width:992px){.aa-forum .card-aa-forum-personal-messages-item,.aa-forum .card-aa-forum-personal-messages-item-header{align-items:center;display:flex;flex-flow:row nowrap;place-content:flex-start flex-start}.aa-forum .aa-forum-personal-message-date,.aa-forum .aa-forum-personal-message-recipient,.aa-forum .aa-forum-personal-message-sender{min-width:200px}.aa-forum .aa-forum-personal-message-subject{width:100%}}@media all{.aa-forum figure.media .oembed-video{height:auto;max-width:100%;overflow:hidden;padding-bottom:56.25%;position:relative}.aa-forum figure.media .oembed-video>iframe{height:100%;left:0;position:absolute;top:0;width:100%}}
+:root{--bg-hover-transition:background-color 0.25s linear}@media all{.aa-forum .aa-forum-svg-wrapper{height:0;width:0}.aa-forum .aa-forum-body #aa-forum-form-search-results .input-group{margin-bottom:1rem}.aa-forum .aa-forum-ui-placeholder{outline:1px dashed rgb(0 0 0)}.aa-forum .boards-sortable,.aa-forum .categories-sortable{list-style-type:none}.aa-forum .boards-sortable>li:first-child{margin-top:1rem}.aa-forum [data-bs-toggle=collapse].collapsed .if-expanded{display:none}.aa-forum [data-bs-toggle=collapse]:not(.collapsed) .if-collapsed{display:none}.aa-forum .category-sortable{cursor:move}.aa-forum .aa-forum-breadcrumb ul{list-style-type:none;padding:0}.aa-forum .aa-forum-breadcrumb ul li{display:inline}.aa-forum .aa-forum-breadcrumb ul li:first-child{padding-left:0}.aa-forum .card-aa-forum-category .aa-forum-board{flex-direction:row;transition:var(--bg-hover-transition)}.aa-forum .card-aa-forum-category .aa-forum-board:last-child{margin-bottom:0}.aa-forum .card-aa-forum-category .aa-forum-board:hover{background:rgb(0 0 0/5%)}.aa-forum .card-aa-forum-category .aa-forum-board-image svg{height:65px;margin-top:-1rem;width:65px}.aa-forum .card-aa-forum-category .aa-forum-board-name{width:100%}.aa-forum .aa-forum-board-name p:last-child{margin:0}.aa-forum .aa-forum-board-group-restrictions{list-style-type:none;margin:0;padding:0}.aa-forum .aa-forum-board-last-post .img-last-post-avatar{float:left;height:55px;margin-right:1rem;width:55px}.aa-forum .aa-forum-board-last-post .last-post-information{overflow:hidden;text-overflow:ellipsis;white-space:nowrap;word-wrap:normal}.aa-forum .aa-forum-legend>span{display:flex;margin-right:5rem}.aa-forum .aa-forum-legend .aa-forum-legend-image svg{height:30px;width:30px}.aa-forum .aa-forum-legend .aa-forum-legend-text{display:inline-block}.aa-forum .aa-forum-legend span:last-child{margin-right:0}.aa-forum .aa-forum-topic-row .aa-forum-topic{align-content:center;align-items:center;display:flex;flex-direction:row;transition:var(--bg-hover-transition)}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name p:last-child,.aa-forum .aa-forum-topic-row:last-child .aa-forum-topic{margin-bottom:0}.aa-forum .aa-forum-topic-row .aa-forum-topic:hover{background:rgb(0 0 0/5%)}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image{width:40px}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image svg{height:35px;margin-top:-1rem;width:35px}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name{width:auto}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-stats{text-align:center;width:15%}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-last-post{width:25%}.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-actions{width:70px}.aa-forum .aa-forum-topic-locked{background-color:rgb(185 199 219/25%)}.aa-forum .aa-forum-topic-sticky{background-color:rgb(255 220 104/25%)}.aa-forum .label-aa-forum-topic-new-message{font-size:55%}.aa-forum .label-aa-forum-child-board-new-message{font-size:55%;margin-left:.25rem;padding:.3em .6em;vertical-align:middle}.aa-forum .aa-forum-message-author .img-author-avatar{max-width:100%}.aa-forum .aa-forum-message-wrapper{width:auto}.aa-forum .aa-forum-message-body{border-top:1px solid rgb(236 240 241)}.aa-forum .aa-forum-message-body-author-signature{border-top:1px solid rgb(236 240 241);margin-top:3em}.aa-forum .aa-forum-message-body-last-edited{margin-top:5rem}.aa-forum .aa-forum-message-body img{height:auto!important;max-width:100%}.aa-forum .aa-forum-search-result-inner{align-items:flex-start;display:flex;flex-flow:row nowrap;place-content:flex-start flex-start}.aa-forum .aa-forum-search-results-total-number{font-size:2rem;font-weight:bolder;margin-bottom:2rem}.aa-forum .aa-forum-search-result-counter{font-size:3rem;font-weight:bolder;margin-right:1rem;min-width:50px;padding:1rem}.aa-forum .aa-forum-search-result-details{width:100%}.aa-forum .aa-forum-search-term-highlight{color:rgb(255 114 0)!important;font-size:1.1em;font-weight:700}.aa-forum .card-aa-forum-personal-messages-item{padding:1rem;transition:var(--bg-hover-transition)}.aa-forum .card-aa-forum-personal-messages-item:hover{background:rgb(0 0 0/5%)}.aa-forum .card-aa-forum-personal-messages-item-header{border-bottom:1px solid rgb(236 240 241);font-weight:700}.aa-forum .card-aa-forum-personal-messages-item-unread{font-weight:700}.aa-forum .aa-forum-personal-messages-message .card{margin-top:2rem}.aa-forum li.aa-forum-messages-sidebar-menu-item:has(a.active){background-color:var(--bs-secondary-bg-subtle)}.aa-forum li.aa-forum-messages-sidebar-menu-item>a.active{color:rgb(var(--bs-primary-rgb))}.aa-forum .aa-forum-lightbox-modal{align-items:center;display:flex!important;justify-content:center;z-index:-1}.aa-forum .aa-forum-lightbox-modal .modal-dialog{display:inline-block;height:auto!important;max-height:95%;max-width:95%;width:auto!important}.aa-forum .aa-forum-lightbox-modal.fade.in{z-index:1050}.aa-forum .btn-aa-forum-topic-moderation{background:0 0}.aa-forum .btn-aa-forum-topic-moderation.focus,.aa-forum .btn-aa-forum-topic-moderation:focus,.aa-forum .btn-aa-forum-topic-moderation:hover{color:inherit;outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}.aa-forum .btn-aa-forum-delete{color:rgb(255 0 0)}.aa-forum .SumoSelect p{border-radius:var(--bs-border-radius);height:auto}.aa-forum .SumoSelect{color:rgb(54 54 54);display:block}.aa-forum .SumoSelect>.CaptionCont>label>i{background-image:none}.aa-forum .SumoSelect>.CaptionCont>span.placeholder{background-color:transparent;color:rgb(62 68 76);opacity:1}.aa-forum .select2-container--bootstrap-5{max-width:100%!important}.aa-forum .ck-rounded-corners{--ck-border-radius:var(--bs-border-radius)}.aa-forum .ck-editor__editable{color:initial}.aa-forum .ck-word-count{color:var(--bs-secondary-color)!important;--bs-text-opacity:1}.aa-forum .ck-content .image{margin:.9em 0}.aa-forum .ck-content .image-style-align-center{margin-left:auto;margin-right:auto}.aa-forum .ck-content .image-style-align-left{margin-right:var(--ck-image-style-spacing)}.aa-forum .ck-content .image-style-align-right,.aa-forum .ck-content .image-style-side{margin-left:var(--ck-image-style-spacing)}#aa-forum-dashboard-widget-unread-topics .card-aa-forum-category:last-child{margin-bottom:0!important}}@media all and (min-width:768px){.aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name,.aa-forum .card-aa-forum-category .aa-forum-board-name{width:60%}.aa-forum .card-aa-forum-category .aa-forum-board-stats{text-align:center;width:15%}.aa-forum .card-aa-forum-category .aa-forum-board-last-post{width:25%}.aa-forum .aa-forum-legend{display:flex}.aa-forum .aa-forum-message{align-items:flex-start;display:flex;flex-wrap:nowrap}.aa-forum .aa-forum-message-author figure{width:auto}.aa-forum .aa-forum-message-author{min-width:150px;width:150px}.aa-forum .aa-forum-message-wrapper{width:100%}}@media all and (min-width:992px){.aa-forum .card-aa-forum-personal-messages-item,.aa-forum .card-aa-forum-personal-messages-item-header{align-items:center;display:flex;flex-flow:row nowrap;place-content:flex-start flex-start}.aa-forum .aa-forum-personal-message-date,.aa-forum .aa-forum-personal-message-recipient,.aa-forum .aa-forum-personal-message-sender{min-width:200px}.aa-forum .aa-forum-personal-message-subject{width:100%}}@media all{.aa-forum figure.media .oembed-video{height:auto;max-width:100%;overflow:hidden;padding-bottom:56.25%;position:relative}.aa-forum figure.media .oembed-video>iframe{height:100%;left:0;position:absolute;top:0;width:100%}}
 /*# sourceMappingURL=aa-forum.min.css.map */
```

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/css/aa-forum.min.css.map` & `aa_forum-2.3.0/aa_forum/static/aa_forum/css/aa-forum.min.css.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'mappings'": "'AAEA,K,CACI,mD,CAKJ,WACI,+B,CACI,Q,CACA,O,CAOJ,mE,CACI,kB,CAOJ,kC,CACI,6B,CAIJ,0B,CADA,8B,CAEI,oB,CAGJ,yC,CACI,e,CAGJ,0D,CACI,Y,CAGJ,wCAA0C,yB,CACtC,Y,CAGJ,4B,CACI,W,CAOJ,iC,CACI,oB,CACA,S,CAGJ,oC,CACI,c,CAGJ,gD,CACI,c,CAOJ,iD,CACI,kB,CACA,qC,CAGJ,4D,CACI,e,CAGJ,uD,CACI,wB,CAGJ,2D,CACI,W,CACA,gB,CACA,U,CAGJ,sD,CACI,U,CAGJ,2C,CACI,Q,CAGJ,4C,CACI,oB,CACA,Q,CACA,S,CAGJ,yD,CACI,U,CACA,W,CACA,iB,CACA,U,CAGJ,0D,CACI,e,CACA,sB,CACA,kB,CACA,gB,CAGJ,+B,CACI,Y,CACA,iB,CAGJ,qD,CACI,W,CACA,U,CAGJ,gD,CA […]*

```diff
@@ -1,12 +1,12 @@
 {
     "file": "aa-forum.css",
-    "mappings": "AAEA,K,CACI,mD,CAKJ,WACI,+B,CACI,Q,CACA,O,CAOJ,mE,CACI,kB,CAOJ,kC,CACI,6B,CAIJ,0B,CADA,8B,CAEI,oB,CAGJ,yC,CACI,e,CAGJ,0D,CACI,Y,CAGJ,wCAA0C,yB,CACtC,Y,CAGJ,4B,CACI,W,CAOJ,iC,CACI,oB,CACA,S,CAGJ,oC,CACI,c,CAGJ,gD,CACI,c,CAOJ,iD,CACI,kB,CACA,qC,CAGJ,4D,CACI,e,CAGJ,uD,CACI,wB,CAGJ,2D,CACI,W,CACA,gB,CACA,U,CAGJ,sD,CACI,U,CAGJ,2C,CACI,Q,CAGJ,4C,CACI,oB,CACA,Q,CACA,S,CAGJ,yD,CACI,U,CACA,W,CACA,iB,CACA,U,CAGJ,0D,CACI,e,CACA,sB,CACA,kB,CACA,gB,CAGJ,+B,CACI,Y,CACA,iB,CAGJ,qD,CACI,W,CACA,U,CAGJ,gD,CACI,oB,CAGJ,0C,CACI,c,CAOJ,6C,CACI,oB,CACA,kB,CACA,Y,CACA,kB,CACA,qC,CAyBJ,+E,CAtBA,wD,CACI,e,CAGJ,mD,CACI,wB,CAGJ,mE,CACI,U,CAGJ,uE,CACI,W,CACA,gB,CACA,U,CAGJ,kE,CACI,U,CAOJ,mE,CACI,iB,CACA,S,CAGJ,uE,CACI,S,CAGJ,qE,CACI,U,CAGJ,gC,CACI,qC,CAGJ,gC,CACI,qC,CAGJ,2C,CACI,a,CAGJ,iD,CACI,a,CACA,kB,CACA,iB,CACA,qB,CAOJ,qD,CACI,c,CAGJ,mC,CACI,U,CAGJ,gC,CACI,qC,CAGJ,iD,CACI,qC,CACA,c,CAGJ,4C,CACI,e,CAGJ,oC,CACI,qB,CACA,c,CAOJ,uC,CACI,sB,CACA,Y,CACA,oB,CACA,mC,CAGJ,+C,CACI,c,CACA,kB,CACA,kB,CAGJ,yC,CACI,c,CACA,kB,CACA,iB,CACA,c,CACA,Y,CAGJ,yC,CACI,U,CAGJ,yC,CACI,8B,CACA,e,CACA,e,CAOJ,+C,CACI,Y,CACA,qC,CAGJ,qD,CACI,wB,CAGJ,sD,CACI,wC,CACA,e,CAGJ,sD,CACI,e,CAGJ,mD,CACI,e,CAGJ,qDAAqD,S,CACjD,8C,CAGJ,yD,CACI,gC,CAOJ,kC,CACI,kB,CACA,sB,CACA,sB,CACA,U,CAGJ,gD,CACI,oB,CACA,qB,CACA,c,CACA,a,CACA,oB,CAGJ,0C,CACI,Y,CAOJ,wC,CACI,c,CAGJ,8C,CACA,8C,CACA,8C,CACI,a,CACA,yC,CACA,mB,CAGJ,8B,CACI,kB,CAOJ,uB,CACI,qC,CACA,W,CAGJ,qB,CACI,mB,CACA,a,CAGJ,0C,CACI,qB,CAGJ,mD,CACI,4B,CACA,mB,CACA,S,CAOJ,yC,CACI,wB,CAOJ,6B,CACI,0C,CAGJ,8B,CACI,a,CAGJ,wB,CACI,yC,CAEA,mB,CAKJ,4B,CACI,a,CAGJ,+C,CACI,gB,CACA,iB,CAGJ,6C,CACI,0C,CAGJ,8C,CAIA,uC,CAHI,2CAgBR,A,iCAsBI,kE,CArBA,sD,CACI,S,CAGJ,uD,CACI,iB,CACA,S,CAGJ,2D,CACI,S,CAGJ,0B,CACI,Y,CAeJ,2B,CACI,sB,CACA,Y,CACA,gB,CAGJ,yC,CACI,U,CAGJ,kC,CACI,e,CACA,W,CAGJ,mC,CACI,YAYR,A,iCAEI,+C,CADA,sD,CAEI,kB,CACA,Y,CACA,oB,CACA,mC,CAGJ,yC,CAKA,8C,CADA,2C,CAHI,e,CAQJ,4C,CACI,YAMR,A,WACI,oC,CACI,W,CACA,c,CACA,e,CACA,qB,CACA,iB,CAGJ,2C,CACI,W,CACA,M,CACA,iB,CACA,K,CACA,Y",
+    "mappings": "AAEA,K,CACI,mD,CAKJ,WACI,+B,CACI,Q,CACA,O,CAOJ,mE,CACI,kB,CAOJ,kC,CACI,6B,CAIJ,0B,CADA,8B,CAEI,oB,CAGJ,yC,CACI,e,CAGJ,0D,CACI,Y,CAGJ,wCAA0C,yB,CACtC,Y,CAGJ,4B,CACI,W,CAOJ,iC,CACI,oB,CACA,S,CAGJ,oC,CACI,c,CAGJ,gD,CACI,c,CAOJ,iD,CACI,kB,CACA,qC,CAGJ,4D,CACI,e,CAGJ,uD,CACI,wB,CAGJ,2D,CACI,W,CACA,gB,CACA,U,CAGJ,sD,CACI,U,CAGJ,2C,CACI,Q,CAGJ,4C,CACI,oB,CACA,Q,CACA,S,CAGJ,yD,CACI,U,CACA,W,CACA,iB,CACA,U,CAGJ,0D,CACI,e,CACA,sB,CACA,kB,CACA,gB,CAGJ,+B,CACI,Y,CACA,iB,CAGJ,qD,CACI,W,CACA,U,CAGJ,gD,CACI,oB,CAGJ,0C,CACI,c,CAOJ,6C,CACI,oB,CACA,kB,CACA,Y,CACA,kB,CACA,qC,CAyBJ,+E,CAtBA,wD,CACI,e,CAGJ,mD,CACI,wB,CAGJ,mE,CACI,U,CAGJ,uE,CACI,W,CACA,gB,CACA,U,CAGJ,kE,CACI,U,CAOJ,mE,CACI,iB,CACA,S,CAGJ,uE,CACI,S,CAGJ,qE,CACI,U,CAGJ,gC,CACI,qC,CAGJ,gC,CACI,qC,CAGJ,2C,CACI,a,CAGJ,iD,CACI,a,CACA,kB,CACA,iB,CACA,qB,CAOJ,qD,CACI,c,CAGJ,mC,CACI,U,CAGJ,gC,CACI,qC,CAGJ,iD,CACI,qC,CACA,c,CAGJ,4C,CACI,e,CAGJ,oC,CACI,qB,CACA,c,CAOJ,uC,CACI,sB,CACA,Y,CACA,oB,CACA,mC,CAGJ,+C,CACI,c,CACA,kB,CACA,kB,CAGJ,yC,CACI,c,CACA,kB,CACA,iB,CACA,c,CACA,Y,CAGJ,yC,CACI,U,CAGJ,yC,CACI,8B,CACA,e,CACA,e,CAOJ,+C,CACI,Y,CACA,qC,CAGJ,qD,CACI,wB,CAGJ,sD,CACI,wC,CACA,e,CAGJ,sD,CACI,e,CAGJ,mD,CACI,e,CAGJ,qDAAqD,S,CACjD,8C,CAGJ,yD,CACI,gC,CAOJ,kC,CACI,kB,CACA,sB,CACA,sB,CACA,U,CAGJ,gD,CACI,oB,CACA,qB,CACA,c,CACA,a,CACA,oB,CAGJ,0C,CACI,Y,CAOJ,wC,CACI,c,CAGJ,8C,CACA,8C,CACA,8C,CACI,a,CACA,yC,CACA,mB,CAGJ,8B,CACI,kB,CAOJ,uB,CACI,qC,CACA,W,CAGJ,qB,CACI,mB,CACA,a,CAGJ,0C,CACI,qB,CAGJ,mD,CACI,4B,CACA,mB,CACA,S,CAOJ,yC,CACI,wB,CAOJ,6B,CACI,0C,CAGJ,8B,CACI,a,CAGJ,wB,CACI,yC,CAEA,mB,CAKJ,4B,CACI,a,CAGJ,+C,CACI,gB,CACA,iB,CAGJ,6C,CACI,0C,CAGJ,8C,CAIA,uC,CAHI,yC,CAWJ,2E,CACI,2BAYR,A,iCAsBI,kE,CArBA,sD,CACI,S,CAGJ,uD,CACI,iB,CACA,S,CAGJ,2D,CACI,S,CAGJ,0B,CACI,Y,CAeJ,2B,CACI,sB,CACA,Y,CACA,gB,CAGJ,yC,CACI,U,CAGJ,kC,CACI,e,CACA,W,CAGJ,mC,CACI,YAYR,A,iCAEI,+C,CADA,sD,CAEI,kB,CACA,Y,CACA,oB,CACA,mC,CAGJ,yC,CAKA,8C,CADA,2C,CAHI,e,CAQJ,4C,CACI,YAMR,A,WACI,oC,CACI,W,CACA,c,CACA,e,CACA,qB,CACA,iB,CAGJ,2C,CACI,W,CACA,M,CACA,iB,CACA,K,CACA,Y",
     "names": [],
     "sources": [
         "aa-forum.css"
     ],
     "sourcesContent": [
-        "/* Variable definitions\n------------------------------------------------------------------------------------- */\n:root {\n    --bg-hover-transition: background-color 0.25s linear;\n}\n\n/* General\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-svg-wrapper {\n        height: 0;\n        width: 0;\n    }\n}\n\n/* Search Box\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-body #aa-forum-form-search-results .input-group {\n        margin-bottom: 1rem;\n    }\n}\n\n/* Administration :: Sortable categories and boards\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-ui-placeholder {\n        outline: 1px dashed rgb(0 0 0);\n    }\n\n    .aa-forum .categories-sortable,\n    .aa-forum .boards-sortable {\n        list-style-type: none;\n    }\n\n    .aa-forum .boards-sortable > li:first-child {\n        margin-top: 1rem;\n    }\n\n    .aa-forum [data-bs-toggle=\"collapse\"].collapsed .if-expanded {\n        display: none;\n    }\n\n    .aa-forum [data-bs-toggle=\"collapse\"]:not(.collapsed) .if-collapsed {\n        display: none;\n    }\n\n    .aa-forum .category-sortable {\n        cursor: move;\n    }\n}\n\n/* Breadcrumb\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-breadcrumb ul {\n        list-style-type: none;\n        padding: 0;\n    }\n\n    .aa-forum .aa-forum-breadcrumb ul li {\n        display: inline;\n    }\n\n    .aa-forum .aa-forum-breadcrumb ul li:first-child {\n        padding-left: 0;\n    }\n}\n\n/* Category view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .card-aa-forum-category .aa-forum-board {\n        flex-direction: row;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board:last-child {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-image svg {\n        height: 65px;\n        margin-top: -1rem;\n        width: 65px;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-name {\n        width: 100%;\n    }\n\n    .aa-forum .aa-forum-board-name p:last-child {\n        margin: 0;\n    }\n\n    .aa-forum .aa-forum-board-group-restrictions {\n        list-style-type: none;\n        margin: 0;\n        padding: 0;\n    }\n\n    .aa-forum .aa-forum-board-last-post .img-last-post-avatar {\n        float: left;\n        height: 55px;\n        margin-right: 1rem;\n        width: 55px;\n    }\n\n    .aa-forum .aa-forum-board-last-post .last-post-information {\n        overflow: hidden;\n        text-overflow: ellipsis;\n        white-space: nowrap;\n        word-wrap: normal;\n    }\n\n    .aa-forum .aa-forum-legend > span {\n        display: flex;\n        margin-right: 5rem;\n    }\n\n    .aa-forum .aa-forum-legend .aa-forum-legend-image svg {\n        height: 30px;\n        width: 30px;\n    }\n\n    .aa-forum .aa-forum-legend .aa-forum-legend-text {\n        display: inline-block;\n    }\n\n    .aa-forum .aa-forum-legend span:last-child {\n        margin-right: 0;\n    }\n}\n\n/* Board view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-topic-row .aa-forum-topic {\n        align-content: center;\n        align-items: center;\n        display: flex;\n        flex-direction: row;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .aa-forum-topic-row:last-child .aa-forum-topic {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image {\n        width: 40px;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image svg {\n        height: 35px;\n        margin-top: -1rem;\n        width: 35px;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name p:last-child {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-stats {\n        text-align: center;\n        width: 15%;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-last-post {\n        width: 25%;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-actions {\n        width: 70px;\n    }\n\n    .aa-forum .aa-forum-topic-locked {\n        background-color: rgb(185 199 219 / 25%);\n    }\n\n    .aa-forum .aa-forum-topic-sticky {\n        background-color: rgb(255 220 104 / 25%);\n    }\n\n    .aa-forum .label-aa-forum-topic-new-message {\n        font-size: 55%;\n    }\n\n    .aa-forum .label-aa-forum-child-board-new-message {\n        font-size: 55%;\n        margin-left: 0.25rem;\n        padding: 0.3em 0.6em;\n        vertical-align: middle;\n    }\n}\n\n/* Message view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-message-author .img-author-avatar {\n        max-width: 100%;\n    }\n\n    .aa-forum .aa-forum-message-wrapper {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-message-body {\n        border-top: 1px solid rgb(236 240 241);\n    }\n\n    .aa-forum .aa-forum-message-body-author-signature {\n        border-top: 1px solid rgb(236 240 241);\n        margin-top: 3em;\n    }\n\n    .aa-forum .aa-forum-message-body-last-edited {\n        margin-top: 5rem;\n    }\n\n    .aa-forum .aa-forum-message-body img {\n        height: auto !important; /* to override inline style added by CKEditor */\n        max-width: 100%;\n    }\n}\n\n/* Search view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-search-result-inner {\n        align-items: flex-start;\n        display: flex;\n        flex-flow: row nowrap;\n        place-content: flex-start flex-start;\n    }\n\n    .aa-forum .aa-forum-search-results-total-number {\n        font-size: 2rem;\n        font-weight: bolder;\n        margin-bottom: 2rem;\n    }\n\n    .aa-forum .aa-forum-search-result-counter {\n        font-size: 3rem;\n        font-weight: bolder;\n        margin-right: 1rem;\n        min-width: 50px;\n        padding: 1rem;\n    }\n\n    .aa-forum .aa-forum-search-result-details {\n        width: 100%;\n    }\n\n    .aa-forum .aa-forum-search-term-highlight {\n        color: rgb(255 114 0) !important;\n        font-size: 1.1em;\n        font-weight: bold;\n    }\n}\n\n/* Personal messages view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .card-aa-forum-personal-messages-item {\n        padding: 1rem;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item-header {\n        border-bottom: 1px solid rgb(236 240 241);\n        font-weight: 700;\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item-unread {\n        font-weight: 700;\n    }\n\n    .aa-forum .aa-forum-personal-messages-message .card {\n        margin-top: 2rem;\n    }\n\n    .aa-forum li.aa-forum-messages-sidebar-menu-item:has(a.active) {\n        background-color: var(--bs-secondary-bg-subtle);\n    }\n\n    .aa-forum li.aa-forum-messages-sidebar-menu-item > a.active {\n        color: rgb(var(--bs-primary-rgb));\n    }\n}\n\n/* Lightbox\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-lightbox-modal {\n        align-items: center;\n        display: flex !important;\n        justify-content: center;\n        z-index: -1;\n    }\n\n    .aa-forum .aa-forum-lightbox-modal .modal-dialog {\n        display: inline-block;\n        height: auto !important;\n        max-height: 95%;\n        max-width: 95%;\n        width: auto !important;\n    }\n\n    .aa-forum .aa-forum-lightbox-modal.fade.in {\n        z-index: 1050;\n    }\n}\n\n/* Buttons\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .btn-aa-forum-topic-moderation {\n        background: none;\n    }\n\n    .aa-forum .btn-aa-forum-topic-moderation.focus,\n    .aa-forum .btn-aa-forum-topic-moderation:focus,\n    .aa-forum .btn-aa-forum-topic-moderation:hover {\n        color: inherit;\n        outline: 5px auto -webkit-focus-ring-color;\n        outline-offset: -2px;\n    }\n\n    .aa-forum .btn-aa-forum-delete {\n        color: rgb(255 0 0);\n    }\n}\n\n/* SumoSelect\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .SumoSelect p {\n        border-radius: var(--bs-border-radius);\n        height: auto;\n    }\n\n    .aa-forum .SumoSelect {\n        color: rgb(54 54 54);\n        display: block;\n    }\n\n    .aa-forum .SumoSelect > .CaptionCont > label > i {\n        background-image: none;\n    }\n\n    .aa-forum .SumoSelect > .CaptionCont > span.placeholder {\n        background-color: transparent;\n        color: rgb(62 68 76);\n        opacity: 1;\n    }\n}\n\n/* Select2\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .select2-container--bootstrap-5 {\n        max-width: 100% !important;\n    }\n}\n\n/* CKEditor 5 (WYSIWYG editor)\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .ck-rounded-corners {\n        --ck-border-radius: var(--bs-border-radius);\n    }\n\n    .aa-forum .ck-editor__editable {\n        color: initial;\n    }\n\n    .aa-forum .ck-word-count {\n        color: var(--bs-secondary-color) !important;\n\n        --bs-text-opacity: 1;\n    }\n\n    /* Image alignment\n    --------------------------------------------------------------------------------- */\n    .aa-forum .ck-content .image {\n        margin: 0.9em 0;\n    }\n\n    .aa-forum .ck-content .image-style-align-center {\n        margin-left: auto;\n        margin-right: auto;\n    }\n\n    .aa-forum .ck-content .image-style-align-left {\n        margin-right: var(--ck-image-style-spacing);\n    }\n\n    .aa-forum .ck-content .image-style-align-right {\n        margin-left: var(--ck-image-style-spacing);\n    }\n\n    .aa-forum .ck-content .image-style-side {\n        margin-left: var(--ck-image-style-spacing);\n    }\n}\n\n/*\n----------------------------------------------------------------------------------------\n                Responsive (@media all and (min-width: 768px))\n----------------------------------------------------------------------------------------\n*/\n\n/* Category view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .card-aa-forum-category .aa-forum-board-name {\n        width: 60%;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-stats {\n        text-align: center;\n        width: 15%;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-last-post {\n        width: 25%;\n    }\n\n    .aa-forum .aa-forum-legend {\n        display: flex;\n    }\n}\n\n/* Board view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name {\n        width: 60%;\n    }\n}\n\n/* Message view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .aa-forum-message {\n        align-items: flex-start;\n        display: flex;\n        flex-wrap: nowrap;\n    }\n\n    .aa-forum .aa-forum-message-author figure {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-message-author {\n        min-width: 150px;\n        width: 150px;\n    }\n\n    .aa-forum .aa-forum-message-wrapper {\n        width: 100%;\n    }\n}\n\n/*\n----------------------------------------------------------------------------------------\n                Responsive (@media all and (min-width: 992px))\n----------------------------------------------------------------------------------------\n*/\n\n/* Personal messages view (@media all and (min-width: 992px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 992px) {\n    .aa-forum .card-aa-forum-personal-messages-item-header,\n    .aa-forum .card-aa-forum-personal-messages-item {\n        align-items: center;\n        display: flex;\n        flex-flow: row nowrap;\n        place-content: flex-start flex-start;\n    }\n\n    .aa-forum .aa-forum-personal-message-date {\n        min-width: 200px;\n    }\n\n    .aa-forum .aa-forum-personal-message-sender,\n    .aa-forum .aa-forum-personal-message-recipient {\n        min-width: 200px;\n    }\n\n    .aa-forum .aa-forum-personal-message-subject {\n        width: 100%;\n    }\n}\n\n/* Fix for oEmbed videos\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum figure.media .oembed-video {\n        height: auto;\n        max-width: 100%;\n        overflow: hidden;\n        padding-bottom: 56.25%;\n        position: relative;\n    }\n\n    .aa-forum figure.media .oembed-video > iframe {\n        height: 100%;\n        left: 0;\n        position: absolute;\n        top: 0;\n        width: 100%;\n    }\n}\n"
+        "/* Variable definitions\n------------------------------------------------------------------------------------- */\n:root {\n    --bg-hover-transition: background-color 0.25s linear;\n}\n\n/* General\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-svg-wrapper {\n        height: 0;\n        width: 0;\n    }\n}\n\n/* Search Box\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-body #aa-forum-form-search-results .input-group {\n        margin-bottom: 1rem;\n    }\n}\n\n/* Administration :: Sortable categories and boards\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-ui-placeholder {\n        outline: 1px dashed rgb(0 0 0);\n    }\n\n    .aa-forum .categories-sortable,\n    .aa-forum .boards-sortable {\n        list-style-type: none;\n    }\n\n    .aa-forum .boards-sortable > li:first-child {\n        margin-top: 1rem;\n    }\n\n    .aa-forum [data-bs-toggle=\"collapse\"].collapsed .if-expanded {\n        display: none;\n    }\n\n    .aa-forum [data-bs-toggle=\"collapse\"]:not(.collapsed) .if-collapsed {\n        display: none;\n    }\n\n    .aa-forum .category-sortable {\n        cursor: move;\n    }\n}\n\n/* Breadcrumb\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-breadcrumb ul {\n        list-style-type: none;\n        padding: 0;\n    }\n\n    .aa-forum .aa-forum-breadcrumb ul li {\n        display: inline;\n    }\n\n    .aa-forum .aa-forum-breadcrumb ul li:first-child {\n        padding-left: 0;\n    }\n}\n\n/* Category view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .card-aa-forum-category .aa-forum-board {\n        flex-direction: row;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board:last-child {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-image svg {\n        height: 65px;\n        margin-top: -1rem;\n        width: 65px;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-name {\n        width: 100%;\n    }\n\n    .aa-forum .aa-forum-board-name p:last-child {\n        margin: 0;\n    }\n\n    .aa-forum .aa-forum-board-group-restrictions {\n        list-style-type: none;\n        margin: 0;\n        padding: 0;\n    }\n\n    .aa-forum .aa-forum-board-last-post .img-last-post-avatar {\n        float: left;\n        height: 55px;\n        margin-right: 1rem;\n        width: 55px;\n    }\n\n    .aa-forum .aa-forum-board-last-post .last-post-information {\n        overflow: hidden;\n        text-overflow: ellipsis;\n        white-space: nowrap;\n        word-wrap: normal;\n    }\n\n    .aa-forum .aa-forum-legend > span {\n        display: flex;\n        margin-right: 5rem;\n    }\n\n    .aa-forum .aa-forum-legend .aa-forum-legend-image svg {\n        height: 30px;\n        width: 30px;\n    }\n\n    .aa-forum .aa-forum-legend .aa-forum-legend-text {\n        display: inline-block;\n    }\n\n    .aa-forum .aa-forum-legend span:last-child {\n        margin-right: 0;\n    }\n}\n\n/* Board view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-topic-row .aa-forum-topic {\n        align-content: center;\n        align-items: center;\n        display: flex;\n        flex-direction: row;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .aa-forum-topic-row:last-child .aa-forum-topic {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image {\n        width: 40px;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image svg {\n        height: 35px;\n        margin-top: -1rem;\n        width: 35px;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name p:last-child {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-stats {\n        text-align: center;\n        width: 15%;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-last-post {\n        width: 25%;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-actions {\n        width: 70px;\n    }\n\n    .aa-forum .aa-forum-topic-locked {\n        background-color: rgb(185 199 219 / 25%);\n    }\n\n    .aa-forum .aa-forum-topic-sticky {\n        background-color: rgb(255 220 104 / 25%);\n    }\n\n    .aa-forum .label-aa-forum-topic-new-message {\n        font-size: 55%;\n    }\n\n    .aa-forum .label-aa-forum-child-board-new-message {\n        font-size: 55%;\n        margin-left: 0.25rem;\n        padding: 0.3em 0.6em;\n        vertical-align: middle;\n    }\n}\n\n/* Message view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-message-author .img-author-avatar {\n        max-width: 100%;\n    }\n\n    .aa-forum .aa-forum-message-wrapper {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-message-body {\n        border-top: 1px solid rgb(236 240 241);\n    }\n\n    .aa-forum .aa-forum-message-body-author-signature {\n        border-top: 1px solid rgb(236 240 241);\n        margin-top: 3em;\n    }\n\n    .aa-forum .aa-forum-message-body-last-edited {\n        margin-top: 5rem;\n    }\n\n    .aa-forum .aa-forum-message-body img {\n        height: auto !important; /* to override inline style added by CKEditor */\n        max-width: 100%;\n    }\n}\n\n/* Search view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-search-result-inner {\n        align-items: flex-start;\n        display: flex;\n        flex-flow: row nowrap;\n        place-content: flex-start flex-start;\n    }\n\n    .aa-forum .aa-forum-search-results-total-number {\n        font-size: 2rem;\n        font-weight: bolder;\n        margin-bottom: 2rem;\n    }\n\n    .aa-forum .aa-forum-search-result-counter {\n        font-size: 3rem;\n        font-weight: bolder;\n        margin-right: 1rem;\n        min-width: 50px;\n        padding: 1rem;\n    }\n\n    .aa-forum .aa-forum-search-result-details {\n        width: 100%;\n    }\n\n    .aa-forum .aa-forum-search-term-highlight {\n        color: rgb(255 114 0) !important;\n        font-size: 1.1em;\n        font-weight: bold;\n    }\n}\n\n/* Personal messages view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .card-aa-forum-personal-messages-item {\n        padding: 1rem;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item-header {\n        border-bottom: 1px solid rgb(236 240 241);\n        font-weight: 700;\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item-unread {\n        font-weight: 700;\n    }\n\n    .aa-forum .aa-forum-personal-messages-message .card {\n        margin-top: 2rem;\n    }\n\n    .aa-forum li.aa-forum-messages-sidebar-menu-item:has(a.active) {\n        background-color: var(--bs-secondary-bg-subtle);\n    }\n\n    .aa-forum li.aa-forum-messages-sidebar-menu-item > a.active {\n        color: rgb(var(--bs-primary-rgb));\n    }\n}\n\n/* Lightbox\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-lightbox-modal {\n        align-items: center;\n        display: flex !important;\n        justify-content: center;\n        z-index: -1;\n    }\n\n    .aa-forum .aa-forum-lightbox-modal .modal-dialog {\n        display: inline-block;\n        height: auto !important;\n        max-height: 95%;\n        max-width: 95%;\n        width: auto !important;\n    }\n\n    .aa-forum .aa-forum-lightbox-modal.fade.in {\n        z-index: 1050;\n    }\n}\n\n/* Buttons\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .btn-aa-forum-topic-moderation {\n        background: none;\n    }\n\n    .aa-forum .btn-aa-forum-topic-moderation.focus,\n    .aa-forum .btn-aa-forum-topic-moderation:focus,\n    .aa-forum .btn-aa-forum-topic-moderation:hover {\n        color: inherit;\n        outline: 5px auto -webkit-focus-ring-color;\n        outline-offset: -2px;\n    }\n\n    .aa-forum .btn-aa-forum-delete {\n        color: rgb(255 0 0);\n    }\n}\n\n/* SumoSelect\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .SumoSelect p {\n        border-radius: var(--bs-border-radius);\n        height: auto;\n    }\n\n    .aa-forum .SumoSelect {\n        color: rgb(54 54 54);\n        display: block;\n    }\n\n    .aa-forum .SumoSelect > .CaptionCont > label > i {\n        background-image: none;\n    }\n\n    .aa-forum .SumoSelect > .CaptionCont > span.placeholder {\n        background-color: transparent;\n        color: rgb(62 68 76);\n        opacity: 1;\n    }\n}\n\n/* Select2\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .select2-container--bootstrap-5 {\n        max-width: 100% !important;\n    }\n}\n\n/* CKEditor 5 (WYSIWYG editor)\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .ck-rounded-corners {\n        --ck-border-radius: var(--bs-border-radius);\n    }\n\n    .aa-forum .ck-editor__editable {\n        color: initial;\n    }\n\n    .aa-forum .ck-word-count {\n        color: var(--bs-secondary-color) !important;\n\n        --bs-text-opacity: 1;\n    }\n\n    /* Image alignment\n    --------------------------------------------------------------------------------- */\n    .aa-forum .ck-content .image {\n        margin: 0.9em 0;\n    }\n\n    .aa-forum .ck-content .image-style-align-center {\n        margin-left: auto;\n        margin-right: auto;\n    }\n\n    .aa-forum .ck-content .image-style-align-left {\n        margin-right: var(--ck-image-style-spacing);\n    }\n\n    .aa-forum .ck-content .image-style-align-right {\n        margin-left: var(--ck-image-style-spacing);\n    }\n\n    .aa-forum .ck-content .image-style-side {\n        margin-left: var(--ck-image-style-spacing);\n    }\n}\n\n/* Dashboard widget\n------------------------------------------------------------------------------------- */\n@media all {\n    #aa-forum-dashboard-widget-unread-topics .card-aa-forum-category:last-child {\n        margin-bottom: 0 !important;\n    }\n}\n\n/*\n----------------------------------------------------------------------------------------\n                Responsive (@media all and (min-width: 768px))\n----------------------------------------------------------------------------------------\n*/\n\n/* Category view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .card-aa-forum-category .aa-forum-board-name {\n        width: 60%;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-stats {\n        text-align: center;\n        width: 15%;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-last-post {\n        width: 25%;\n    }\n\n    .aa-forum .aa-forum-legend {\n        display: flex;\n    }\n}\n\n/* Board view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name {\n        width: 60%;\n    }\n}\n\n/* Message view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .aa-forum-message {\n        align-items: flex-start;\n        display: flex;\n        flex-wrap: nowrap;\n    }\n\n    .aa-forum .aa-forum-message-author figure {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-message-author {\n        min-width: 150px;\n        width: 150px;\n    }\n\n    .aa-forum .aa-forum-message-wrapper {\n        width: 100%;\n    }\n}\n\n/*\n----------------------------------------------------------------------------------------\n                Responsive (@media all and (min-width: 992px))\n----------------------------------------------------------------------------------------\n*/\n\n/* Personal messages view (@media all and (min-width: 992px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 992px) {\n    .aa-forum .card-aa-forum-personal-messages-item-header,\n    .aa-forum .card-aa-forum-personal-messages-item {\n        align-items: center;\n        display: flex;\n        flex-flow: row nowrap;\n        place-content: flex-start flex-start;\n    }\n\n    .aa-forum .aa-forum-personal-message-date {\n        min-width: 200px;\n    }\n\n    .aa-forum .aa-forum-personal-message-sender,\n    .aa-forum .aa-forum-personal-message-recipient {\n        min-width: 200px;\n    }\n\n    .aa-forum .aa-forum-personal-message-subject {\n        width: 100%;\n    }\n}\n\n/* Fix for oEmbed videos\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum figure.media .oembed-video {\n        height: auto;\n        max-width: 100%;\n        overflow: hidden;\n        padding-bottom: 56.25%;\n        position: relative;\n    }\n\n    .aa-forum figure.media .oembed-video > iframe {\n        height: 100%;\n        left: 0;\n        position: absolute;\n        top: 0;\n        width: 100%;\n    }\n}\n"
     ],
     "version": 3
 }
```

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.js` & `aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js` & `aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js.map` & `aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.js` & `aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js` & `aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js.map` & `aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.js` & `aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js` & `aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js.map` & `aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.js` & `aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js` & `aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js.map` & `aa_forum-2.3.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/LICENSE.md` & `aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.css` & `aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.min.css` & `aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.js` & `aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.min.js` & `aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.js` & `aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.min.js` & `aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/LICENSE` & `aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.css` & `aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css` & `aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css.map` & `aa_forum-2.3.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.js` & `aa_forum-2.3.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.min.js` & `aa_forum-2.3.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.css` & `aa_forum-2.3.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.min.css` & `aa_forum-2.3.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.min.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/base.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/base.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/select2-css.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/bundles/select2-css.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/svg/aa-forum-icons.svg` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/bundles/svg/aa-forum-icons.svg`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/administration/delete-board.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/modals/administration/delete-board.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/administration/delete-category.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/modals/administration/delete-category.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/breadcrumb.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/board-loop.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/administration/board-loop.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/categories.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/administration/categories.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/category-loop.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/administration/category-loop.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/new-category.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/administration/new-category.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/settings-form.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/administration/settings-form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/board-index.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/board/board-index.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/board.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/board/board.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/pagination.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/board/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/topic.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/board/topic.html`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
                 <a href="{{ topic.get_absolute_url }}">{{ topic.subject }}</a>
 
                 {% if topic.has_unread_messages %}
                     <a
                         id="aa-forum-link-new-{{ topic.id }}"
                         href="{% url 'aa_forum:forum_topic_first_unread_message' topic.board.category.slug topic.board.slug topic.slug %}"
                         class="badge bg-warning label-aa-forum-topic-new-message ms-2"
+                        title="{% translate 'Go to first unread message' %}"
+                        data-bs-tooltip="aa-forum"
                     >
                         {% translate "New" %}
                     </a>
                 {% endif %}
                 <br>
                 <span class="small">
                     {% if topic.is_sticky %}
```

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/message.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/topic/message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/reply.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/topic/reply.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/menu/menu-admin.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/menu/menu-admin.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/menu/menu-user.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/menu/menu-user.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/profile/form.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/profile/form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/search/pagination.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/search/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/search/search-form.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/partials/search/search-form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/administration/categories-and-boards.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/view/administration/categories-and-boards.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/board.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/view/forum/board.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/index.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/view/forum/index.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/modify-message.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/view/forum/modify-message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/modify-topic.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/view/forum/modify-topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/new-topic.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/view/forum/new-topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/topic.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/view/forum/topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/unread-topics.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/view/forum/unread-topics.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/personal-messages/inbox.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/view/personal-messages/inbox.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/personal-messages/new-message.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/view/personal-messages/new-message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/personal-messages/reply-message.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/view/personal-messages/reply-message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/profile/index.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/view/profile/index.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/search/results.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/view/search/results.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/widgets/dashboard-widgets.html` & `aa_forum-2.3.0/aa_forum/templates/aa_forum/view/widgets/dashboard-widgets.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% if perms.aa_forum.basic_access %}
-    <div id="aa-forum-dashboard-widgets" class="col-12 align-self-stretch py-2 collapse">
+    <div id="aa-forum-dashboard-widgets" class="aa-forum col-12 align-self-stretch py-2 collapse">
         {% if user_profile.show_unread_topics_dashboard_widget %}
-            <div id="aa-forum-dashboard-widget-unread-topics" class="col-12 align-self-stretch py-2 collapse">
+            <div id="aa-forum-dashboard-widget-unread-topics" class="col-12 align-self-stretch collapse">
                 <div class="aa-forum-dashboard-widget-unread-topics-content"></div>
             </div>
         {% endif %}
 
         <div class="aa-forum-svg-wrapper">
             {% include "aa_forum/bundles/svg/aa-forum-icons.svg" %}
         </div>
```

### Comparing `aa_forum-2.2.1/aa_forum/templatetags/aa_forum.py` & `aa_forum-2.3.0/aa_forum/templatetags/aa_forum.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/tests/test_app_settings.py` & `aa_forum-2.3.0/aa_forum/tests/test_app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/tests/test_auth_hooks.py` & `aa_forum-2.3.0/aa_forum/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/tests/test_helpers.py` & `aa_forum-2.3.0/aa_forum/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/tests/test_integration.py` & `aa_forum-2.3.0/aa_forum/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/tests/test_managers.py` & `aa_forum-2.3.0/aa_forum/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/tests/test_models.py` & `aa_forum-2.3.0/aa_forum/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/tests/test_signals.py` & `aa_forum-2.3.0/aa_forum/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/tests/test_templatetags.py` & `aa_forum-2.3.0/aa_forum/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/tests/test_views_admin.py` & `aa_forum-2.3.0/aa_forum/tests/test_views_admin.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/tests/test_views_forum.py` & `aa_forum-2.3.0/aa_forum/tests/test_views_forum.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/tests/utils.py` & `aa_forum-2.3.0/aa_forum/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/views/admin.py` & `aa_forum-2.3.0/aa_forum/views/admin.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/views/forum.py` & `aa_forum-2.3.0/aa_forum/views/forum.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/views/personal_messages.py` & `aa_forum-2.3.0/aa_forum/views/personal_messages.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/views/profile.py` & `aa_forum-2.3.0/aa_forum/views/profile.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/views/search.py` & `aa_forum-2.3.0/aa_forum/views/search.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/aa_forum/views/widgets.py` & `aa_forum-2.3.0/aa_forum/views/widgets.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/LICENSE` & `aa_forum-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.1/README.md` & `aa_forum-2.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
 ![Screenshot: Admin View]
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA Forum >= 2.0.0 needs at least Alliance Auth v4.0.0!**
+> **AA Forum >= 2.0.0 needs at least Alliance Auth v4!**
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
 >
 > The last version of AA Forum that supports Alliance Auth v3 is `1.19.5`.
```

### Comparing `aa_forum-2.2.1/pyproject.toml` & `aa_forum-2.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dynamic = [
     "version",
 ]
 dependencies = [
-    "allianceauth<5.0.0,>=4",
+    "allianceauth<5.0.0,>=4.1",
     "allianceauth-app-utils>=1.24",
     "dhooks-lite>=1.1",
     "django-ckeditor-5>=0.2.13",
     "unidecode>=1.3.7",
 ]
 [project.optional-dependencies]
 tests-allianceauth-latest = [
```

### Comparing `aa_forum-2.2.1/PKG-INFO` & `aa_forum-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aa-forum
-Version: 2.2.1
+Version: 2.3.0
 Summary: Simple forum for Alliance Auth
 Project-URL: Changelog, https://github.com/ppfeufer/aa-forum/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-forum/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-forum
 Project-URL: Source, https://github.com/ppfeufer/aa-forum.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-forum/issues
@@ -698,15 +698,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Requires-Dist: allianceauth-app-utils>=1.24
-Requires-Dist: allianceauth<5.0.0,>=4
+Requires-Dist: allianceauth<5.0.0,>=4.1
 Requires-Dist: dhooks-lite>=1.1
 Requires-Dist: django-ckeditor-5>=0.2.13
 Requires-Dist: unidecode>=1.3.7
 Provides-Extra: tests-allianceauth-latest
 Requires-Dist: aa-timezones; extra == 'tests-allianceauth-latest'
 Requires-Dist: allianceauth-discordbot; extra == 'tests-allianceauth-latest'
 Requires-Dist: coverage; extra == 'tests-allianceauth-latest'
@@ -819,15 +819,15 @@
 
 ![Screenshot: Admin View]
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA Forum >= 2.0.0 needs at least Alliance Auth v4.0.0!**
+> **AA Forum >= 2.0.0 needs at least Alliance Auth v4!**
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
 >
 > The last version of AA Forum that supports Alliance Auth v3 is `1.19.5`.
```

