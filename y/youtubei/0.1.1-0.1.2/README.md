# Comparing `tmp/youtubei-0.1.1.tar.gz` & `tmp/youtubei-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtubei-0.1.1.tar", max compression
+gzip compressed data, was "youtubei-0.1.2.tar", max compression
```

## Comparing `youtubei-0.1.1.tar` & `youtubei-0.1.2.tar`

### file list

```diff
@@ -1,182 +1,189 @@
--rw-r--r--   0        0        0     1067 2024-01-07 14:35:08.333602 youtubei-0.1.1/LICENSE
--rw-r--r--   0        0        0       37 2024-03-24 15:33:03.141373 youtubei-0.1.1/README.md
--rw-r--r--   0        0        0      547 2024-03-24 15:57:53.263177 youtubei-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      163 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/__init__.py
--rw-r--r--   0        0        0      294 2024-02-21 23:27:18.155210 youtubei-0.1.1/youtubei/_registries.py
--rw-r--r--   0        0        0      137 2024-02-21 23:27:18.155210 youtubei-0.1.1/youtubei/clients/__init__.py
--rw-r--r--   0        0        0      242 2024-02-21 23:27:18.155210 youtubei-0.1.1/youtubei/clients/android/__init__.py
--rw-r--r--   0        0        0      520 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/android/constants.py
--rw-r--r--   0        0        0      270 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/android/parser.py
--rw-r--r--   0        0        0      612 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/android/responses.py
--rw-r--r--   0        0        0      360 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/android/types.py
--rw-r--r--   0        0        0      706 2024-03-24 15:57:53.263177 youtubei-0.1.1/youtubei/clients/android/wrapper.py
--rw-r--r--   0        0        0      206 2024-02-21 23:27:18.155210 youtubei-0.1.1/youtubei/clients/ios/__init__.py
--rw-r--r--   0        0        0      449 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/ios/constants.py
--rw-r--r--   0        0        0      250 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/ios/parser.py
--rw-r--r--   0        0        0      574 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/ios/responses.py
--rw-r--r--   0        0        0      360 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/ios/types.py
--rw-r--r--   0        0        0      666 2024-03-24 15:57:53.263177 youtubei-0.1.1/youtubei/clients/ios/wrapper.py
--rw-r--r--   0        0        0      255 2024-02-21 23:27:18.159209 youtubei-0.1.1/youtubei/clients/ios_music/__init__.py
--rw-r--r--   0        0        0      547 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/ios_music/constants.py
--rw-r--r--   0        0        0      275 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/ios_music/parser.py
--rw-r--r--   0        0        0      859 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/ios_music/responses.py
--rw-r--r--   0        0        0      720 2024-03-24 15:57:53.263177 youtubei-0.1.1/youtubei/clients/ios_music/wrapper.py
--rw-r--r--   0        0        0      206 2024-02-21 23:27:18.159209 youtubei-0.1.1/youtubei/clients/web/__init__.py
--rw-r--r--   0        0        0      458 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/web/constants.py
--rw-r--r--   0        0        0      382 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/web/parser.py
--rw-r--r--   0        0        0     2033 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/web/responses.py
--rw-r--r--   0        0        0      919 2024-03-24 15:57:53.263177 youtubei-0.1.1/youtubei/clients/web/wrapper.py
--rw-r--r--   0        0        0      255 2024-02-21 23:27:18.159209 youtubei-0.1.1/youtubei/clients/web_remix/__init__.py
--rw-r--r--   0        0        0      557 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/web_remix/constants.py
--rw-r--r--   0        0        0     2486 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/web_remix/models.py
--rw-r--r--   0        0        0      883 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/web_remix/parser.py
--rw-r--r--   0        0        0     1517 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/web_remix/responses.py
--rw-r--r--   0        0        0      385 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/clients/web_remix/types.py
--rw-r--r--   0        0        0     1601 2024-03-24 15:57:53.263177 youtubei-0.1.1/youtubei/clients/web_remix/wrapper.py
--rw-r--r--   0        0        0       84 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/enums/__init__.py
--rw-r--r--   0        0        0      130 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/enums/_base.py
--rw-r--r--   0        0        0      732 2024-03-24 15:33:03.141373 youtubei-0.1.1/youtubei/enums/action.py
--rw-r--r--   0        0        0    42633 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/enums/icon.py
--rw-r--r--   0        0        0     1673 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/enums/music.py
--rw-r--r--   0        0        0    14843 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/enums/other.py
--rw-r--r--   0        0        0      482 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/__init__.py
--rw-r--r--   0        0        0      204 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/_base.py
--rw-r--r--   0        0        0      366 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/accessibility.py
--rw-r--r--   0        0        0     4497 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/actions.py
--rw-r--r--   0        0        0     1536 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/ad.py
--rw-r--r--   0        0        0      344 2024-03-24 15:57:53.263177 youtubei-0.1.1/youtubei/models/colour.py
--rw-r--r--   0        0        0     1046 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/command.py
--rw-r--r--   0        0        0    11757 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/commands.py
--rw-r--r--   0        0        0     1395 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/config.py
--rw-r--r--   0        0        0      345 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/contexts.py
--rw-r--r--   0        0        0      225 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/data.py
--rw-r--r--   0        0        0      464 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/data_bound.py
--rw-r--r--   0        0        0    13456 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/endpoints.py
--rw-r--r--   0        0        0      655 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/logging.py
--rw-r--r--   0        0        0      663 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/metadata.py
--rw-r--r--   0        0        0      424 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/music.py
--rw-r--r--   0        0        0     5797 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/other.py
--rw-r--r--   0        0        0      305 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/params.py
--rw-r--r--   0        0        0      497 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/reminders.py
--rw-r--r--   0        0        0     1051 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/response.py
--rw-r--r--   0        0        0     1660 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/text.py
--rw-r--r--   0        0        0      869 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/models/thumbnail.py
--rw-r--r--   0        0        0      243 2024-02-21 23:27:18.167209 youtubei-0.1.1/youtubei/parse/__init__.py
--rw-r--r--   0        0        0      217 2024-02-21 23:27:18.167209 youtubei-0.1.1/youtubei/parse/constants.py
--rw-r--r--   0        0        0       80 2024-02-21 23:27:18.167209 youtubei-0.1.1/youtubei/parse/exceptions.py
--rw-r--r--   0        0        0      777 2024-03-24 15:57:53.263177 youtubei-0.1.1/youtubei/parse/parser.py
--rw-r--r--   0        0        0      342 2024-02-21 23:27:18.167209 youtubei-0.1.1/youtubei/parse/registry.py
--rw-r--r--   0        0        0      252 2024-02-21 23:27:18.167209 youtubei-0.1.1/youtubei/parse/types.py
--rw-r--r--   0        0        0      206 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/parse/utils.py
--rw-r--r--   0        0        0      241 2024-02-21 23:27:18.167209 youtubei-0.1.1/youtubei/parse/validated_types.py
--rw-r--r--   0        0        0      845 2024-02-21 23:27:18.167209 youtubei-0.1.1/youtubei/parse/validators.py
--rw-r--r--   0        0        0      553 2024-03-24 15:37:35.348062 youtubei-0.1.1/youtubei/parser.py
--rw-r--r--   0        0        0        0 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/py.typed
--rw-r--r--   0        0        0     5720 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/__init__.py
--rw-r--r--   0        0        0      177 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/_base.py
--rw-r--r--   0        0        0      193 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/about_this_ad.py
--rw-r--r--   0        0        0      174 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/ad_break_service.py
--rw-r--r--   0        0        0      229 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/ad_duration_remaining.py
--rw-r--r--   0        0        0      320 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/ad_hover_text_button.py
--rw-r--r--   0        0        0      425 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/ad_placement.py
--rw-r--r--   0        0        0      504 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/ad_preview.py
--rw-r--r--   0        0        0      432 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/ad_slot.py
--rw-r--r--   0        0        0      226 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/audio_only_playability.py
--rw-r--r--   0        0        0      618 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/background_promo.py
--rw-r--r--   0        0        0     1132 2024-03-24 15:57:53.263177 youtubei-0.1.1/youtubei/renderers/button.py
--rw-r--r--   0        0        0      306 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/card.py
--rw-r--r--   0        0        0      493 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/card_collection.py
--rw-r--r--   0        0        0      445 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/checkbox.py
--rw-r--r--   0        0        0      465 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/cinematic_container.py
--rw-r--r--   0        0        0      136 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/client_forecasting_ad.py
--rw-r--r--   0        0        0      491 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/compact_link.py
--rw-r--r--   0        0        0      571 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/confirm_dialog.py
--rw-r--r--   0        0        0      274 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/cropped_square_thumbnail.py
--rw-r--r--   0        0        0     1024 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/desktop_topbar.py
--rw-r--r--   0        0        0      280 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/endscreen.py
--rw-r--r--   0        0        0      812 2024-03-24 15:57:53.263177 youtubei-0.1.1/youtubei/renderers/endscreen_element.py
--rw-r--r--   0        0        0      538 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/engagement_panel_section_list.py
--rw-r--r--   0        0        0      278 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/engagement_panel_title_header.py
--rw-r--r--   0        0        0      710 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/fusion_searchbox.py
--rw-r--r--   0        0        0      816 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/guide_entry.py
--rw-r--r--   0        0        0      480 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/guide_section.py
--rw-r--r--   0        0        0      441 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/guide_signin_promo.py
--rw-r--r--   0        0        0      655 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/hero_playlist_thumbnail.py
--rw-r--r--   0        0        0      561 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/hotkey_dialog.py
--rw-r--r--   0        0        0      505 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/hotkey_dialog_section.py
--rw-r--r--   0        0        0      432 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/hotkey_dialog_section_option.py
--rw-r--r--   0        0        0      122 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/info_card_icon.py
--rw-r--r--   0        0        0      772 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/instream_ad_player_overlay.py
--rw-r--r--   0        0        0     1102 2024-03-24 15:57:53.263177 youtubei-0.1.1/youtubei/renderers/instream_video_ad.py
--rw-r--r--   0        0        0      346 2024-03-24 15:33:03.145373 youtubei-0.1.1/youtubei/renderers/item_section.py
--rw-r--r--   0        0        0      567 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/like_button.py
--rw-r--r--   0        0        0      277 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/linear_ad_sequence.py
--rw-r--r--   0        0        0      278 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/lugash_footer.py
--rw-r--r--   0        0        0     1166 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/menu.py
--rw-r--r--   0        0        0      667 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/menu_navigation_item.py
--rw-r--r--   0        0        0      601 2024-03-24 15:57:53.263177 youtubei-0.1.1/youtubei/renderers/menu_service_item.py
--rw-r--r--   0        0        0      313 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/metadata_badge.py
--rw-r--r--   0        0        0     1774 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/microformat_data.py
--rw-r--r--   0        0        0      182 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/miniplayer.py
--rw-r--r--   0        0        0      899 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/mobile_topbar.py
--rw-r--r--   0        0        0      504 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/modal_with_title_and_button.py
--rw-r--r--   0        0        0      764 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/multi_page_menu.py
--rw-r--r--   0        0        0      649 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/multi_page_menu_section.py
--rw-r--r--   0        0        0      199 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/music_carousel_shelf.py
--rw-r--r--   0        0        0      591 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/music_data_bound_menu.py
--rw-r--r--   0        0        0      778 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/music_detail_header.py
--rw-r--r--   0        0        0      743 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/music_item_thumbnail_overlay.py
--rw-r--r--   0        0        0      930 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/music_play_button.py
--rw-r--r--   0        0        0      549 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/music_playlist_shelf.py
--rw-r--r--   0        0        0     1483 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/music_responsive_list_item.py
--rw-r--r--   0        0        0      537 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/music_responsive_list_item_fixed_column.py
--rw-r--r--   0        0        0      482 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/music_responsive_list_item_flex_column.py
--rw-r--r--   0        0        0      586 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/music_shelf.py
--rw-r--r--   0        0        0      205 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/music_shelf_divider.py
--rw-r--r--   0        0        0      411 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/music_thumbnail.py
--rw-r--r--   0        0        0      278 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/notification_text.py
--rw-r--r--   0        0        0      424 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/pivot_bar.py
--rw-r--r--   0        0        0      753 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/pivot_bar_item.py
--rw-r--r--   0        0        0      281 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/player_annotations_expanded.py
--rw-r--r--   0        0        0      222 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/player_attestations.py
--rw-r--r--   0        0        0      629 2024-03-24 15:57:53.263177 youtubei-0.1.1/youtubei/renderers/player_bytes_ad_layout.py
--rw-r--r--   0        0        0      315 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/player_bytes_sequential_layout.py
--rw-r--r--   0        0        0      419 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/player_captions_tracklist.py
--rw-r--r--   0        0        0      310 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/player_error_message.py
--rw-r--r--   0        0        0      333 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/player_legacy_desktop_watch_ads.py
--rw-r--r--   0        0        0      765 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/player_microformat.py
--rw-r--r--   0        0        0      259 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/player_storyboard_spec.py
--rw-r--r--   0        0        0      268 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/playlist_byline.py
--rw-r--r--   0        0        0      271 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/playlist_custom_thumbnail.py
--rw-r--r--   0        0        0     1710 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/playlist_header.py
--rw-r--r--   0        0        0      261 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/playlist_metadata.py
--rw-r--r--   0        0        0      435 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/playlist_sidebar.py
--rw-r--r--   0        0        0     1109 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/playlist_sidebar_primary_info.py
--rw-r--r--   0        0        0     1232 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/playlist_video.py
--rw-r--r--   0        0        0      471 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/playlist_video_list.py
--rw-r--r--   0        0        0      624 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/privacy_tos_footer.py
--rw-r--r--   0        0        0      355 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/reel_player_overlay.py
--rw-r--r--   0        0        0      994 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/section_list.py
--rw-r--r--   0        0        0      558 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/simple_ad_badge.py
--rw-r--r--   0        0        0      345 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/simple_card_teaser.py
--rw-r--r--   0        0        0      373 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/single_column_browse_results.py
--rw-r--r--   0        0        0      296 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/skip_ad.py
--rw-r--r--   0        0        0      184 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/skip_button.py
--rw-r--r--   0        0        0      770 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/subscribe_button.py
--rw-r--r--   0        0        0      418 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/tab.py
--rw-r--r--   0        0        0      319 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/thumbnail_overlay_hover_text.py
--rw-r--r--   0        0        0      269 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/thumbnail_overlay_now_playing.py
--rw-r--r--   0        0        0      319 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/thumbnail_overlay_side_panel.py
--rw-r--r--   0        0        0      357 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/thumbnail_overlay_time_status.py
--rw-r--r--   0        0        0     1073 2024-03-24 15:33:03.149373 youtubei-0.1.1/youtubei/renderers/toggle_button.py
--rw-r--r--   0        0        0      414 2024-03-24 15:33:03.153373 youtubei-0.1.1/youtubei/renderers/topbar_button.py
--rw-r--r--   0        0        0      580 2024-03-24 15:33:03.153373 youtubei-0.1.1/youtubei/renderers/topbar_logo.py
--rw-r--r--   0        0        0      921 2024-03-24 15:57:53.263177 youtubei-0.1.1/youtubei/renderers/topbar_menu_button.py
--rw-r--r--   0        0        0      402 2024-03-24 15:33:03.153373 youtubei-0.1.1/youtubei/renderers/two_column_browse_results.py
--rw-r--r--   0        0        0      215 2024-03-24 15:33:03.153373 youtubei-0.1.1/youtubei/renderers/unified_share_panel.py
--rw-r--r--   0        0        0      477 2024-03-24 15:33:03.153373 youtubei-0.1.1/youtubei/renderers/upload_progress_arrow.py
--rw-r--r--   0        0        0      527 2024-03-24 15:33:03.153373 youtubei-0.1.1/youtubei/renderers/watch_break.py
--rw-r--r--   0        0        0      216 2024-03-24 15:33:03.153373 youtubei-0.1.1/youtubei/types.py
--rw-r--r--   0        0        0      342 2024-03-24 14:12:43.309436 youtubei-0.1.1/youtubei/validated_types.py
--rw-r--r--   0        0        0     1075 2024-03-24 15:33:03.153373 youtubei-0.1.1/youtubei/validators.py
--rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 youtubei-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-01-07 14:35:08.333602 youtubei-0.1.2/LICENSE
+-rw-r--r--   0        0        0       37 2024-03-24 15:33:03.141373 youtubei-0.1.2/README.md
+-rw-r--r--   0        0        0      547 2024-05-27 15:45:27.493767 youtubei-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      163 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/__init__.py
+-rw-r--r--   0        0        0      294 2024-02-21 23:27:18.155210 youtubei-0.1.2/youtubei/_registries.py
+-rw-r--r--   0        0        0      137 2024-02-21 23:27:18.155210 youtubei-0.1.2/youtubei/clients/__init__.py
+-rw-r--r--   0        0        0      242 2024-02-21 23:27:18.155210 youtubei-0.1.2/youtubei/clients/android/__init__.py
+-rw-r--r--   0        0        0      520 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/clients/android/constants.py
+-rw-r--r--   0        0        0      270 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/clients/android/parser.py
+-rw-r--r--   0        0        0      612 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/clients/android/responses.py
+-rw-r--r--   0        0        0      360 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/clients/android/types.py
+-rw-r--r--   0        0        0      706 2024-03-24 15:57:53.263177 youtubei-0.1.2/youtubei/clients/android/wrapper.py
+-rw-r--r--   0        0        0      206 2024-02-21 23:27:18.155210 youtubei-0.1.2/youtubei/clients/ios/__init__.py
+-rw-r--r--   0        0        0      449 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/clients/ios/constants.py
+-rw-r--r--   0        0        0      250 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/clients/ios/parser.py
+-rw-r--r--   0        0        0      574 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/clients/ios/responses.py
+-rw-r--r--   0        0        0      360 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/clients/ios/types.py
+-rw-r--r--   0        0        0      666 2024-03-24 15:57:53.263177 youtubei-0.1.2/youtubei/clients/ios/wrapper.py
+-rw-r--r--   0        0        0      255 2024-02-21 23:27:18.159209 youtubei-0.1.2/youtubei/clients/ios_music/__init__.py
+-rw-r--r--   0        0        0      547 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/clients/ios_music/constants.py
+-rw-r--r--   0        0        0      275 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/clients/ios_music/parser.py
+-rw-r--r--   0        0        0      859 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/clients/ios_music/responses.py
+-rw-r--r--   0        0        0      720 2024-03-24 15:57:53.263177 youtubei-0.1.2/youtubei/clients/ios_music/wrapper.py
+-rw-r--r--   0        0        0      206 2024-02-21 23:27:18.159209 youtubei-0.1.2/youtubei/clients/web/__init__.py
+-rw-r--r--   0        0        0      458 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/clients/web/constants.py
+-rw-r--r--   0        0        0      382 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/clients/web/parser.py
+-rw-r--r--   0        0        0     2033 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/clients/web/responses.py
+-rw-r--r--   0        0        0      919 2024-03-24 15:57:53.263177 youtubei-0.1.2/youtubei/clients/web/wrapper.py
+-rw-r--r--   0        0        0      255 2024-02-21 23:27:18.159209 youtubei-0.1.2/youtubei/clients/web_remix/__init__.py
+-rw-r--r--   0        0        0      557 2024-05-27 14:21:01.405315 youtubei-0.1.2/youtubei/clients/web_remix/constants.py
+-rw-r--r--   0        0        0     2486 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/clients/web_remix/models.py
+-rw-r--r--   0        0        0     1043 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/clients/web_remix/parser.py
+-rw-r--r--   0        0        0     1653 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/clients/web_remix/responses.py
+-rw-r--r--   0        0        0      385 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/clients/web_remix/types.py
+-rw-r--r--   0        0        0     2187 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/clients/web_remix/wrapper.py
+-rw-r--r--   0        0        0       84 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/enums/__init__.py
+-rw-r--r--   0        0        0      130 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/enums/_base.py
+-rw-r--r--   0        0        0      732 2024-03-24 15:33:03.141373 youtubei-0.1.2/youtubei/enums/action.py
+-rw-r--r--   0        0        0    42633 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/enums/icon.py
+-rw-r--r--   0        0        0     2166 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/enums/music.py
+-rw-r--r--   0        0        0    15181 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/enums/other.py
+-rw-r--r--   0        0        0      482 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/__init__.py
+-rw-r--r--   0        0        0      204 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/_base.py
+-rw-r--r--   0        0        0      366 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/accessibility.py
+-rw-r--r--   0        0        0     4497 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/actions.py
+-rw-r--r--   0        0        0     1536 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/ad.py
+-rw-r--r--   0        0        0      344 2024-03-24 15:57:53.263177 youtubei-0.1.2/youtubei/models/colour.py
+-rw-r--r--   0        0        0     1046 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/command.py
+-rw-r--r--   0        0        0    11757 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/commands.py
+-rw-r--r--   0        0        0     1395 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/config.py
+-rw-r--r--   0        0        0      345 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/contexts.py
+-rw-r--r--   0        0        0      225 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/data.py
+-rw-r--r--   0        0        0      464 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/data_bound.py
+-rw-r--r--   0        0        0    13622 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/models/endpoints.py
+-rw-r--r--   0        0        0      655 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/logging.py
+-rw-r--r--   0        0        0      663 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/metadata.py
+-rw-r--r--   0        0        0      451 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/models/music.py
+-rw-r--r--   0        0        0     5867 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/models/other.py
+-rw-r--r--   0        0        0      305 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/params.py
+-rw-r--r--   0        0        0      497 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/reminders.py
+-rw-r--r--   0        0        0     1051 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/response.py
+-rw-r--r--   0        0        0     1660 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/text.py
+-rw-r--r--   0        0        0      869 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/models/thumbnail.py
+-rw-r--r--   0        0        0      243 2024-02-21 23:27:18.167209 youtubei-0.1.2/youtubei/parse/__init__.py
+-rw-r--r--   0        0        0      217 2024-02-21 23:27:18.167209 youtubei-0.1.2/youtubei/parse/constants.py
+-rw-r--r--   0        0        0       80 2024-02-21 23:27:18.167209 youtubei-0.1.2/youtubei/parse/exceptions.py
+-rw-r--r--   0        0        0      777 2024-03-24 15:57:53.263177 youtubei-0.1.2/youtubei/parse/parser.py
+-rw-r--r--   0        0        0      342 2024-02-21 23:27:18.167209 youtubei-0.1.2/youtubei/parse/registry.py
+-rw-r--r--   0        0        0      252 2024-02-21 23:27:18.167209 youtubei-0.1.2/youtubei/parse/types.py
+-rw-r--r--   0        0        0      206 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/parse/utils.py
+-rw-r--r--   0        0        0      241 2024-02-21 23:27:18.167209 youtubei-0.1.2/youtubei/parse/validated_types.py
+-rw-r--r--   0        0        0      845 2024-02-21 23:27:18.167209 youtubei-0.1.2/youtubei/parse/validators.py
+-rw-r--r--   0        0        0      553 2024-03-24 15:37:35.348062 youtubei-0.1.2/youtubei/parser.py
+-rw-r--r--   0        0        0        0 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/py.typed
+-rw-r--r--   0        0        0     6170 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/renderers/__init__.py
+-rw-r--r--   0        0        0      177 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/_base.py
+-rw-r--r--   0        0        0      193 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/about_this_ad.py
+-rw-r--r--   0        0        0      174 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/ad_break_service.py
+-rw-r--r--   0        0        0      229 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/ad_duration_remaining.py
+-rw-r--r--   0        0        0      320 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/ad_hover_text_button.py
+-rw-r--r--   0        0        0      425 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/ad_placement.py
+-rw-r--r--   0        0        0      504 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/ad_preview.py
+-rw-r--r--   0        0        0      432 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/ad_slot.py
+-rw-r--r--   0        0        0      226 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/audio_only_playability.py
+-rw-r--r--   0        0        0      618 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/background_promo.py
+-rw-r--r--   0        0        0     1132 2024-03-24 15:57:53.263177 youtubei-0.1.2/youtubei/renderers/button.py
+-rw-r--r--   0        0        0      306 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/card.py
+-rw-r--r--   0        0        0      493 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/card_collection.py
+-rw-r--r--   0        0        0      445 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/checkbox.py
+-rw-r--r--   0        0        0      434 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/renderers/chip_cloud.py
+-rw-r--r--   0        0        0      702 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/renderers/chip_cloud_chip.py
+-rw-r--r--   0        0        0      465 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/cinematic_container.py
+-rw-r--r--   0        0        0      136 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/client_forecasting_ad.py
+-rw-r--r--   0        0        0      491 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/compact_link.py
+-rw-r--r--   0        0        0      571 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/confirm_dialog.py
+-rw-r--r--   0        0        0      274 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/cropped_square_thumbnail.py
+-rw-r--r--   0        0        0     1024 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/desktop_topbar.py
+-rw-r--r--   0        0        0      280 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/endscreen.py
+-rw-r--r--   0        0        0      812 2024-03-24 15:57:53.263177 youtubei-0.1.2/youtubei/renderers/endscreen_element.py
+-rw-r--r--   0        0        0      538 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/engagement_panel_section_list.py
+-rw-r--r--   0        0        0      278 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/engagement_panel_title_header.py
+-rw-r--r--   0        0        0      710 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/fusion_searchbox.py
+-rw-r--r--   0        0        0      816 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/guide_entry.py
+-rw-r--r--   0        0        0      480 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/guide_section.py
+-rw-r--r--   0        0        0      441 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/guide_signin_promo.py
+-rw-r--r--   0        0        0      655 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/hero_playlist_thumbnail.py
+-rw-r--r--   0        0        0      561 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/hotkey_dialog.py
+-rw-r--r--   0        0        0      505 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/hotkey_dialog_section.py
+-rw-r--r--   0        0        0      432 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/hotkey_dialog_section_option.py
+-rw-r--r--   0        0        0      122 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/info_card_icon.py
+-rw-r--r--   0        0        0      772 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/instream_ad_player_overlay.py
+-rw-r--r--   0        0        0     1102 2024-03-24 15:57:53.263177 youtubei-0.1.2/youtubei/renderers/instream_video_ad.py
+-rw-r--r--   0        0        0      346 2024-03-24 15:33:03.145373 youtubei-0.1.2/youtubei/renderers/item_section.py
+-rw-r--r--   0        0        0      567 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/like_button.py
+-rw-r--r--   0        0        0      277 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/linear_ad_sequence.py
+-rw-r--r--   0        0        0      278 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/lugash_footer.py
+-rw-r--r--   0        0        0     1414 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/renderers/menu.py
+-rw-r--r--   0        0        0      667 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/menu_navigation_item.py
+-rw-r--r--   0        0        0      601 2024-03-24 15:57:53.263177 youtubei-0.1.2/youtubei/renderers/menu_service_item.py
+-rw-r--r--   0        0        0      313 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/metadata_badge.py
+-rw-r--r--   0        0        0     1774 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/microformat_data.py
+-rw-r--r--   0        0        0      182 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/miniplayer.py
+-rw-r--r--   0        0        0      899 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/mobile_topbar.py
+-rw-r--r--   0        0        0      504 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/modal_with_title_and_button.py
+-rw-r--r--   0        0        0      764 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/multi_page_menu.py
+-rw-r--r--   0        0        0      649 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/multi_page_menu_section.py
+-rw-r--r--   0        0        0     1182 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/renderers/music_card_shelf.py
+-rw-r--r--   0        0        0      272 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/renderers/music_card_shelf_header_basic.py
+-rw-r--r--   0        0        0      199 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/music_carousel_shelf.py
+-rw-r--r--   0        0        0      591 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/music_data_bound_menu.py
+-rw-r--r--   0        0        0      778 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/music_detail_header.py
+-rw-r--r--   0        0        0      334 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/renderers/music_inline_badge.py
+-rw-r--r--   0        0        0      743 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/music_item_thumbnail_overlay.py
+-rw-r--r--   0        0        0     1022 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/renderers/music_play_button.py
+-rw-r--r--   0        0        0      549 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/music_playlist_shelf.py
+-rw-r--r--   0        0        0     2059 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/renderers/music_responsive_list_item.py
+-rw-r--r--   0        0        0      537 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/music_responsive_list_item_fixed_column.py
+-rw-r--r--   0        0        0      482 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/music_responsive_list_item_flex_column.py
+-rw-r--r--   0        0        0     1048 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/renderers/music_shelf.py
+-rw-r--r--   0        0        0      205 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/music_shelf_divider.py
+-rw-r--r--   0        0        0      411 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/music_thumbnail.py
+-rw-r--r--   0        0        0      278 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/notification_text.py
+-rw-r--r--   0        0        0      424 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/pivot_bar.py
+-rw-r--r--   0        0        0      753 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/pivot_bar_item.py
+-rw-r--r--   0        0        0      281 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/player_annotations_expanded.py
+-rw-r--r--   0        0        0      222 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/player_attestations.py
+-rw-r--r--   0        0        0      629 2024-03-24 15:57:53.263177 youtubei-0.1.2/youtubei/renderers/player_bytes_ad_layout.py
+-rw-r--r--   0        0        0      315 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/player_bytes_sequential_layout.py
+-rw-r--r--   0        0        0      419 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/player_captions_tracklist.py
+-rw-r--r--   0        0        0      310 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/player_error_message.py
+-rw-r--r--   0        0        0      333 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/player_legacy_desktop_watch_ads.py
+-rw-r--r--   0        0        0      765 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/player_microformat.py
+-rw-r--r--   0        0        0      259 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/player_storyboard_spec.py
+-rw-r--r--   0        0        0      268 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/playlist_byline.py
+-rw-r--r--   0        0        0      271 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/playlist_custom_thumbnail.py
+-rw-r--r--   0        0        0     1710 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/playlist_header.py
+-rw-r--r--   0        0        0      261 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/playlist_metadata.py
+-rw-r--r--   0        0        0      435 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/playlist_sidebar.py
+-rw-r--r--   0        0        0     1109 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/playlist_sidebar_primary_info.py
+-rw-r--r--   0        0        0     1232 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/playlist_video.py
+-rw-r--r--   0        0        0      471 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/playlist_video_list.py
+-rw-r--r--   0        0        0      624 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/privacy_tos_footer.py
+-rw-r--r--   0        0        0      355 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/reel_player_overlay.py
+-rw-r--r--   0        0        0     1221 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/renderers/section_list.py
+-rw-r--r--   0        0        0      558 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/simple_ad_badge.py
+-rw-r--r--   0        0        0      345 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/simple_card_teaser.py
+-rw-r--r--   0        0        0      373 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/single_column_browse_results.py
+-rw-r--r--   0        0        0      296 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/skip_ad.py
+-rw-r--r--   0        0        0      184 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/skip_button.py
+-rw-r--r--   0        0        0      770 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/subscribe_button.py
+-rw-r--r--   0        0        0      491 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/renderers/tab.py
+-rw-r--r--   0        0        0      367 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/renderers/tabbed_search_results.py
+-rw-r--r--   0        0        0      319 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/thumbnail_overlay_hover_text.py
+-rw-r--r--   0        0        0      269 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/thumbnail_overlay_now_playing.py
+-rw-r--r--   0        0        0      319 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/thumbnail_overlay_side_panel.py
+-rw-r--r--   0        0        0      357 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/thumbnail_overlay_time_status.py
+-rw-r--r--   0        0        0     1073 2024-03-24 15:33:03.149373 youtubei-0.1.2/youtubei/renderers/toggle_button.py
+-rw-r--r--   0        0        0      676 2024-05-27 15:45:27.493767 youtubei-0.1.2/youtubei/renderers/toggle_menu_service_item.py
+-rw-r--r--   0        0        0      414 2024-03-24 15:33:03.153373 youtubei-0.1.2/youtubei/renderers/topbar_button.py
+-rw-r--r--   0        0        0      580 2024-03-24 15:33:03.153373 youtubei-0.1.2/youtubei/renderers/topbar_logo.py
+-rw-r--r--   0        0        0      921 2024-03-24 15:57:53.263177 youtubei-0.1.2/youtubei/renderers/topbar_menu_button.py
+-rw-r--r--   0        0        0      402 2024-03-24 15:33:03.153373 youtubei-0.1.2/youtubei/renderers/two_column_browse_results.py
+-rw-r--r--   0        0        0      215 2024-03-24 15:33:03.153373 youtubei-0.1.2/youtubei/renderers/unified_share_panel.py
+-rw-r--r--   0        0        0      477 2024-03-24 15:33:03.153373 youtubei-0.1.2/youtubei/renderers/upload_progress_arrow.py
+-rw-r--r--   0        0        0      527 2024-03-24 15:33:03.153373 youtubei-0.1.2/youtubei/renderers/watch_break.py
+-rw-r--r--   0        0        0      216 2024-03-24 15:33:03.153373 youtubei-0.1.2/youtubei/types.py
+-rw-r--r--   0        0        0      342 2024-03-24 14:12:43.309436 youtubei-0.1.2/youtubei/validated_types.py
+-rw-r--r--   0        0        0     1075 2024-03-24 15:33:03.153373 youtubei-0.1.2/youtubei/validators.py
+-rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 youtubei-0.1.2/PKG-INFO
```

### Comparing `youtubei-0.1.1/LICENSE` & `youtubei-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/pyproject.toml` & `youtubei-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "youtubei"
-version = "0.1.1"
+version = "0.1.2"
 description = "InnerTube Parsing Library"
 authors = ["Tom Bulled <26026015+tombulled@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-innertube = "^2.1.13"
+innertube = "^2.1.16"
 pyhumps = "^3.8.0"
 pydantic = "^2.5.3"
 typing-extensions = "^4.9.0"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^3.0.3"
 mypy = "^1.8.0"
```

### Comparing `youtubei-0.1.1/youtubei/clients/android/constants.py` & `youtubei-0.1.2/youtubei/clients/android/constants.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/clients/android/responses.py` & `youtubei-0.1.2/youtubei/clients/android/responses.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/clients/android/wrapper.py` & `youtubei-0.1.2/youtubei/clients/android/wrapper.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/clients/ios/responses.py` & `youtubei-0.1.2/youtubei/clients/ios/responses.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/clients/ios/wrapper.py` & `youtubei-0.1.2/youtubei/clients/ios/wrapper.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/clients/ios_music/constants.py` & `youtubei-0.1.2/youtubei/clients/ios_music/constants.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/clients/ios_music/responses.py` & `youtubei-0.1.2/youtubei/clients/ios_music/responses.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/clients/ios_music/wrapper.py` & `youtubei-0.1.2/youtubei/clients/ios_music/wrapper.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/clients/web/responses.py` & `youtubei-0.1.2/youtubei/clients/web/responses.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/clients/web/wrapper.py` & `youtubei-0.1.2/youtubei/clients/web/wrapper.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/clients/web_remix/constants.py` & `youtubei-0.1.2/youtubei/clients/web_remix/constants.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/clients/web_remix/models.py` & `youtubei-0.1.2/youtubei/clients/web_remix/models.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/clients/web_remix/parser.py` & `youtubei-0.1.2/youtubei/clients/web_remix/parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from youtubei.parser import ClientParser
 
 from .responses import (
     WebRemixConfigResponse,
     WebRemixGetBrowseAlbumDetailPageResponse,
     WebRemixGetBrowsePlaylistDetailPageResponse,
     WebRemixGuideResponse,
+    WebRemixGetSearchResponse,
 )
 
 __all__ = ("WebRemixParser",)
 
 
 class WebRemixParser(ClientParser):
     def browse_album(self, response, /) -> WebRemixGetBrowseAlbumDetailPageResponse:
@@ -20,7 +21,10 @@
         return self._parse(response, WebRemixGetBrowsePlaylistDetailPageResponse)
 
     def config(self, response, /) -> WebRemixConfigResponse:
         return self._parse(response, WebRemixConfigResponse)
 
     def guide(self, response, /) -> WebRemixGuideResponse:
         return self._parse(response, WebRemixGuideResponse)
+
+    def search(self, response, /) -> WebRemixGetSearchResponse:
+        return self._parse(response, WebRemixGetSearchResponse)
```

### Comparing `youtubei-0.1.1/youtubei/clients/web_remix/responses.py` & `youtubei-0.1.2/youtubei/clients/web_remix/responses.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from youtubei.clients.web_remix.models import GlobalConfigGroup
 from youtubei.models.response import Response, ResponseContext
 from youtubei.parse.validated_types import Dynamic
 from youtubei.renderers import (
     MicroformatDataRenderer,
     MusicDetailHeaderRenderer,
     SingleColumnBrowseResultsRenderer,
+    TabbedSearchResultsRenderer,
 )
-
 from .types import GuideItem
 
 __all__ = (
     "WebRemixResponseContext",
     "WebRemixResponse",
     "WebRemixConfigResponse",
     "WebRemixGuideResponse",
@@ -44,7 +44,11 @@
     header: Dynamic[MusicDetailHeaderRenderer]
     microformat: Optional[Dynamic[MicroformatDataRenderer]] = None
 
 
 class WebRemixGetBrowsePlaylistDetailPageResponse(WebRemixResponse):
     contents: Dynamic[SingleColumnBrowseResultsRenderer]
     header: Optional[Dynamic[MusicDetailHeaderRenderer]] = None
+
+
+class WebRemixGetSearchResponse(WebRemixResponse):
+    contents: Dynamic[TabbedSearchResultsRenderer]
```

### Comparing `youtubei-0.1.1/youtubei/clients/web_remix/wrapper.py` & `youtubei-0.1.2/youtubei/clients/web_remix/wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from dataclasses import dataclass, field
+from typing import Optional
 
-from innertube import InnerTube
+from innertube import InnerTube, utils
+from innertube.enums import Endpoint
 
 from .constants import WEB_REMIX_CLIENT, WEB_REMIX_PARSER
 from .parser import WebRemixParser
 from .responses import (
     WebRemixConfigResponse,
     WebRemixGetBrowseAlbumDetailPageResponse,
     WebRemixGetBrowsePlaylistDetailPageResponse,
@@ -49,7 +51,27 @@
 
         return self.parser.config(response)
 
     def guide(self) -> WebRemixGuideResponse:
         response: dict = self.client.adaptor.dispatch("guide")
 
         return self.parser.guide(response)
+
+    def search(
+        self,
+        query: Optional[str] = None,
+        *,
+        params: Optional[str] = None,
+        continuation: Optional[str] = None,
+    ):
+        response: dict = self.client.adaptor.dispatch(
+            Endpoint.SEARCH,
+            body=utils.filter(
+                dict(
+                    query=query or "",
+                    params=params,
+                    continuation=continuation,
+                )
+            ),
+        )
+
+        return self.parser.search(response)
```

### Comparing `youtubei-0.1.1/youtubei/enums/action.py` & `youtubei-0.1.2/youtubei/enums/action.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/enums/icon.py` & `youtubei-0.1.2/youtubei/enums/icon.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/enums/music.py` & `youtubei-0.1.2/youtubei/enums/music.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     "MusicItemThumbnailOverlayContentPosition",
     "MusicItemThumbnailOverlayDisplayStyle",
     "MusicPlayButtonRippleTarget",
     "MusicPlayButtonSize",
     "MusicResponsiveListItemColumnDisplayPriority",
     "MusicResponsiveListItemFixedColumnSize",
     "MusicResponsiveListItemHeight",
+    "MusicResponsiveListItemFlexColumnDisplayStyle",
     "MusicThumbnailCrop",
     "MusicThumbnailScale",
     "MusicVideoType",
 )
 
 
 class MusicItemThumbnailOverlayContentPosition(StrEnum):
@@ -37,21 +38,32 @@
 
 class MusicResponsiveListItemFixedColumnSize(StrEnum):
     SMALL: str = "MUSIC_RESPONSIVE_LIST_ITEM_FIXED_COLUMN_SIZE_SMALL"
 
 
 class MusicResponsiveListItemHeight(StrEnum):
     MEDIUM: str = "MUSIC_RESPONSIVE_LIST_ITEM_HEIGHT_MEDIUM"
+    TALL: str = "MUSIC_RESPONSIVE_LIST_ITEM_HEIGHT_TALL"
+
+
+class MusicResponsiveListItemFlexColumnDisplayStyle(StrEnum):
+    TWO_LINE_STACK: str = (
+        "MUSIC_RESPONSIVE_LIST_ITEM_FLEX_COLUMN_DISPLAY_STYLE_TWO_LINE_STACK"
+    )
 
 
 class MusicThumbnailCrop(StrEnum):
     UNSPECIFIED: str = "MUSIC_THUMBNAIL_CROP_UNSPECIFIED"
+    CIRCLE: str = "MUSIC_THUMBNAIL_CROP_CIRCLE"
 
 
 class MusicThumbnailScale(StrEnum):
     ASPECT_FIT: str = "MUSIC_THUMBNAIL_SCALE_ASPECT_FIT"
+    ASPECT_FILL: str = "MUSIC_THUMBNAIL_SCALE_ASPECT_FILL"
     UNSPECIFIED: str = "MUSIC_THUMBNAIL_SCALE_UNSPECIFIED"
 
 
 class MusicVideoType(StrEnum):
     ATV: str = "MUSIC_VIDEO_TYPE_ATV"
     OMV: str = "MUSIC_VIDEO_TYPE_OMV"
+    UGC: str = "MUSIC_VIDEO_TYPE_UGC"
+    PODCAST_EPISODE: str = "MUSIC_VIDEO_TYPE_PODCAST_EPISODE"
```

### Comparing `youtubei-0.1.1/youtubei/enums/other.py` & `youtubei-0.1.2/youtubei/enums/other.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,14 +493,18 @@
     REPORT_CHANNEL = "MULTI_PAGE_MENU_STYLE_TYPE_REPORT_CHANNEL"
 
 
 class MusicPageType(StrEnum):
     METRONOME = "MUSIC_PAGE_TYPE_METRONOME"
     ALBUM = "MUSIC_PAGE_TYPE_ALBUM"
     ARTIST = "MUSIC_PAGE_TYPE_ARTIST"
+    USER_CHANNEL = "MUSIC_PAGE_TYPE_USER_CHANNEL"
+    PODCAST_SHOW_DETAIL_PAGE = "MUSIC_PAGE_TYPE_PODCAST_SHOW_DETAIL_PAGE"
+    NON_MUSIC_AUDIO_TRACK_PAGE = "MUSIC_PAGE_TYPE_NON_MUSIC_AUDIO_TRACK_PAGE"
+    PLAYLIST = "MUSIC_PAGE_TYPE_PLAYLIST"
 
 
 class PlaybackMode(StrEnum):
     ALLOW = "PLAYBACK_MODE_ALLOW"
 
 
 class PlaylistEditListType(StrEnum):
@@ -594,14 +598,16 @@
     UNKNOWN: str = "STYLE_UNKNOWN"
     MONO_FILLED: str = "STYLE_MONO_FILLED"
     MONO_TONAL: str = "STYLE_MONO_TONAL"
     BRAND: str = "STYLE_BRAND"
     MONO_TONAL_OVERLAY: str = "STYLE_MONO_TONAL_OVERLAY"
     MONO_FILLED_OVERLAY: str = "STYLE_MONO_FILLED_OVERLAY"
     DARK_ON_WHITE: str = "STYLE_DARK_ON_WHITE"
+    WHITE_TRANSLUCENT: str = "STYLE_WHITE_TRANSLUCENT"
+    SECONDARY: str = "STYLE_SECONDARY"
 
 
 class Target(StrEnum):
     NEW_WINDOW: str = "TARGET_NEW_WINDOW"
 
 
 class TargetId(StrEnum):
```

### Comparing `youtubei-0.1.1/youtubei/models/actions.py` & `youtubei-0.1.2/youtubei/models/actions.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/models/ad.py` & `youtubei-0.1.2/youtubei/models/ad.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/models/command.py` & `youtubei-0.1.2/youtubei/models/command.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/models/commands.py` & `youtubei-0.1.2/youtubei/models/commands.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/models/config.py` & `youtubei-0.1.2/youtubei/models/config.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/models/endpoints.py` & `youtubei-0.1.2/youtubei/models/endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,23 @@
     QueueInsertPosition,
     ReelWatchInputType,
     ReelWatchSequenceProvider,
     SharePanelType,
     Signal,
     Target,
 )
+from youtubei.enums.other import LikeStatus
 from youtubei.models.actions import AddToToastAction
 from youtubei.models.config import (
     BrowseEndpointContextMusicConfig,
     Html5PlaybackOnesieConfig,
     WatchEndpointMusicConfig,
 )
 from youtubei.models.contexts import LoggingContext
-from youtubei.models.other import PlaylistEditAction, QueueTarget
+from youtubei.models.other import LikeTarget, PlaylistEditAction, QueueTarget
 from youtubei.models.params import SkAdParameters
 from youtubei.parse.validated_types import Dynamic
 from youtubei.types import BrowseId
 from youtubei.validated_types import DynamicCommand
 
 from ._base import BaseModel
 
@@ -338,16 +339,18 @@
 
 @IOS_REGISTRY
 class IosApplicationEndpoint(BaseModel):
     external_app_url: str
     fallback_endpoint: DynamicCommand[Any]  # Observed: AppStoreEndpoint
 
 
+@WEB_REMIX_REGISTRY
 class LikeEndpoint(BaseEndpoint):
-    pass
+    status: LikeStatus
+    target: LikeTarget
 
 
 class LiveChatActionEndpoint(BaseEndpoint):
     pass
 
 
 class LiveChatEndpoint(BaseEndpoint):
@@ -447,19 +450,21 @@
     pass
 
 
 class ScrollToSectionEndpoint(BaseEndpoint):
     pass
 
 
+@WEB_REMIX_REGISTRY
 @WEB_REGISTRY
 @ANDROID_REGISTRY
 @IOS_REGISTRY
 class SearchEndpoint(BaseEndpoint):
     query: str
+    params: Optional[str] = None
 
 
 class SelectActiveIdentityEndpoint(BaseEndpoint):
     pass
 
 
 class SendLiveChatMessageEndpoint(BaseEndpoint):
```

### Comparing `youtubei-0.1.1/youtubei/models/logging.py` & `youtubei-0.1.2/youtubei/models/logging.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/models/metadata.py` & `youtubei-0.1.2/youtubei/models/metadata.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/models/other.py` & `youtubei-0.1.2/youtubei/models/other.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     "ShareData",
     "SodarExtensionData",
     "Style",
     "Size",
     "TranslationLanguage",
     "VideoDetails",
     "QueueTarget",
+    "LikeTarget",
     "LikeButtonTarget",
 )
 
 
 class ActiveViewTracking(BaseModel):
     traffic_type: ActiveViewTrafficType
 
@@ -252,9 +253,13 @@
 
 class QueueTarget(BaseModel):
     video_id: Optional[str] = None
     playlist_id: Optional[str] = None
     on_empty_queue: DynamicCommand[Any]  # Observed: WatchEndpoint
 
 
+class LikeTarget(BaseModel):
+    playlist_id: str
+
+
 class LikeButtonTarget(BaseModel):
     video_id: str
```

### Comparing `youtubei-0.1.1/youtubei/models/response.py` & `youtubei-0.1.2/youtubei/models/response.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/models/text.py` & `youtubei-0.1.2/youtubei/models/text.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/models/thumbnail.py` & `youtubei-0.1.2/youtubei/models/thumbnail.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/parse/parser.py` & `youtubei-0.1.2/youtubei/parse/parser.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/parse/validators.py` & `youtubei-0.1.2/youtubei/parse/validators.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/parser.py` & `youtubei-0.1.2/youtubei/parser.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/__init__.py` & `youtubei-0.1.2/youtubei/renderers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from .ad_preview import AdPreviewRenderer
 from .ad_slot import AdSlotRenderer
 from .audio_only_playability import AudioOnlyPlayabilityRenderer
 from .background_promo import BackgroundPromoRenderer
 from .button import ButtonRenderer
 from .card import CardRenderer
 from .card_collection import CardCollectionRenderer
+from .checkbox import CheckboxRenderer
+from .chip_cloud import ChipCloudRenderer
+from .chip_cloud_chip import ChipCloudChipRenderer
 from .cinematic_container import CinematicContainerRenderer
 from .client_forecasting_ad import ClientForecastingAdRenderer
 from .compact_link import CompactLinkRenderer
 from .confirm_dialog import ConfirmDialogRenderer
 from .cropped_square_thumbnail import CroppedSquareThumbnailRenderer
 from .desktop_topbar import DesktopTopbarRenderer
 from .endscreen import EndscreenRenderer
@@ -41,17 +44,20 @@
 from .metadata_badge import MetadataBadgeRenderer
 from .microformat_data import MicroformatDataRenderer
 from .miniplayer import MiniplayerRenderer
 from .mobile_topbar import MobileTopbarRenderer
 from .modal_with_title_and_button import ModalWithTitleAndButtonRenderer
 from .multi_page_menu import MultiPageMenuRenderer
 from .multi_page_menu_section import MultiPageMenuSectionRenderer
+from .music_card_shelf import MusicCardShelfRenderer
+from .music_card_shelf_header_basic import MusicCardShelfHeaderBasicRenderer
 from .music_carousel_shelf import MusicCarouselShelfRenderer
 from .music_data_bound_menu import MusicDataBoundMenuRenderer
 from .music_detail_header import MusicDetailHeaderRenderer
+from .music_inline_badge import MusicInlineBadgeRenderer
 from .music_item_thumbnail_overlay import MusicItemThumbnailOverlayRenderer
 from .music_play_button import MusicPlayButtonRenderer
 from .music_playlist_shelf import MusicPlaylistShelfRenderer
 from .music_responsive_list_item import MusicResponsiveListItemRenderer
 from .music_responsive_list_item_flex_column import (
     MusicResponsiveListItemFlexColumnRenderer,
 )
@@ -84,19 +90,21 @@
 from .simple_ad_badge import SimpleAdBadgeRenderer
 from .simple_card_teaser import SimpleCardTeaserRenderer
 from .single_column_browse_results import SingleColumnBrowseResultsRenderer
 from .skip_ad import SkipAdRenderer
 from .skip_button import SkipButtonRenderer
 from .subscribe_button import SubscribeButtonRenderer
 from .tab import TabRenderer
+from .tabbed_search_results import TabbedSearchResultsRenderer
 from .thumbnail_overlay_hover_text import ThumbnailOverlayHoverTextRenderer
 from .thumbnail_overlay_now_playing import ThumbnailOverlayNowPlayingRenderer
 from .thumbnail_overlay_side_panel import ThumbnailOverlaySidePanelRenderer
 from .thumbnail_overlay_time_status import ThumbnailOverlayTimeStatusRenderer
 from .toggle_button import ToggleButtonRenderer
+from .toggle_menu_service_item import ToggleMenuServiceItemRenderer
 from .topbar_button import TopbarButtonRenderer
 from .topbar_logo import TopbarLogoRenderer
 from .topbar_menu_button import TopbarMenuButtonRenderer
 from .two_column_browse_results import TwoColumnBrowseResultsRenderer
 from .unified_share_panel import UnifiedSharePanelRenderer
 from .upload_progress_arrow import UploadProgressArrowRenderer
 from .watch_break import WatchBreakRenderer
```

### Comparing `youtubei-0.1.1/youtubei/renderers/background_promo.py` & `youtubei-0.1.2/youtubei/renderers/background_promo.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/button.py` & `youtubei-0.1.2/youtubei/renderers/button.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/confirm_dialog.py` & `youtubei-0.1.2/youtubei/renderers/confirm_dialog.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/desktop_topbar.py` & `youtubei-0.1.2/youtubei/renderers/desktop_topbar.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/endscreen_element.py` & `youtubei-0.1.2/youtubei/renderers/endscreen_element.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/engagement_panel_section_list.py` & `youtubei-0.1.2/youtubei/renderers/engagement_panel_section_list.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/fusion_searchbox.py` & `youtubei-0.1.2/youtubei/renderers/fusion_searchbox.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/guide_entry.py` & `youtubei-0.1.2/youtubei/renderers/guide_entry.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/hero_playlist_thumbnail.py` & `youtubei-0.1.2/youtubei/renderers/hero_playlist_thumbnail.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/hotkey_dialog.py` & `youtubei-0.1.2/youtubei/renderers/hotkey_dialog.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/instream_ad_player_overlay.py` & `youtubei-0.1.2/youtubei/renderers/instream_ad_player_overlay.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/instream_video_ad.py` & `youtubei-0.1.2/youtubei/renderers/instream_video_ad.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/like_button.py` & `youtubei-0.1.2/youtubei/renderers/like_button.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/menu.py` & `youtubei-0.1.2/youtubei/renderers/menu.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,25 +4,34 @@
 from youtubei.models.accessibility import Accessibility
 from youtubei.parse.validated_types import Dynamic
 from youtubei.renderers.button import ButtonRenderer
 from youtubei.renderers.like_button import LikeButtonRenderer
 from youtubei.renderers.menu_navigation_item import MenuNavigationItemRenderer
 from youtubei.renderers.menu_service_item import MenuServiceItemRenderer
 from youtubei.renderers.toggle_button import ToggleButtonRenderer
+from youtubei.renderers.toggle_menu_service_item import ToggleMenuServiceItemRenderer
 
 from ._base import BaseRenderer
 
 __all__ = ("MenuRenderer",)
 
 
 @WEB_REGISTRY
 @WEB_REMIX_REGISTRY
 class MenuRenderer(BaseRenderer):
     items: Optional[
-        Sequence[Dynamic[Union[MenuNavigationItemRenderer, MenuServiceItemRenderer]]]
+        Sequence[
+            Dynamic[
+                Union[
+                    MenuNavigationItemRenderer,
+                    MenuServiceItemRenderer,
+                    ToggleMenuServiceItemRenderer,
+                ]
+            ]
+        ]
     ] = None
     open_immediately: Optional[bool] = None
     top_level_buttons: Optional[
         Sequence[
             Dynamic[
                 Union[
                     ToggleButtonRenderer,
```

### Comparing `youtubei-0.1.1/youtubei/renderers/menu_navigation_item.py` & `youtubei-0.1.2/youtubei/renderers/menu_navigation_item.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/menu_service_item.py` & `youtubei-0.1.2/youtubei/renderers/menu_service_item.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/microformat_data.py` & `youtubei-0.1.2/youtubei/renderers/microformat_data.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/mobile_topbar.py` & `youtubei-0.1.2/youtubei/renderers/mobile_topbar.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/multi_page_menu.py` & `youtubei-0.1.2/youtubei/renderers/multi_page_menu.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/multi_page_menu_section.py` & `youtubei-0.1.2/youtubei/renderers/multi_page_menu_section.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/music_data_bound_menu.py` & `youtubei-0.1.2/youtubei/renderers/music_data_bound_menu.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/music_detail_header.py` & `youtubei-0.1.2/youtubei/renderers/music_detail_header.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/music_item_thumbnail_overlay.py` & `youtubei-0.1.2/youtubei/renderers/music_item_thumbnail_overlay.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/music_play_button.py` & `youtubei-0.1.2/youtubei/renderers/music_play_button.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+from typing import Union
 from youtubei.enums.music import MusicPlayButtonRippleTarget, MusicPlayButtonSize
 from youtubei.models.accessibility import Accessibility
-from youtubei.models.endpoints import WatchEndpoint
+from youtubei.models.endpoints import WatchEndpoint, WatchPlaylistEndpoint
 from youtubei.models.other import Icon
 from youtubei.validated_types import DynamicCommand
 
 from .._registries import WEB_REMIX_REGISTRY
 from ._base import BaseRenderer
 
 __all__ = ("MusicPlayButtonRenderer",)
 
 
 @WEB_REMIX_REGISTRY
 class MusicPlayButtonRenderer(BaseRenderer):
-    play_navigation_endpoint: DynamicCommand[WatchEndpoint]
+    play_navigation_endpoint: DynamicCommand[
+        Union[WatchEndpoint, WatchPlaylistEndpoint]
+    ]
     play_icon: Icon
     pause_icon: Icon
     icon_color: int
     background_color: int
     active_background_color: int
     loading_indicator_color: int
     playing_icon: Icon
```

### Comparing `youtubei-0.1.1/youtubei/renderers/music_playlist_shelf.py` & `youtubei-0.1.2/youtubei/renderers/music_playlist_shelf.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/music_responsive_list_item.py` & `youtubei-0.1.2/youtubei/renderers/music_responsive_list_item.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 from typing import Optional, Sequence
 
-from youtubei.enums.music import MusicResponsiveListItemHeight
+from youtubei.enums.music import (
+    MusicResponsiveListItemFlexColumnDisplayStyle,
+    MusicResponsiveListItemHeight,
+)
+from youtubei.models.endpoints import BrowseEndpoint
 from youtubei.models.music import PlaylistItemData
 from youtubei.models.text import ComplexText
 from youtubei.parse.validated_types import Dynamic
 from youtubei.renderers.checkbox import CheckboxRenderer
 from youtubei.renderers.menu import MenuRenderer
+from youtubei.renderers.music_inline_badge import MusicInlineBadgeRenderer
 from youtubei.renderers.music_item_thumbnail_overlay import (
     MusicItemThumbnailOverlayRenderer,
 )
 from youtubei.renderers.music_responsive_list_item_fixed_column import (
     MusicResponsiveListItemFixedColumnRenderer,
 )
 from youtubei.renderers.music_responsive_list_item_flex_column import (
     MusicResponsiveListItemFlexColumnRenderer,
 )
 from youtubei.renderers.music_thumbnail import MusicThumbnailRenderer
+from youtubei.validated_types import DynamicCommand
 
 from .._registries import WEB_REMIX_REGISTRY
 from ._base import BaseRenderer
 
 __all__ = ("MusicResponsiveListItemRenderer",)
 
 
 @WEB_REMIX_REGISTRY
 class MusicResponsiveListItemRenderer(BaseRenderer):
     thumbnail: Optional[Dynamic[MusicThumbnailRenderer]] = None
-    overlay: Dynamic[MusicItemThumbnailOverlayRenderer]
+    overlay: Optional[Dynamic[MusicItemThumbnailOverlayRenderer]] = None
     flex_columns: Sequence[Dynamic[MusicResponsiveListItemFlexColumnRenderer]]
-    fixed_columns: Sequence[Dynamic[MusicResponsiveListItemFixedColumnRenderer]]
+    fixed_columns: Optional[
+        Sequence[Dynamic[MusicResponsiveListItemFixedColumnRenderer]]
+    ] = None
     menu: Dynamic[MenuRenderer]
-    playlist_item_data: PlaylistItemData
+    playlist_item_data: Optional[PlaylistItemData] = None
     item_height: Optional[MusicResponsiveListItemHeight] = None
     index: Optional[ComplexText] = None
-    multi_select_checkbox: Dynamic[CheckboxRenderer]
+    multi_select_checkbox: Optional[Dynamic[CheckboxRenderer]] = None
+    navigation_endpoint: Optional[DynamicCommand[BrowseEndpoint]] = None
+    flex_column_display_style: Optional[
+        MusicResponsiveListItemFlexColumnDisplayStyle
+    ] = None
+    badges: Optional[Sequence[Dynamic[MusicInlineBadgeRenderer]]] = None
```

### Comparing `youtubei-0.1.1/youtubei/renderers/music_responsive_list_item_fixed_column.py` & `youtubei-0.1.2/youtubei/renderers/music_responsive_list_item_fixed_column.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/pivot_bar_item.py` & `youtubei-0.1.2/youtubei/renderers/pivot_bar_item.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/player_bytes_ad_layout.py` & `youtubei-0.1.2/youtubei/renderers/player_bytes_ad_layout.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/player_microformat.py` & `youtubei-0.1.2/youtubei/renderers/player_microformat.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/playlist_header.py` & `youtubei-0.1.2/youtubei/renderers/playlist_header.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/playlist_sidebar_primary_info.py` & `youtubei-0.1.2/youtubei/renderers/playlist_sidebar_primary_info.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/playlist_video.py` & `youtubei-0.1.2/youtubei/renderers/playlist_video.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/privacy_tos_footer.py` & `youtubei-0.1.2/youtubei/renderers/privacy_tos_footer.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/section_list.py` & `youtubei-0.1.2/youtubei/renderers/topbar_menu_button.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from typing import Optional, Sequence, Union
+from typing import Any, Optional
 
-from youtubei._registries import ANDROID_REGISTRY, WEB_REGISTRY, WEB_REMIX_REGISTRY
-from youtubei.models.data import NextContinuationData
+from youtubei._registries import ANDROID_REGISTRY, IOS_REGISTRY, WEB_REGISTRY
+from youtubei.enums import Style, TargetId
+from youtubei.models.accessibility import Accessibility
+from youtubei.models.other import Icon
 from youtubei.parse import Dynamic
-from youtubei.renderers.item_section import ItemSectionRenderer
-from youtubei.renderers.music_carousel_shelf import MusicCarouselShelfRenderer
-from youtubei.renderers.music_playlist_shelf import MusicPlaylistShelfRenderer
-from youtubei.renderers.music_shelf import MusicShelfRenderer
+from youtubei.renderers.multi_page_menu import MultiPageMenuRenderer
+from youtubei.validated_types import DynamicCommand
 
 from ._base import BaseRenderer
 
-__all__ = ("SectionListRenderer",)
+__all__ = ("TopbarMenuButtonRenderer",)
 
 
-@WEB_REMIX_REGISTRY
 @WEB_REGISTRY
 @ANDROID_REGISTRY
-class SectionListRenderer(BaseRenderer):
-    contents: Sequence[
-        Dynamic[
-            Union[
-                ItemSectionRenderer,
-                MusicPlaylistShelfRenderer,
-                MusicCarouselShelfRenderer,
-                MusicShelfRenderer,
-            ]
-        ]
-    ]
-    continuations: Optional[Sequence[Dynamic[NextContinuationData]]] = None
+@IOS_REGISTRY
+class TopbarMenuButtonRenderer(BaseRenderer):
+    icon: Icon
+    menu_renderer: Optional[Dynamic[MultiPageMenuRenderer]] = None
+    target_id: Optional[TargetId] = None
+    menu_request: Optional[DynamicCommand[Any]] = (
+        None  # Observed: SignalServiceEndpoint
+    )
+    accessibility: Optional[Accessibility] = None
+    tooltip: Optional[str] = None
+    style: Optional[Style] = None
```

### Comparing `youtubei-0.1.1/youtubei/renderers/simple_ad_badge.py` & `youtubei-0.1.2/youtubei/renderers/simple_ad_badge.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/subscribe_button.py` & `youtubei-0.1.2/youtubei/renderers/subscribe_button.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/toggle_button.py` & `youtubei-0.1.2/youtubei/renderers/toggle_button.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/topbar_logo.py` & `youtubei-0.1.2/youtubei/renderers/topbar_logo.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/renderers/topbar_menu_button.py` & `youtubei-0.1.2/youtubei/renderers/chip_cloud_chip.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-from typing import Any, Optional
+from typing import Optional
 
-from youtubei._registries import ANDROID_REGISTRY, IOS_REGISTRY, WEB_REGISTRY
-from youtubei.enums import Style, TargetId
 from youtubei.models.accessibility import Accessibility
-from youtubei.models.other import Icon
-from youtubei.parse import Dynamic
-from youtubei.renderers.multi_page_menu import MultiPageMenuRenderer
+from youtubei.models.endpoints import SearchEndpoint
+from youtubei.models.other import Icon, Style
+from youtubei.models.text import ComplexText
 from youtubei.validated_types import DynamicCommand
 
+from .._registries import WEB_REMIX_REGISTRY
 from ._base import BaseRenderer
 
-__all__ = ("TopbarMenuButtonRenderer",)
+__all__ = ("ChipCloudChipRenderer",)
 
 
-@WEB_REGISTRY
-@ANDROID_REGISTRY
-@IOS_REGISTRY
-class TopbarMenuButtonRenderer(BaseRenderer):
-    icon: Icon
-    menu_renderer: Optional[Dynamic[MultiPageMenuRenderer]] = None
-    target_id: Optional[TargetId] = None
-    menu_request: Optional[DynamicCommand[Any]] = (
-        None  # Observed: SignalServiceEndpoint
-    )
-    accessibility: Optional[Accessibility] = None
-    tooltip: Optional[str] = None
-    style: Optional[Style] = None
+@WEB_REMIX_REGISTRY
+class ChipCloudChipRenderer(BaseRenderer):
+    style: Style
+    text: Optional[ComplexText] = None
+    icon: Optional[Icon] = None
+    navigation_endpoint: DynamicCommand[SearchEndpoint]
+    accessibility_data: Accessibility
+    is_selected: bool
+    unique_id: Optional[str] = None
```

### Comparing `youtubei-0.1.1/youtubei/renderers/watch_break.py` & `youtubei-0.1.2/youtubei/renderers/watch_break.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/youtubei/validators.py` & `youtubei-0.1.2/youtubei/validators.py`

 * *Files identical despite different names*

### Comparing `youtubei-0.1.1/PKG-INFO` & `youtubei-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: youtubei
-Version: 0.1.1
+Version: 0.1.2
 Summary: InnerTube Parsing Library
 License: MIT
 Author: Tom Bulled
 Author-email: 26026015+tombulled@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: innertube (>=2.1.13,<3.0.0)
+Requires-Dist: innertube (>=2.1.16,<3.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # youtubei
 InnerTube Parsing Library
```

