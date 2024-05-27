# Comparing `tmp/pydivkit-30.1.0.tar.gz` & `tmp/pydivkit-30.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydivkit-30.1.0.tar", max compression
+gzip compressed data, was "pydivkit-30.2.0.tar", max compression
```

## Comparing `pydivkit-30.1.0.tar` & `pydivkit-30.2.0.tar`

### file list

```diff
@@ -1,158 +1,158 @@
--rw-r--r--   0        0        0     9446 2024-05-20 09:17:17.816935 pydivkit-30.1.0/README.md
--rw-r--r--   0        0        0      700 2024-05-20 09:17:17.816935 pydivkit-30.1.0/pydivkit/__init__.py
--rw-r--r--   0        0        0      164 2024-05-20 09:17:17.816935 pydivkit-30.1.0/pydivkit/core/__init__.py
--rw-r--r--   0        0        0      445 2024-05-20 09:17:17.816935 pydivkit-30.1.0/pydivkit/core/compat.py
--rw-r--r--   0        0        0    28631 2024-05-20 09:17:17.816935 pydivkit-30.1.0/pydivkit/core/entities.py
--rw-r--r--   0        0        0     3039 2024-05-20 09:17:17.816935 pydivkit-30.1.0/pydivkit/core/fields.py
--rw-r--r--   0        0        0        0 2024-05-20 09:17:17.816935 pydivkit-30.1.0/pydivkit/core/types/__init__.py
--rw-r--r--   0        0        0      728 2024-05-20 09:17:17.816935 pydivkit-30.1.0/pydivkit/core/types/union.py
--rw-r--r--   0        0        0    16973 2024-05-20 09:18:14.543106 pydivkit-30.1.0/pydivkit/div/__init__.py
--rw-r--r--   0        0        0      611 2024-05-20 09:18:14.016360 pydivkit-30.1.0/pydivkit/div/array_value.py
--rw-r--r--   0        0        0      857 2024-05-20 09:18:14.022334 pydivkit-30.1.0/pydivkit/div/array_variable.py
--rw-r--r--   0        0        0      613 2024-05-20 09:18:14.015573 pydivkit-30.1.0/pydivkit/div/boolean_value.py
--rw-r--r--   0        0        0      861 2024-05-20 09:18:14.022880 pydivkit-30.1.0/pydivkit/div/boolean_variable.py
--rw-r--r--   0        0        0      627 2024-05-20 09:18:14.025132 pydivkit-30.1.0/pydivkit/div/color_value.py
--rw-r--r--   0        0        0      875 2024-05-20 09:18:14.017014 pydivkit-30.1.0/pydivkit/div/color_variable.py
--rw-r--r--   0        0        0      603 2024-05-20 09:18:14.010462 pydivkit-30.1.0/pydivkit/div/content_text.py
--rw-r--r--   0        0        0      621 2024-05-20 09:18:14.028986 pydivkit-30.1.0/pydivkit/div/content_url.py
--rw-r--r--   0        0        0      609 2024-05-20 09:18:14.024900 pydivkit-30.1.0/pydivkit/div/dict_value.py
--rw-r--r--   0        0        0      856 2024-05-20 09:18:14.033551 pydivkit-30.1.0/pydivkit/div/dict_variable.py
--rw-r--r--   0        0        0      863 2024-05-20 09:18:14.028798 pydivkit-30.1.0/pydivkit/div/div.py
--rw-r--r--   0        0        0     1209 2024-05-20 09:18:14.032027 pydivkit-30.1.0/pydivkit/div/div_absolute_edge_insets.py
--rw-r--r--   0        0        0     3234 2024-05-20 09:18:14.050317 pydivkit-30.1.0/pydivkit/div/div_accessibility.py
--rw-r--r--   0        0        0     4138 2024-05-20 09:18:14.060274 pydivkit-30.1.0/pydivkit/div/div_action.py
--rw-r--r--   0        0        0     1057 2024-05-20 09:18:14.041695 pydivkit-30.1.0/pydivkit/div/div_action_array_insert_value.py
--rw-r--r--   0        0        0      863 2024-05-20 09:18:14.040687 pydivkit-30.1.0/pydivkit/div/div_action_array_remove_value.py
--rw-r--r--   0        0        0      529 2024-05-20 09:18:14.044917 pydivkit-30.1.0/pydivkit/div/div_action_clear_focus.py
--rw-r--r--   0        0        0      837 2024-05-20 09:18:14.046762 pydivkit-30.1.0/pydivkit/div/div_action_copy_to_clipboard.py
--rw-r--r--   0        0        0      346 2024-05-20 09:18:14.041693 pydivkit-30.1.0/pydivkit/div/div_action_copy_to_clipboard_content.py
--rw-r--r--   0        0        0      732 2024-05-20 09:18:14.047642 pydivkit-30.1.0/pydivkit/div/div_action_focus_element.py
--rw-r--r--   0        0        0      885 2024-05-20 09:18:14.055057 pydivkit-30.1.0/pydivkit/div/div_action_set_variable.py
--rw-r--r--   0        0        0      759 2024-05-20 09:18:14.050720 pydivkit-30.1.0/pydivkit/div/div_action_typed.py
--rw-r--r--   0        0        0      321 2024-05-20 09:18:14.055619 pydivkit-30.1.0/pydivkit/div/div_alignment_horizontal.py
--rw-r--r--   0        0        0      309 2024-05-20 09:18:14.056560 pydivkit-30.1.0/pydivkit/div/div_alignment_vertical.py
--rw-r--r--   0        0        0     3016 2024-05-20 09:18:14.072358 pydivkit-30.1.0/pydivkit/div/div_animation.py
--rw-r--r--   0        0        0      371 2024-05-20 09:18:14.058613 pydivkit-30.1.0/pydivkit/div/div_animation_interpolator.py
--rw-r--r--   0        0        0      879 2024-05-20 09:18:14.063530 pydivkit-30.1.0/pydivkit/div/div_appearance_set_transition.py
--rw-r--r--   0        0        0      557 2024-05-20 09:18:14.062123 pydivkit-30.1.0/pydivkit/div/div_appearance_transition.py
--rw-r--r--   0        0        0      671 2024-05-20 09:18:14.065707 pydivkit-30.1.0/pydivkit/div/div_aspect.py
--rw-r--r--   0        0        0      599 2024-05-20 09:18:14.065776 pydivkit-30.1.0/pydivkit/div/div_background.py
--rw-r--r--   0        0        0     9648 2024-05-20 09:18:14.097307 pydivkit-30.1.0/pydivkit/div/div_base.py
--rw-r--r--   0        0        0      369 2024-05-20 09:18:14.069184 pydivkit-30.1.0/pydivkit/div/div_blend_mode.py
--rw-r--r--   0        0        0      764 2024-05-20 09:18:14.075790 pydivkit-30.1.0/pydivkit/div/div_blur.py
--rw-r--r--   0        0        0     1734 2024-05-20 09:18:14.075606 pydivkit-30.1.0/pydivkit/div/div_border.py
--rw-r--r--   0        0        0     1403 2024-05-20 09:18:14.081618 pydivkit-30.1.0/pydivkit/div/div_change_bounds_transition.py
--rw-r--r--   0        0        0      809 2024-05-20 09:18:14.083598 pydivkit-30.1.0/pydivkit/div/div_change_set_transition.py
--rw-r--r--   0        0        0      420 2024-05-20 09:18:14.079282 pydivkit-30.1.0/pydivkit/div/div_change_transition.py
--rw-r--r--   0        0        0     1176 2024-05-20 09:18:14.090162 pydivkit-30.1.0/pydivkit/div/div_circle_shape.py
--rw-r--r--   0        0        0     2552 2024-05-20 09:18:14.086880 pydivkit-30.1.0/pydivkit/div/div_collection_item_builder.py
--rw-r--r--   0        0        0    18163 2024-05-20 09:18:14.163493 pydivkit-30.1.0/pydivkit/div/div_container.py
--rw-r--r--   0        0        0      432 2024-05-20 09:18:14.090137 pydivkit-30.1.0/pydivkit/div/div_content_alignment_horizontal.py
--rw-r--r--   0        0        0      420 2024-05-20 09:18:14.093239 pydivkit-30.1.0/pydivkit/div/div_content_alignment_vertical.py
--rw-r--r--   0        0        0     1861 2024-05-20 09:18:14.105254 pydivkit-30.1.0/pydivkit/div/div_corners_radius.py
--rw-r--r--   0        0        0      351 2024-05-20 09:18:14.091763 pydivkit-30.1.0/pydivkit/div/div_count.py
--rw-r--r--   0        0        0     1246 2024-05-20 09:18:14.105244 pydivkit-30.1.0/pydivkit/div/div_currency_input_mask.py
--rw-r--r--   0        0        0    10545 2024-05-20 09:18:14.158833 pydivkit-30.1.0/pydivkit/div/div_custom.py
--rw-r--r--   0        0        0     2826 2024-05-20 09:18:14.111704 pydivkit-30.1.0/pydivkit/div/div_data.py
--rw-r--r--   0        0        0      872 2024-05-20 09:18:14.107228 pydivkit-30.1.0/pydivkit/div/div_default_indicator_item_placement.py
--rw-r--r--   0        0        0      802 2024-05-20 09:18:14.106170 pydivkit-30.1.0/pydivkit/div/div_dimension.py
--rw-r--r--   0        0        0     3504 2024-05-20 09:18:14.123464 pydivkit-30.1.0/pydivkit/div/div_disappear_action.py
--rw-r--r--   0        0        0     1177 2024-05-20 09:18:14.117928 pydivkit-30.1.0/pydivkit/div/div_download_callbacks.py
--rw-r--r--   0        0        0      302 2024-05-20 09:18:14.116656 pydivkit-30.1.0/pydivkit/div/div_drawable.py
--rw-r--r--   0        0        0     2081 2024-05-20 09:18:14.124623 pydivkit-30.1.0/pydivkit/div/div_edge_insets.py
--rw-r--r--   0        0        0      804 2024-05-20 09:18:14.124105 pydivkit-30.1.0/pydivkit/div/div_extension.py
--rw-r--r--   0        0        0     1675 2024-05-20 09:18:14.140486 pydivkit-30.1.0/pydivkit/div/div_fade_transition.py
--rw-r--r--   0        0        0      340 2024-05-20 09:18:14.128314 pydivkit-30.1.0/pydivkit/div/div_filter.py
--rw-r--r--   0        0        0      564 2024-05-20 09:18:14.134892 pydivkit-30.1.0/pydivkit/div/div_filter_rtl_mirror.py
--rw-r--r--   0        0        0      686 2024-05-20 09:18:14.140288 pydivkit-30.1.0/pydivkit/div/div_fixed_count.py
--rw-r--r--   0        0        0     3267 2024-05-20 09:18:14.157804 pydivkit-30.1.0/pydivkit/div/div_fixed_length_input_mask.py
--rw-r--r--   0        0        0     1070 2024-05-20 09:18:14.145945 pydivkit-30.1.0/pydivkit/div/div_fixed_size.py
--rw-r--r--   0        0        0     2850 2024-05-20 09:18:14.151386 pydivkit-30.1.0/pydivkit/div/div_focus.py
--rw-r--r--   0        0        0      300 2024-05-20 09:18:14.144735 pydivkit-30.1.0/pydivkit/div/div_font_weight.py
--rw-r--r--   0        0        0    15538 2024-05-20 09:18:14.223783 pydivkit-30.1.0/pydivkit/div/div_gallery.py
--rw-r--r--   0        0        0    14157 2024-05-20 09:18:14.216764 pydivkit-30.1.0/pydivkit/div/div_gif_image.py
--rw-r--r--   0        0        0    12630 2024-05-20 09:18:14.228635 pydivkit-30.1.0/pydivkit/div/div_grid.py
--rw-r--r--   0        0        0    15881 2024-05-20 09:18:14.236836 pydivkit-30.1.0/pydivkit/div/div_image.py
--rw-r--r--   0        0        0     2530 2024-05-20 09:18:14.180651 pydivkit-30.1.0/pydivkit/div/div_image_background.py
--rw-r--r--   0        0        0      300 2024-05-20 09:18:14.167817 pydivkit-30.1.0/pydivkit/div/div_image_scale.py
--rw-r--r--   0        0        0    13813 2024-05-20 09:18:14.228711 pydivkit-30.1.0/pydivkit/div/div_indicator.py
--rw-r--r--   0        0        0      490 2024-05-20 09:18:14.171754 pydivkit-30.1.0/pydivkit/div/div_indicator_item_placement.py
--rw-r--r--   0        0        0      516 2024-05-20 09:18:14.179571 pydivkit-30.1.0/pydivkit/div/div_infinity_count.py
--rw-r--r--   0        0        0    16451 2024-05-20 09:18:14.272678 pydivkit-30.1.0/pydivkit/div/div_input.py
--rw-r--r--   0        0        0      478 2024-05-20 09:18:14.186593 pydivkit-30.1.0/pydivkit/div/div_input_mask.py
--rw-r--r--   0        0        0      648 2024-05-20 09:18:14.190068 pydivkit-30.1.0/pydivkit/div/div_input_mask_base.py
--rw-r--r--   0        0        0      424 2024-05-20 09:18:14.200207 pydivkit-30.1.0/pydivkit/div/div_input_validator.py
--rw-r--r--   0        0        0     1277 2024-05-20 09:18:14.207123 pydivkit-30.1.0/pydivkit/div/div_input_validator_base.py
--rw-r--r--   0        0        0     1710 2024-05-20 09:18:14.220607 pydivkit-30.1.0/pydivkit/div/div_input_validator_expression.py
--rw-r--r--   0        0        0     1628 2024-05-20 09:18:14.233751 pydivkit-30.1.0/pydivkit/div/div_input_validator_regex.py
--rw-r--r--   0        0        0      255 2024-05-20 09:18:14.227018 pydivkit-30.1.0/pydivkit/div/div_line_style.py
--rw-r--r--   0        0        0     1046 2024-05-20 09:18:14.236257 pydivkit-30.1.0/pydivkit/div/div_linear_gradient.py
--rw-r--r--   0        0        0      974 2024-05-20 09:18:14.237407 pydivkit-30.1.0/pydivkit/div/div_match_parent_size.py
--rw-r--r--   0        0        0      858 2024-05-20 09:18:14.242486 pydivkit-30.1.0/pydivkit/div/div_neighbour_page_size.py
--rw-r--r--   0        0        0     1297 2024-05-20 09:18:14.243154 pydivkit-30.1.0/pydivkit/div/div_nine_patch_background.py
--rw-r--r--   0        0        0      795 2024-05-20 09:18:14.247837 pydivkit-30.1.0/pydivkit/div/div_page_size.py
--rw-r--r--   0        0        0      443 2024-05-20 09:18:14.241492 pydivkit-30.1.0/pydivkit/div/div_page_transformation.py
--rw-r--r--   0        0        0     3983 2024-05-20 09:18:14.263223 pydivkit-30.1.0/pydivkit/div/div_page_transformation_overlap.py
--rw-r--r--   0        0        0     3379 2024-05-20 09:18:14.262260 pydivkit-30.1.0/pydivkit/div/div_page_transformation_slide.py
--rw-r--r--   0        0        0    13945 2024-05-20 09:18:14.307124 pydivkit-30.1.0/pydivkit/div/div_pager.py
--rw-r--r--   0        0        0      369 2024-05-20 09:18:14.251427 pydivkit-30.1.0/pydivkit/div/div_pager_layout_mode.py
--rw-r--r--   0        0        0     1928 2024-05-20 09:18:14.264204 pydivkit-30.1.0/pydivkit/div/div_patch.py
--rw-r--r--   0        0        0      694 2024-05-20 09:18:14.258591 pydivkit-30.1.0/pydivkit/div/div_percentage_size.py
--rw-r--r--   0        0        0      820 2024-05-20 09:18:14.261479 pydivkit-30.1.0/pydivkit/div/div_phone_input_mask.py
--rw-r--r--   0        0        0      357 2024-05-20 09:18:14.261289 pydivkit-30.1.0/pydivkit/div/div_pivot.py
--rw-r--r--   0        0        0     1116 2024-05-20 09:18:14.274285 pydivkit-30.1.0/pydivkit/div/div_pivot_fixed.py
--rw-r--r--   0        0        0      800 2024-05-20 09:18:14.274269 pydivkit-30.1.0/pydivkit/div/div_pivot_percentage.py
--rw-r--r--   0        0        0      768 2024-05-20 09:18:14.271643 pydivkit-30.1.0/pydivkit/div/div_point.py
--rw-r--r--   0        0        0     1933 2024-05-20 09:18:14.281089 pydivkit-30.1.0/pydivkit/div/div_radial_gradient.py
--rw-r--r--   0        0        0      473 2024-05-20 09:18:14.273510 pydivkit-30.1.0/pydivkit/div/div_radial_gradient_center.py
--rw-r--r--   0        0        0     1136 2024-05-20 09:18:14.280160 pydivkit-30.1.0/pydivkit/div/div_radial_gradient_fixed_center.py
--rw-r--r--   0        0        0      412 2024-05-20 09:18:14.280345 pydivkit-30.1.0/pydivkit/div/div_radial_gradient_radius.py
--rw-r--r--   0        0        0      800 2024-05-20 09:18:14.285644 pydivkit-30.1.0/pydivkit/div/div_radial_gradient_relative_center.py
--rw-r--r--   0        0        0     1052 2024-05-20 09:18:14.291656 pydivkit-30.1.0/pydivkit/div/div_radial_gradient_relative_radius.py
--rw-r--r--   0        0        0     1721 2024-05-20 09:18:14.292216 pydivkit-30.1.0/pydivkit/div/div_rounded_rectangle_shape.py
--rw-r--r--   0        0        0     2300 2024-05-20 09:18:14.295685 pydivkit-30.1.0/pydivkit/div/div_scale_transition.py
--rw-r--r--   0        0        0    13636 2024-05-20 09:18:14.349116 pydivkit-30.1.0/pydivkit/div/div_select.py
--rw-r--r--   0        0        0    12803 2024-05-20 09:18:14.347075 pydivkit-30.1.0/pydivkit/div/div_separator.py
--rw-r--r--   0        0        0     1198 2024-05-20 09:18:14.293940 pydivkit-30.1.0/pydivkit/div/div_shadow.py
--rw-r--r--   0        0        0      380 2024-05-20 09:18:14.295196 pydivkit-30.1.0/pydivkit/div/div_shape.py
--rw-r--r--   0        0        0     1144 2024-05-20 09:18:14.309919 pydivkit-30.1.0/pydivkit/div/div_shape_drawable.py
--rw-r--r--   0        0        0     2699 2024-05-20 09:18:14.310877 pydivkit-30.1.0/pydivkit/div/div_sight_action.py
--rw-r--r--   0        0        0      424 2024-05-20 09:18:14.305808 pydivkit-30.1.0/pydivkit/div/div_size.py
--rw-r--r--   0        0        0      256 2024-05-20 09:18:14.306473 pydivkit-30.1.0/pydivkit/div/div_size_unit.py
--rw-r--r--   0        0        0     2360 2024-05-20 09:18:14.317505 pydivkit-30.1.0/pydivkit/div/div_slide_transition.py
--rw-r--r--   0        0        0    16397 2024-05-20 09:18:14.408225 pydivkit-30.1.0/pydivkit/div/div_slider.py
--rw-r--r--   0        0        0      700 2024-05-20 09:18:14.326191 pydivkit-30.1.0/pydivkit/div/div_solid_background.py
--rw-r--r--   0        0        0    13634 2024-05-20 09:18:14.379124 pydivkit-30.1.0/pydivkit/div/div_state.py
--rw-r--r--   0        0        0     1101 2024-05-20 09:18:14.327294 pydivkit-30.1.0/pydivkit/div/div_stretch_indicator_item_placement.py
--rw-r--r--   0        0        0     1000 2024-05-20 09:18:14.331310 pydivkit-30.1.0/pydivkit/div/div_stroke.py
--rw-r--r--   0        0        0    20334 2024-05-20 09:18:14.428943 pydivkit-30.1.0/pydivkit/div/div_tabs.py
--rw-r--r--   0        0        0    25955 2024-05-20 09:18:14.485229 pydivkit-30.1.0/pydivkit/div/div_text.py
--rw-r--r--   0        0        0      373 2024-05-20 09:18:14.335424 pydivkit-30.1.0/pydivkit/div/div_text_gradient.py
--rw-r--r--   0        0        0      319 2024-05-20 09:18:14.347489 pydivkit-30.1.0/pydivkit/div/div_text_range_background.py
--rw-r--r--   0        0        0      975 2024-05-20 09:18:14.351514 pydivkit-30.1.0/pydivkit/div/div_text_range_border.py
--rw-r--r--   0        0        0     2706 2024-05-20 09:18:14.364914 pydivkit-30.1.0/pydivkit/div/div_timer.py
--rw-r--r--   0        0        0     2922 2024-05-20 09:18:14.375775 pydivkit-30.1.0/pydivkit/div/div_tooltip.py
--rw-r--r--   0        0        0     1171 2024-05-20 09:18:14.362244 pydivkit-30.1.0/pydivkit/div/div_transform.py
--rw-r--r--   0        0        0     1234 2024-05-20 09:18:14.368307 pydivkit-30.1.0/pydivkit/div/div_transition_base.py
--rw-r--r--   0        0        0      338 2024-05-20 09:18:14.378806 pydivkit-30.1.0/pydivkit/div/div_transition_selector.py
--rw-r--r--   0        0        0      333 2024-05-20 09:18:14.379500 pydivkit-30.1.0/pydivkit/div/div_transition_trigger.py
--rw-r--r--   0        0        0     1581 2024-05-20 09:18:14.391891 pydivkit-30.1.0/pydivkit/div/div_trigger.py
--rw-r--r--   0        0        0      593 2024-05-20 09:18:14.385950 pydivkit-30.1.0/pydivkit/div/div_typed_value.py
--rw-r--r--   0        0        0      663 2024-05-20 09:18:14.389472 pydivkit-30.1.0/pydivkit/div/div_variable.py
--rw-r--r--   0        0        0    14416 2024-05-20 09:18:14.455426 pydivkit-30.1.0/pydivkit/div/div_video.py
--rw-r--r--   0        0        0      276 2024-05-20 09:18:14.391209 pydivkit-30.1.0/pydivkit/div/div_video_scale.py
--rw-r--r--   0        0        0     2331 2024-05-20 09:18:14.412387 pydivkit-30.1.0/pydivkit/div/div_video_source.py
--rw-r--r--   0        0        0      286 2024-05-20 09:18:14.400915 pydivkit-30.1.0/pydivkit/div/div_visibility.py
--rw-r--r--   0        0        0     3490 2024-05-20 09:18:14.415334 pydivkit-30.1.0/pydivkit/div/div_visibility_action.py
--rw-r--r--   0        0        0     2298 2024-05-20 09:18:14.416476 pydivkit-30.1.0/pydivkit/div/div_wrap_content_size.py
--rw-r--r--   0        0        0      611 2024-05-20 09:18:14.415753 pydivkit-30.1.0/pydivkit/div/integer_value.py
--rw-r--r--   0        0        0      843 2024-05-20 09:18:14.427987 pydivkit-30.1.0/pydivkit/div/integer_variable.py
--rw-r--r--   0        0        0      611 2024-05-20 09:18:14.427784 pydivkit-30.1.0/pydivkit/div/number_value.py
--rw-r--r--   0        0        0      849 2024-05-20 09:18:14.433017 pydivkit-30.1.0/pydivkit/div/number_variable.py
--rw-r--r--   0        0        0      607 2024-05-20 09:18:14.431162 pydivkit-30.1.0/pydivkit/div/string_value.py
--rw-r--r--   0        0        0      837 2024-05-20 09:18:14.437621 pydivkit-30.1.0/pydivkit/div/string_variable.py
--rw-r--r--   0        0        0      617 2024-05-20 09:18:14.442151 pydivkit-30.1.0/pydivkit/div/url_value.py
--rw-r--r--   0        0        0      859 2024-05-20 09:18:14.444550 pydivkit-30.1.0/pydivkit/div/url_variable.py
--rw-r--r--   0        0        0        0 2024-05-20 09:17:17.816935 pydivkit-30.1.0/pydivkit/py.typed
--rw-r--r--   0        0        0     1697 2024-05-20 09:17:17.816935 pydivkit-30.1.0/pyproject.toml
--rw-r--r--   0        0        0    10885 1970-01-01 00:00:00.000000 pydivkit-30.1.0/PKG-INFO
+-rw-r--r--   0        0        0     9446 2024-05-27 11:01:33.857126 pydivkit-30.2.0/README.md
+-rw-r--r--   0        0        0      700 2024-05-27 11:01:33.857126 pydivkit-30.2.0/pydivkit/__init__.py
+-rw-r--r--   0        0        0      164 2024-05-27 11:01:33.857126 pydivkit-30.2.0/pydivkit/core/__init__.py
+-rw-r--r--   0        0        0      445 2024-05-27 11:01:33.857126 pydivkit-30.2.0/pydivkit/core/compat.py
+-rw-r--r--   0        0        0    28631 2024-05-27 11:01:33.857126 pydivkit-30.2.0/pydivkit/core/entities.py
+-rw-r--r--   0        0        0     3039 2024-05-27 11:01:33.857126 pydivkit-30.2.0/pydivkit/core/fields.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:01:33.857126 pydivkit-30.2.0/pydivkit/core/types/__init__.py
+-rw-r--r--   0        0        0      728 2024-05-27 11:01:33.857126 pydivkit-30.2.0/pydivkit/core/types/union.py
+-rw-r--r--   0        0        0    17078 2024-05-27 11:02:50.013597 pydivkit-30.2.0/pydivkit/div/__init__.py
+-rw-r--r--   0        0        0      611 2024-05-27 11:02:48.446516 pydivkit-30.2.0/pydivkit/div/array_value.py
+-rw-r--r--   0        0        0      857 2024-05-27 11:02:48.411509 pydivkit-30.2.0/pydivkit/div/array_variable.py
+-rw-r--r--   0        0        0      613 2024-05-27 11:02:48.434706 pydivkit-30.2.0/pydivkit/div/boolean_value.py
+-rw-r--r--   0        0        0      861 2024-05-27 11:02:48.420336 pydivkit-30.2.0/pydivkit/div/boolean_variable.py
+-rw-r--r--   0        0        0      627 2024-05-27 11:02:48.416701 pydivkit-30.2.0/pydivkit/div/color_value.py
+-rw-r--r--   0        0        0      875 2024-05-27 11:02:48.435499 pydivkit-30.2.0/pydivkit/div/color_variable.py
+-rw-r--r--   0        0        0      603 2024-05-27 11:02:48.413956 pydivkit-30.2.0/pydivkit/div/content_text.py
+-rw-r--r--   0        0        0      621 2024-05-27 11:02:48.427327 pydivkit-30.2.0/pydivkit/div/content_url.py
+-rw-r--r--   0        0        0      609 2024-05-27 11:02:48.461621 pydivkit-30.2.0/pydivkit/div/dict_value.py
+-rw-r--r--   0        0        0      856 2024-05-27 11:02:48.464151 pydivkit-30.2.0/pydivkit/div/dict_variable.py
+-rw-r--r--   0        0        0      863 2024-05-27 11:02:48.438157 pydivkit-30.2.0/pydivkit/div/div.py
+-rw-r--r--   0        0        0     1209 2024-05-27 11:02:48.516104 pydivkit-30.2.0/pydivkit/div/div_absolute_edge_insets.py
+-rw-r--r--   0        0        0     3234 2024-05-27 11:02:48.532292 pydivkit-30.2.0/pydivkit/div/div_accessibility.py
+-rw-r--r--   0        0        0     4138 2024-05-27 11:02:48.512670 pydivkit-30.2.0/pydivkit/div/div_action.py
+-rw-r--r--   0        0        0     1057 2024-05-27 11:02:48.539644 pydivkit-30.2.0/pydivkit/div/div_action_array_insert_value.py
+-rw-r--r--   0        0        0      863 2024-05-27 11:02:48.492901 pydivkit-30.2.0/pydivkit/div/div_action_array_remove_value.py
+-rw-r--r--   0        0        0      529 2024-05-27 11:02:48.550358 pydivkit-30.2.0/pydivkit/div/div_action_clear_focus.py
+-rw-r--r--   0        0        0      837 2024-05-27 11:02:48.542608 pydivkit-30.2.0/pydivkit/div/div_action_copy_to_clipboard.py
+-rw-r--r--   0        0        0      346 2024-05-27 11:02:48.491658 pydivkit-30.2.0/pydivkit/div/div_action_copy_to_clipboard_content.py
+-rw-r--r--   0        0        0      732 2024-05-27 11:02:48.549481 pydivkit-30.2.0/pydivkit/div/div_action_focus_element.py
+-rw-r--r--   0        0        0      885 2024-05-27 11:02:48.551437 pydivkit-30.2.0/pydivkit/div/div_action_set_variable.py
+-rw-r--r--   0        0        0      759 2024-05-27 11:02:48.577931 pydivkit-30.2.0/pydivkit/div/div_action_typed.py
+-rw-r--r--   0        0        0      321 2024-05-27 11:02:48.572788 pydivkit-30.2.0/pydivkit/div/div_alignment_horizontal.py
+-rw-r--r--   0        0        0      309 2024-05-27 11:02:48.582045 pydivkit-30.2.0/pydivkit/div/div_alignment_vertical.py
+-rw-r--r--   0        0        0     3016 2024-05-27 11:02:48.629956 pydivkit-30.2.0/pydivkit/div/div_animation.py
+-rw-r--r--   0        0        0      371 2024-05-27 11:02:48.593556 pydivkit-30.2.0/pydivkit/div/div_animation_interpolator.py
+-rw-r--r--   0        0        0      879 2024-05-27 11:02:48.585613 pydivkit-30.2.0/pydivkit/div/div_appearance_set_transition.py
+-rw-r--r--   0        0        0      557 2024-05-27 11:02:48.578373 pydivkit-30.2.0/pydivkit/div/div_appearance_transition.py
+-rw-r--r--   0        0        0      671 2024-05-27 11:02:48.594107 pydivkit-30.2.0/pydivkit/div/div_aspect.py
+-rw-r--r--   0        0        0      599 2024-05-27 11:02:48.604552 pydivkit-30.2.0/pydivkit/div/div_background.py
+-rw-r--r--   0        0        0     9648 2024-05-27 11:02:48.658123 pydivkit-30.2.0/pydivkit/div/div_base.py
+-rw-r--r--   0        0        0      369 2024-05-27 11:02:48.629896 pydivkit-30.2.0/pydivkit/div/div_blend_mode.py
+-rw-r--r--   0        0        0      764 2024-05-27 11:02:48.642290 pydivkit-30.2.0/pydivkit/div/div_blur.py
+-rw-r--r--   0        0        0     1734 2024-05-27 11:02:48.634845 pydivkit-30.2.0/pydivkit/div/div_border.py
+-rw-r--r--   0        0        0     1403 2024-05-27 11:02:48.644980 pydivkit-30.2.0/pydivkit/div/div_change_bounds_transition.py
+-rw-r--r--   0        0        0      809 2024-05-27 11:02:48.637764 pydivkit-30.2.0/pydivkit/div/div_change_set_transition.py
+-rw-r--r--   0        0        0      420 2024-05-27 11:02:48.636834 pydivkit-30.2.0/pydivkit/div/div_change_transition.py
+-rw-r--r--   0        0        0     1176 2024-05-27 11:02:48.671328 pydivkit-30.2.0/pydivkit/div/div_circle_shape.py
+-rw-r--r--   0        0        0     2552 2024-05-27 11:02:48.666594 pydivkit-30.2.0/pydivkit/div/div_collection_item_builder.py
+-rw-r--r--   0        0        0    18163 2024-05-27 11:02:48.832152 pydivkit-30.2.0/pydivkit/div/div_container.py
+-rw-r--r--   0        0        0      432 2024-05-27 11:02:48.676416 pydivkit-30.2.0/pydivkit/div/div_content_alignment_horizontal.py
+-rw-r--r--   0        0        0      420 2024-05-27 11:02:48.678871 pydivkit-30.2.0/pydivkit/div/div_content_alignment_vertical.py
+-rw-r--r--   0        0        0     1861 2024-05-27 11:02:48.703347 pydivkit-30.2.0/pydivkit/div/div_corners_radius.py
+-rw-r--r--   0        0        0      351 2024-05-27 11:02:48.658422 pydivkit-30.2.0/pydivkit/div/div_count.py
+-rw-r--r--   0        0        0     1246 2024-05-27 11:02:48.693740 pydivkit-30.2.0/pydivkit/div/div_currency_input_mask.py
+-rw-r--r--   0        0        0    10545 2024-05-27 11:02:48.806342 pydivkit-30.2.0/pydivkit/div/div_custom.py
+-rw-r--r--   0        0        0     2826 2024-05-27 11:02:48.723039 pydivkit-30.2.0/pydivkit/div/div_data.py
+-rw-r--r--   0        0        0      872 2024-05-27 11:02:48.723427 pydivkit-30.2.0/pydivkit/div/div_default_indicator_item_placement.py
+-rw-r--r--   0        0        0      802 2024-05-27 11:02:48.708179 pydivkit-30.2.0/pydivkit/div/div_dimension.py
+-rw-r--r--   0        0        0     3504 2024-05-27 11:02:48.750470 pydivkit-30.2.0/pydivkit/div/div_disappear_action.py
+-rw-r--r--   0        0        0     1177 2024-05-27 11:02:48.746594 pydivkit-30.2.0/pydivkit/div/div_download_callbacks.py
+-rw-r--r--   0        0        0      302 2024-05-27 11:02:48.728156 pydivkit-30.2.0/pydivkit/div/div_drawable.py
+-rw-r--r--   0        0        0     2081 2024-05-27 11:02:48.789392 pydivkit-30.2.0/pydivkit/div/div_edge_insets.py
+-rw-r--r--   0        0        0      804 2024-05-27 11:02:48.770074 pydivkit-30.2.0/pydivkit/div/div_extension.py
+-rw-r--r--   0        0        0     1675 2024-05-27 11:02:48.768516 pydivkit-30.2.0/pydivkit/div/div_fade_transition.py
+-rw-r--r--   0        0        0      340 2024-05-27 11:02:48.768406 pydivkit-30.2.0/pydivkit/div/div_filter.py
+-rw-r--r--   0        0        0      564 2024-05-27 11:02:48.789889 pydivkit-30.2.0/pydivkit/div/div_filter_rtl_mirror.py
+-rw-r--r--   0        0        0      686 2024-05-27 11:02:48.854705 pydivkit-30.2.0/pydivkit/div/div_fixed_count.py
+-rw-r--r--   0        0        0     3267 2024-05-27 11:02:48.831555 pydivkit-30.2.0/pydivkit/div/div_fixed_length_input_mask.py
+-rw-r--r--   0        0        0     1070 2024-05-27 11:02:48.802137 pydivkit-30.2.0/pydivkit/div/div_fixed_size.py
+-rw-r--r--   0        0        0     2850 2024-05-27 11:02:48.827800 pydivkit-30.2.0/pydivkit/div/div_focus.py
+-rw-r--r--   0        0        0      300 2024-05-27 11:02:48.856806 pydivkit-30.2.0/pydivkit/div/div_font_weight.py
+-rw-r--r--   0        0        0    15538 2024-05-27 11:02:48.964372 pydivkit-30.2.0/pydivkit/div/div_gallery.py
+-rw-r--r--   0        0        0    14157 2024-05-27 11:02:48.984938 pydivkit-30.2.0/pydivkit/div/div_gif_image.py
+-rw-r--r--   0        0        0    12630 2024-05-27 11:02:48.966190 pydivkit-30.2.0/pydivkit/div/div_grid.py
+-rw-r--r--   0        0        0    15881 2024-05-27 11:02:49.101588 pydivkit-30.2.0/pydivkit/div/div_image.py
+-rw-r--r--   0        0        0     2530 2024-05-27 11:02:48.894569 pydivkit-30.2.0/pydivkit/div/div_image_background.py
+-rw-r--r--   0        0        0      300 2024-05-27 11:02:48.856902 pydivkit-30.2.0/pydivkit/div/div_image_scale.py
+-rw-r--r--   0        0        0    13813 2024-05-27 11:02:49.032772 pydivkit-30.2.0/pydivkit/div/div_indicator.py
+-rw-r--r--   0        0        0      490 2024-05-27 11:02:48.880136 pydivkit-30.2.0/pydivkit/div/div_indicator_item_placement.py
+-rw-r--r--   0        0        0      516 2024-05-27 11:02:48.894353 pydivkit-30.2.0/pydivkit/div/div_infinity_count.py
+-rw-r--r--   0        0        0    16451 2024-05-27 11:02:49.123269 pydivkit-30.2.0/pydivkit/div/div_input.py
+-rw-r--r--   0        0        0      478 2024-05-27 11:02:48.928484 pydivkit-30.2.0/pydivkit/div/div_input_mask.py
+-rw-r--r--   0        0        0      648 2024-05-27 11:02:48.922307 pydivkit-30.2.0/pydivkit/div/div_input_mask_base.py
+-rw-r--r--   0        0        0      424 2024-05-27 11:02:48.955640 pydivkit-30.2.0/pydivkit/div/div_input_validator.py
+-rw-r--r--   0        0        0     1277 2024-05-27 11:02:48.976280 pydivkit-30.2.0/pydivkit/div/div_input_validator_base.py
+-rw-r--r--   0        0        0     1710 2024-05-27 11:02:49.032488 pydivkit-30.2.0/pydivkit/div/div_input_validator_expression.py
+-rw-r--r--   0        0        0     1628 2024-05-27 11:02:49.021649 pydivkit-30.2.0/pydivkit/div/div_input_validator_regex.py
+-rw-r--r--   0        0        0      255 2024-05-27 11:02:48.988315 pydivkit-30.2.0/pydivkit/div/div_line_style.py
+-rw-r--r--   0        0        0     1046 2024-05-27 11:02:49.021718 pydivkit-30.2.0/pydivkit/div/div_linear_gradient.py
+-rw-r--r--   0        0        0      974 2024-05-27 11:02:49.035525 pydivkit-30.2.0/pydivkit/div/div_match_parent_size.py
+-rw-r--r--   0        0        0      858 2024-05-27 11:02:49.039492 pydivkit-30.2.0/pydivkit/div/div_neighbour_page_size.py
+-rw-r--r--   0        0        0     1297 2024-05-27 11:02:49.057169 pydivkit-30.2.0/pydivkit/div/div_nine_patch_background.py
+-rw-r--r--   0        0        0      795 2024-05-27 11:02:49.056288 pydivkit-30.2.0/pydivkit/div/div_page_size.py
+-rw-r--r--   0        0        0      443 2024-05-27 11:02:49.067783 pydivkit-30.2.0/pydivkit/div/div_page_transformation.py
+-rw-r--r--   0        0        0     3983 2024-05-27 11:02:49.100528 pydivkit-30.2.0/pydivkit/div/div_page_transformation_overlap.py
+-rw-r--r--   0        0        0     3379 2024-05-27 11:02:49.089001 pydivkit-30.2.0/pydivkit/div/div_page_transformation_slide.py
+-rw-r--r--   0        0        0    13945 2024-05-27 11:02:49.220948 pydivkit-30.2.0/pydivkit/div/div_pager.py
+-rw-r--r--   0        0        0      369 2024-05-27 11:02:49.086336 pydivkit-30.2.0/pydivkit/div/div_pager_layout_mode.py
+-rw-r--r--   0        0        0     1928 2024-05-27 11:02:49.106581 pydivkit-30.2.0/pydivkit/div/div_patch.py
+-rw-r--r--   0        0        0      694 2024-05-27 11:02:49.113697 pydivkit-30.2.0/pydivkit/div/div_percentage_size.py
+-rw-r--r--   0        0        0      820 2024-05-27 11:02:49.146612 pydivkit-30.2.0/pydivkit/div/div_phone_input_mask.py
+-rw-r--r--   0        0        0      357 2024-05-27 11:02:49.117537 pydivkit-30.2.0/pydivkit/div/div_pivot.py
+-rw-r--r--   0        0        0     1116 2024-05-27 11:02:49.156295 pydivkit-30.2.0/pydivkit/div/div_pivot_fixed.py
+-rw-r--r--   0        0        0      800 2024-05-27 11:02:49.155080 pydivkit-30.2.0/pydivkit/div/div_pivot_percentage.py
+-rw-r--r--   0        0        0      768 2024-05-27 11:02:49.136193 pydivkit-30.2.0/pydivkit/div/div_point.py
+-rw-r--r--   0        0        0     1933 2024-05-27 11:02:49.167776 pydivkit-30.2.0/pydivkit/div/div_radial_gradient.py
+-rw-r--r--   0        0        0      473 2024-05-27 11:02:49.138236 pydivkit-30.2.0/pydivkit/div/div_radial_gradient_center.py
+-rw-r--r--   0        0        0     1136 2024-05-27 11:02:49.164002 pydivkit-30.2.0/pydivkit/div/div_radial_gradient_fixed_center.py
+-rw-r--r--   0        0        0      412 2024-05-27 11:02:49.163029 pydivkit-30.2.0/pydivkit/div/div_radial_gradient_radius.py
+-rw-r--r--   0        0        0      800 2024-05-27 11:02:49.183767 pydivkit-30.2.0/pydivkit/div/div_radial_gradient_relative_center.py
+-rw-r--r--   0        0        0     1052 2024-05-27 11:02:49.201082 pydivkit-30.2.0/pydivkit/div/div_radial_gradient_relative_radius.py
+-rw-r--r--   0        0        0     1721 2024-05-27 11:02:49.287961 pydivkit-30.2.0/pydivkit/div/div_rounded_rectangle_shape.py
+-rw-r--r--   0        0        0     2300 2024-05-27 11:02:49.210694 pydivkit-30.2.0/pydivkit/div/div_scale_transition.py
+-rw-r--r--   0        0        0    13636 2024-05-27 11:02:49.354416 pydivkit-30.2.0/pydivkit/div/div_select.py
+-rw-r--r--   0        0        0    12803 2024-05-27 11:02:49.319069 pydivkit-30.2.0/pydivkit/div/div_separator.py
+-rw-r--r--   0        0        0     1198 2024-05-27 11:02:49.186656 pydivkit-30.2.0/pydivkit/div/div_shadow.py
+-rw-r--r--   0        0        0      380 2024-05-27 11:02:49.209608 pydivkit-30.2.0/pydivkit/div/div_shape.py
+-rw-r--r--   0        0        0     1144 2024-05-27 11:02:49.233684 pydivkit-30.2.0/pydivkit/div/div_shape_drawable.py
+-rw-r--r--   0        0        0     2699 2024-05-27 11:02:49.248572 pydivkit-30.2.0/pydivkit/div/div_sight_action.py
+-rw-r--r--   0        0        0      424 2024-05-27 11:02:49.230212 pydivkit-30.2.0/pydivkit/div/div_size.py
+-rw-r--r--   0        0        0      256 2024-05-27 11:02:49.241846 pydivkit-30.2.0/pydivkit/div/div_size_unit.py
+-rw-r--r--   0        0        0     2360 2024-05-27 11:02:49.332795 pydivkit-30.2.0/pydivkit/div/div_slide_transition.py
+-rw-r--r--   0        0        0    16397 2024-05-27 11:02:49.454789 pydivkit-30.2.0/pydivkit/div/div_slider.py
+-rw-r--r--   0        0        0      700 2024-05-27 11:02:49.288179 pydivkit-30.2.0/pydivkit/div/div_solid_background.py
+-rw-r--r--   0        0        0    13634 2024-05-27 11:02:49.596924 pydivkit-30.2.0/pydivkit/div/div_state.py
+-rw-r--r--   0        0        0     1101 2024-05-27 11:02:49.371716 pydivkit-30.2.0/pydivkit/div/div_stretch_indicator_item_placement.py
+-rw-r--r--   0        0        0     1000 2024-05-27 11:02:49.344032 pydivkit-30.2.0/pydivkit/div/div_stroke.py
+-rw-r--r--   0        0        0    21814 2024-05-27 11:02:49.745039 pydivkit-30.2.0/pydivkit/div/div_tabs.py
+-rw-r--r--   0        0        0    25955 2024-05-27 11:02:49.938396 pydivkit-30.2.0/pydivkit/div/div_text.py
+-rw-r--r--   0        0        0      373 2024-05-27 11:02:49.354058 pydivkit-30.2.0/pydivkit/div/div_text_gradient.py
+-rw-r--r--   0        0        0      319 2024-05-27 11:02:49.383947 pydivkit-30.2.0/pydivkit/div/div_text_range_background.py
+-rw-r--r--   0        0        0      975 2024-05-27 11:02:49.407495 pydivkit-30.2.0/pydivkit/div/div_text_range_border.py
+-rw-r--r--   0        0        0     2706 2024-05-27 11:02:49.431250 pydivkit-30.2.0/pydivkit/div/div_timer.py
+-rw-r--r--   0        0        0     2922 2024-05-27 11:02:49.421331 pydivkit-30.2.0/pydivkit/div/div_tooltip.py
+-rw-r--r--   0        0        0     1171 2024-05-27 11:02:49.423243 pydivkit-30.2.0/pydivkit/div/div_transform.py
+-rw-r--r--   0        0        0     1234 2024-05-27 11:02:49.446698 pydivkit-30.2.0/pydivkit/div/div_transition_base.py
+-rw-r--r--   0        0        0      338 2024-05-27 11:02:49.463912 pydivkit-30.2.0/pydivkit/div/div_transition_selector.py
+-rw-r--r--   0        0        0      333 2024-05-27 11:02:49.460155 pydivkit-30.2.0/pydivkit/div/div_transition_trigger.py
+-rw-r--r--   0        0        0     1581 2024-05-27 11:02:49.516314 pydivkit-30.2.0/pydivkit/div/div_trigger.py
+-rw-r--r--   0        0        0      593 2024-05-27 11:02:49.467814 pydivkit-30.2.0/pydivkit/div/div_typed_value.py
+-rw-r--r--   0        0        0      663 2024-05-27 11:02:49.489272 pydivkit-30.2.0/pydivkit/div/div_variable.py
+-rw-r--r--   0        0        0    14416 2024-05-27 11:02:49.920433 pydivkit-30.2.0/pydivkit/div/div_video.py
+-rw-r--r--   0        0        0      276 2024-05-27 11:02:49.497625 pydivkit-30.2.0/pydivkit/div/div_video_scale.py
+-rw-r--r--   0        0        0     2331 2024-05-27 11:02:49.549720 pydivkit-30.2.0/pydivkit/div/div_video_source.py
+-rw-r--r--   0        0        0      286 2024-05-27 11:02:49.552937 pydivkit-30.2.0/pydivkit/div/div_visibility.py
+-rw-r--r--   0        0        0     3490 2024-05-27 11:02:49.567668 pydivkit-30.2.0/pydivkit/div/div_visibility_action.py
+-rw-r--r--   0        0        0     2298 2024-05-27 11:02:49.613935 pydivkit-30.2.0/pydivkit/div/div_wrap_content_size.py
+-rw-r--r--   0        0        0      611 2024-05-27 11:02:49.639929 pydivkit-30.2.0/pydivkit/div/integer_value.py
+-rw-r--r--   0        0        0      843 2024-05-27 11:02:49.715929 pydivkit-30.2.0/pydivkit/div/integer_variable.py
+-rw-r--r--   0        0        0      611 2024-05-27 11:02:49.711319 pydivkit-30.2.0/pydivkit/div/number_value.py
+-rw-r--r--   0        0        0      849 2024-05-27 11:02:49.725074 pydivkit-30.2.0/pydivkit/div/number_variable.py
+-rw-r--r--   0        0        0      607 2024-05-27 11:02:49.764902 pydivkit-30.2.0/pydivkit/div/string_value.py
+-rw-r--r--   0        0        0      837 2024-05-27 11:02:49.754341 pydivkit-30.2.0/pydivkit/div/string_variable.py
+-rw-r--r--   0        0        0      617 2024-05-27 11:02:49.786945 pydivkit-30.2.0/pydivkit/div/url_value.py
+-rw-r--r--   0        0        0      859 2024-05-27 11:02:49.788923 pydivkit-30.2.0/pydivkit/div/url_variable.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:01:33.857126 pydivkit-30.2.0/pydivkit/py.typed
+-rw-r--r--   0        0        0     1697 2024-05-27 11:01:33.857126 pydivkit-30.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10885 1970-01-01 00:00:00.000000 pydivkit-30.2.0/PKG-INFO
```

### Comparing `pydivkit-30.1.0/README.md` & `pydivkit-30.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/__init__.py` & `pydivkit-30.2.0/pydivkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/core/entities.py` & `pydivkit-30.2.0/pydivkit/core/entities.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/core/fields.py` & `pydivkit-30.2.0/pydivkit/core/fields.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/core/types/union.py` & `pydivkit-30.2.0/pydivkit/core/types/union.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/__init__.py` & `pydivkit-30.2.0/pydivkit/div/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,16 @@
 from .div_solid_background import DivSolidBackground
 from .div_state import DivState, DivStateState
 from .div_stretch_indicator_item_placement import (
     DivStretchIndicatorItemPlacement,
 )
 from .div_stroke import DivStroke
 from .div_tabs import (
-    DivTabs, DivTabsItem, DivTabsTabTitleStyle, TabTitleStyleAnimationType,
+    DivTabs, DivTabsItem, DivTabsTabTitleDelimiter, DivTabsTabTitleStyle,
+    TabTitleStyleAnimationType,
 )
 from .div_text import (
     DivText, DivTextEllipsis, DivTextImage, DivTextRange, DivTextTruncate,
 )
 from .div_text_gradient import DivTextGradient
 from .div_text_range_background import DivTextRangeBackground
 from .div_text_range_border import DivTextRangeBorder
@@ -277,14 +278,15 @@
 DivSolidBackground.update_forward_refs()
 DivState.update_forward_refs()
 DivStateState.update_forward_refs()
 DivStretchIndicatorItemPlacement.update_forward_refs()
 DivStroke.update_forward_refs()
 DivTabs.update_forward_refs()
 DivTabsItem.update_forward_refs()
+DivTabsTabTitleDelimiter.update_forward_refs()
 DivTabsTabTitleStyle.update_forward_refs()
 DivText.update_forward_refs()
 DivTextEllipsis.update_forward_refs()
 DivTextImage.update_forward_refs()
 DivTextRange.update_forward_refs()
 DivTextRangeBorder.update_forward_refs()
 DivTimer.update_forward_refs()
@@ -303,8 +305,8 @@
 NumberValue.update_forward_refs()
 NumberVariable.update_forward_refs()
 StringValue.update_forward_refs()
 StringVariable.update_forward_refs()
 UrlValue.update_forward_refs()
 UrlVariable.update_forward_refs()
 
-__all__ = ("ArrayValue", "ArrayVariable", "BooleanValue", "BooleanVariable", "ColorValue", "ColorVariable", "ContentText", "ContentUrl", "DelimiterStyleOrientation", "DictValue", "DictVariable", "Div", "DivAbsoluteEdgeInsets", "DivAccessibility", "DivAccessibilityMode", "DivAccessibilityType", "DivAction", "DivActionArrayInsertValue", "DivActionArrayRemoveValue", "DivActionClearFocus", "DivActionCopyToClipboard", "DivActionCopyToClipboardContent", "DivActionFocusElement", "DivActionMenuItem", "DivActionSetVariable", "DivActionTarget", "DivActionTyped", "DivAlignmentHorizontal", "DivAlignmentVertical", "DivAnimation", "DivAnimationInterpolator", "DivAnimationName", "DivAppearanceSetTransition", "DivAppearanceTransition", "DivAspect", "DivBackground", "DivBase", "DivBlendMode", "DivBlur", "DivBorder", "DivChangeBoundsTransition", "DivChangeSetTransition", "DivChangeTransition", "DivCircleShape", "DivCollectionItemBuilder", "DivCollectionItemBuilderPrototype", "DivContainer", "DivContainerLayoutMode", "DivContainerOrientation", "DivContainerSeparator", "DivContentAlignmentHorizontal", "DivContentAlignmentVertical", "DivCornersRadius", "DivCount", "DivCurrencyInputMask", "DivCustom", "DivData", "DivDataState", "DivDefaultIndicatorItemPlacement", "DivDimension", "DivDisappearAction", "DivDownloadCallbacks", "DivDrawable", "DivEdgeInsets", "DivExtension", "DivFadeTransition", "DivFilter", "DivFilterRtlMirror", "DivFixedCount", "DivFixedLengthInputMask", "DivFixedLengthInputMaskPatternElement", "DivFixedSize", "DivFocus", "DivFocusNextFocusIds", "DivFontWeight", "DivGallery", "DivGalleryCrossContentAlignment", "DivGalleryOrientation", "DivGalleryScrollMode", "DivGalleryScrollbar", "DivGifImage", "DivGrid", "DivImage", "DivImageBackground", "DivImageScale", "DivIndicator", "DivIndicatorAnimation", "DivIndicatorItemPlacement", "DivInfinityCount", "DivInput", "DivInputKeyboardType", "DivInputMask", "DivInputMaskBase", "DivInputNativeInterface", "DivInputValidator", "DivInputValidatorBase", "DivInputValidatorExpression", "DivInputValidatorRegex", "DivLineStyle", "DivLinearGradient", "DivMatchParentSize", "DivNeighbourPageSize", "DivNinePatchBackground", "DivPageSize", "DivPageTransformation", "DivPageTransformationOverlap", "DivPageTransformationSlide", "DivPager", "DivPagerLayoutMode", "DivPagerOrientation", "DivPatch", "DivPatchChange", "DivPatchMode", "DivPercentageSize", "DivPhoneInputMask", "DivPivot", "DivPivotFixed", "DivPivotPercentage", "DivPoint", "DivRadialGradient", "DivRadialGradientCenter", "DivRadialGradientFixedCenter", "DivRadialGradientRadius", "DivRadialGradientRelativeCenter", "DivRadialGradientRelativeRadius", "DivRadialGradientRelativeRadiusValue", "DivRoundedRectangleShape", "DivScaleTransition", "DivSelect", "DivSelectOption", "DivSeparator", "DivSeparatorDelimiterStyle", "DivShadow", "DivShape", "DivShapeDrawable", "DivSightAction", "DivSize", "DivSizeUnit", "DivSlideTransition", "DivSlideTransitionEdge", "DivSlider", "DivSliderRange", "DivSliderTextStyle", "DivSolidBackground", "DivState", "DivStateState", "DivStretchIndicatorItemPlacement", "DivStroke", "DivTabs", "DivTabsItem", "DivTabsTabTitleStyle", "DivText", "DivTextEllipsis", "DivTextGradient", "DivTextImage", "DivTextRange", "DivTextRangeBackground", "DivTextRangeBorder", "DivTextTruncate", "DivTimer", "DivTooltip", "DivTooltipPosition", "DivTransform", "DivTransitionBase", "DivTransitionSelector", "DivTransitionTrigger", "DivTrigger", "DivTriggerMode", "DivTypedValue", "DivVariable", "DivVideo", "DivVideoScale", "DivVideoSource", "DivVideoSourceResolution", "DivVisibility", "DivVisibilityAction", "DivWrapContentSize", "DivWrapContentSizeConstraintSize", "IntegerValue", "IntegerVariable", "NumberValue", "NumberVariable", "StringValue", "StringVariable", "TabTitleStyleAnimationType", "UrlValue", "UrlVariable")
+__all__ = ("ArrayValue", "ArrayVariable", "BooleanValue", "BooleanVariable", "ColorValue", "ColorVariable", "ContentText", "ContentUrl", "DelimiterStyleOrientation", "DictValue", "DictVariable", "Div", "DivAbsoluteEdgeInsets", "DivAccessibility", "DivAccessibilityMode", "DivAccessibilityType", "DivAction", "DivActionArrayInsertValue", "DivActionArrayRemoveValue", "DivActionClearFocus", "DivActionCopyToClipboard", "DivActionCopyToClipboardContent", "DivActionFocusElement", "DivActionMenuItem", "DivActionSetVariable", "DivActionTarget", "DivActionTyped", "DivAlignmentHorizontal", "DivAlignmentVertical", "DivAnimation", "DivAnimationInterpolator", "DivAnimationName", "DivAppearanceSetTransition", "DivAppearanceTransition", "DivAspect", "DivBackground", "DivBase", "DivBlendMode", "DivBlur", "DivBorder", "DivChangeBoundsTransition", "DivChangeSetTransition", "DivChangeTransition", "DivCircleShape", "DivCollectionItemBuilder", "DivCollectionItemBuilderPrototype", "DivContainer", "DivContainerLayoutMode", "DivContainerOrientation", "DivContainerSeparator", "DivContentAlignmentHorizontal", "DivContentAlignmentVertical", "DivCornersRadius", "DivCount", "DivCurrencyInputMask", "DivCustom", "DivData", "DivDataState", "DivDefaultIndicatorItemPlacement", "DivDimension", "DivDisappearAction", "DivDownloadCallbacks", "DivDrawable", "DivEdgeInsets", "DivExtension", "DivFadeTransition", "DivFilter", "DivFilterRtlMirror", "DivFixedCount", "DivFixedLengthInputMask", "DivFixedLengthInputMaskPatternElement", "DivFixedSize", "DivFocus", "DivFocusNextFocusIds", "DivFontWeight", "DivGallery", "DivGalleryCrossContentAlignment", "DivGalleryOrientation", "DivGalleryScrollMode", "DivGalleryScrollbar", "DivGifImage", "DivGrid", "DivImage", "DivImageBackground", "DivImageScale", "DivIndicator", "DivIndicatorAnimation", "DivIndicatorItemPlacement", "DivInfinityCount", "DivInput", "DivInputKeyboardType", "DivInputMask", "DivInputMaskBase", "DivInputNativeInterface", "DivInputValidator", "DivInputValidatorBase", "DivInputValidatorExpression", "DivInputValidatorRegex", "DivLineStyle", "DivLinearGradient", "DivMatchParentSize", "DivNeighbourPageSize", "DivNinePatchBackground", "DivPageSize", "DivPageTransformation", "DivPageTransformationOverlap", "DivPageTransformationSlide", "DivPager", "DivPagerLayoutMode", "DivPagerOrientation", "DivPatch", "DivPatchChange", "DivPatchMode", "DivPercentageSize", "DivPhoneInputMask", "DivPivot", "DivPivotFixed", "DivPivotPercentage", "DivPoint", "DivRadialGradient", "DivRadialGradientCenter", "DivRadialGradientFixedCenter", "DivRadialGradientRadius", "DivRadialGradientRelativeCenter", "DivRadialGradientRelativeRadius", "DivRadialGradientRelativeRadiusValue", "DivRoundedRectangleShape", "DivScaleTransition", "DivSelect", "DivSelectOption", "DivSeparator", "DivSeparatorDelimiterStyle", "DivShadow", "DivShape", "DivShapeDrawable", "DivSightAction", "DivSize", "DivSizeUnit", "DivSlideTransition", "DivSlideTransitionEdge", "DivSlider", "DivSliderRange", "DivSliderTextStyle", "DivSolidBackground", "DivState", "DivStateState", "DivStretchIndicatorItemPlacement", "DivStroke", "DivTabs", "DivTabsItem", "DivTabsTabTitleDelimiter", "DivTabsTabTitleStyle", "DivText", "DivTextEllipsis", "DivTextGradient", "DivTextImage", "DivTextRange", "DivTextRangeBackground", "DivTextRangeBorder", "DivTextTruncate", "DivTimer", "DivTooltip", "DivTooltipPosition", "DivTransform", "DivTransitionBase", "DivTransitionSelector", "DivTransitionTrigger", "DivTrigger", "DivTriggerMode", "DivTypedValue", "DivVariable", "DivVideo", "DivVideoScale", "DivVideoSource", "DivVideoSourceResolution", "DivVisibility", "DivVisibilityAction", "DivWrapContentSize", "DivWrapContentSizeConstraintSize", "IntegerValue", "IntegerVariable", "NumberValue", "NumberVariable", "StringValue", "StringVariable", "TabTitleStyleAnimationType", "UrlValue", "UrlVariable")
```

### Comparing `pydivkit-30.1.0/pydivkit/div/array_value.py` & `pydivkit-30.2.0/pydivkit/div/array_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/array_variable.py` & `pydivkit-30.2.0/pydivkit/div/array_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/boolean_value.py` & `pydivkit-30.2.0/pydivkit/div/boolean_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/boolean_variable.py` & `pydivkit-30.2.0/pydivkit/div/boolean_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/color_value.py` & `pydivkit-30.2.0/pydivkit/div/color_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/color_variable.py` & `pydivkit-30.2.0/pydivkit/div/color_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/content_text.py` & `pydivkit-30.2.0/pydivkit/div/content_text.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/content_url.py` & `pydivkit-30.2.0/pydivkit/div/content_url.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/dict_value.py` & `pydivkit-30.2.0/pydivkit/div/dict_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/dict_variable.py` & `pydivkit-30.2.0/pydivkit/div/dict_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div.py` & `pydivkit-30.2.0/pydivkit/div/div.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_absolute_edge_insets.py` & `pydivkit-30.2.0/pydivkit/div/div_absolute_edge_insets.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_accessibility.py` & `pydivkit-30.2.0/pydivkit/div/div_accessibility.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_action.py` & `pydivkit-30.2.0/pydivkit/div/div_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_action_array_insert_value.py` & `pydivkit-30.2.0/pydivkit/div/div_action_array_insert_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_action_array_remove_value.py` & `pydivkit-30.2.0/pydivkit/div/div_action_array_remove_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_action_clear_focus.py` & `pydivkit-30.2.0/pydivkit/div/div_action_clear_focus.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_action_copy_to_clipboard.py` & `pydivkit-30.2.0/pydivkit/div/div_action_copy_to_clipboard.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_action_focus_element.py` & `pydivkit-30.2.0/pydivkit/div/div_action_focus_element.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_action_set_variable.py` & `pydivkit-30.2.0/pydivkit/div/div_action_set_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_action_typed.py` & `pydivkit-30.2.0/pydivkit/div/div_action_typed.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_animation.py` & `pydivkit-30.2.0/pydivkit/div/div_animation.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_appearance_set_transition.py` & `pydivkit-30.2.0/pydivkit/div/div_appearance_set_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_appearance_transition.py` & `pydivkit-30.2.0/pydivkit/div/div_appearance_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_aspect.py` & `pydivkit-30.2.0/pydivkit/div/div_aspect.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_background.py` & `pydivkit-30.2.0/pydivkit/div/div_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_base.py` & `pydivkit-30.2.0/pydivkit/div/div_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_blur.py` & `pydivkit-30.2.0/pydivkit/div/div_blur.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_border.py` & `pydivkit-30.2.0/pydivkit/div/div_border.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_change_bounds_transition.py` & `pydivkit-30.2.0/pydivkit/div/div_change_bounds_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_change_set_transition.py` & `pydivkit-30.2.0/pydivkit/div/div_change_set_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_circle_shape.py` & `pydivkit-30.2.0/pydivkit/div/div_circle_shape.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_collection_item_builder.py` & `pydivkit-30.2.0/pydivkit/div/div_collection_item_builder.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_container.py` & `pydivkit-30.2.0/pydivkit/div/div_container.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_corners_radius.py` & `pydivkit-30.2.0/pydivkit/div/div_corners_radius.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_currency_input_mask.py` & `pydivkit-30.2.0/pydivkit/div/div_currency_input_mask.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_custom.py` & `pydivkit-30.2.0/pydivkit/div/div_custom.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_data.py` & `pydivkit-30.2.0/pydivkit/div/div_data.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_default_indicator_item_placement.py` & `pydivkit-30.2.0/pydivkit/div/div_default_indicator_item_placement.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_dimension.py` & `pydivkit-30.2.0/pydivkit/div/div_dimension.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_disappear_action.py` & `pydivkit-30.2.0/pydivkit/div/div_disappear_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_download_callbacks.py` & `pydivkit-30.2.0/pydivkit/div/div_download_callbacks.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_edge_insets.py` & `pydivkit-30.2.0/pydivkit/div/div_edge_insets.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_extension.py` & `pydivkit-30.2.0/pydivkit/div/div_extension.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_fade_transition.py` & `pydivkit-30.2.0/pydivkit/div/div_fade_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_filter_rtl_mirror.py` & `pydivkit-30.2.0/pydivkit/div/div_filter_rtl_mirror.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_fixed_count.py` & `pydivkit-30.2.0/pydivkit/div/div_fixed_count.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_fixed_length_input_mask.py` & `pydivkit-30.2.0/pydivkit/div/div_fixed_length_input_mask.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_fixed_size.py` & `pydivkit-30.2.0/pydivkit/div/div_fixed_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_focus.py` & `pydivkit-30.2.0/pydivkit/div/div_focus.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_gallery.py` & `pydivkit-30.2.0/pydivkit/div/div_gallery.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_gif_image.py` & `pydivkit-30.2.0/pydivkit/div/div_gif_image.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_grid.py` & `pydivkit-30.2.0/pydivkit/div/div_grid.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_image.py` & `pydivkit-30.2.0/pydivkit/div/div_image.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_image_background.py` & `pydivkit-30.2.0/pydivkit/div/div_image_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_indicator.py` & `pydivkit-30.2.0/pydivkit/div/div_indicator.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_infinity_count.py` & `pydivkit-30.2.0/pydivkit/div/div_infinity_count.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_input.py` & `pydivkit-30.2.0/pydivkit/div/div_input.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_input_mask_base.py` & `pydivkit-30.2.0/pydivkit/div/div_input_mask_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_input_validator_base.py` & `pydivkit-30.2.0/pydivkit/div/div_input_validator_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_input_validator_expression.py` & `pydivkit-30.2.0/pydivkit/div/div_input_validator_expression.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_input_validator_regex.py` & `pydivkit-30.2.0/pydivkit/div/div_input_validator_regex.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_linear_gradient.py` & `pydivkit-30.2.0/pydivkit/div/div_linear_gradient.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_match_parent_size.py` & `pydivkit-30.2.0/pydivkit/div/div_match_parent_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_neighbour_page_size.py` & `pydivkit-30.2.0/pydivkit/div/div_neighbour_page_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_nine_patch_background.py` & `pydivkit-30.2.0/pydivkit/div/div_nine_patch_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_page_size.py` & `pydivkit-30.2.0/pydivkit/div/div_page_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_page_transformation_overlap.py` & `pydivkit-30.2.0/pydivkit/div/div_page_transformation_overlap.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_page_transformation_slide.py` & `pydivkit-30.2.0/pydivkit/div/div_page_transformation_slide.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_pager.py` & `pydivkit-30.2.0/pydivkit/div/div_pager.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_patch.py` & `pydivkit-30.2.0/pydivkit/div/div_patch.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_percentage_size.py` & `pydivkit-30.2.0/pydivkit/div/div_percentage_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_phone_input_mask.py` & `pydivkit-30.2.0/pydivkit/div/div_phone_input_mask.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_pivot_fixed.py` & `pydivkit-30.2.0/pydivkit/div/div_pivot_fixed.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_pivot_percentage.py` & `pydivkit-30.2.0/pydivkit/div/div_pivot_percentage.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_point.py` & `pydivkit-30.2.0/pydivkit/div/div_point.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_radial_gradient.py` & `pydivkit-30.2.0/pydivkit/div/div_radial_gradient.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_radial_gradient_fixed_center.py` & `pydivkit-30.2.0/pydivkit/div/div_radial_gradient_fixed_center.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_radial_gradient_relative_center.py` & `pydivkit-30.2.0/pydivkit/div/div_radial_gradient_relative_center.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_radial_gradient_relative_radius.py` & `pydivkit-30.2.0/pydivkit/div/div_radial_gradient_relative_radius.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_rounded_rectangle_shape.py` & `pydivkit-30.2.0/pydivkit/div/div_rounded_rectangle_shape.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_scale_transition.py` & `pydivkit-30.2.0/pydivkit/div/div_scale_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_select.py` & `pydivkit-30.2.0/pydivkit/div/div_select.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_separator.py` & `pydivkit-30.2.0/pydivkit/div/div_separator.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_shadow.py` & `pydivkit-30.2.0/pydivkit/div/div_shadow.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_shape_drawable.py` & `pydivkit-30.2.0/pydivkit/div/div_shape_drawable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_sight_action.py` & `pydivkit-30.2.0/pydivkit/div/div_sight_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_slide_transition.py` & `pydivkit-30.2.0/pydivkit/div/div_slide_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_slider.py` & `pydivkit-30.2.0/pydivkit/div/div_slider.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_solid_background.py` & `pydivkit-30.2.0/pydivkit/div/div_solid_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_state.py` & `pydivkit-30.2.0/pydivkit/div/div_state.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_stretch_indicator_item_placement.py` & `pydivkit-30.2.0/pydivkit/div/div_stretch_indicator_item_placement.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_stroke.py` & `pydivkit-30.2.0/pydivkit/div/div_stroke.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_tabs.py` & `pydivkit-30.2.0/pydivkit/div/div_tabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div, div_accessibility, div_action, div_alignment_horizontal,
     div_alignment_vertical, div_appearance_transition, div_background,
     div_border, div_change_transition, div_corners_radius, div_disappear_action,
-    div_edge_insets, div_extension, div_focus, div_font_weight, div_size,
-    div_size_unit, div_tooltip, div_transform, div_transition_trigger,
+    div_edge_insets, div_extension, div_fixed_size, div_focus, div_font_weight,
+    div_size, div_size_unit, div_tooltip, div_transform, div_transition_trigger,
     div_visibility, div_visibility_action,
 )
 
 
 # Tabs. Height of the first tab is determined by its contents, and height of the
 # remaining [depends on the platform](../../location#tabs).
 class DivTabs(BaseDiv):
@@ -45,14 +45,15 @@
         restrict_parent_scroll: typing.Optional[typing.Union[Expr, bool]] = None,
         row_span: typing.Optional[typing.Union[Expr, int]] = None,
         selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
         selected_tab: typing.Optional[typing.Union[Expr, int]] = None,
         separator_color: typing.Optional[typing.Union[Expr, str]] = None,
         separator_paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
         switch_tabs_by_content_swipe_enabled: typing.Optional[typing.Union[Expr, bool]] = None,
+        tab_title_delimiter: typing.Optional[DivTabsTabTitleDelimiter] = None,
         tab_title_style: typing.Optional[DivTabsTabTitleStyle] = None,
         title_paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
         tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = None,
         transform: typing.Optional[div_transform.DivTransform] = None,
         transition_change: typing.Optional[div_change_transition.DivChangeTransition] = None,
         transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
         transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
@@ -85,14 +86,15 @@
             restrict_parent_scroll=restrict_parent_scroll,
             row_span=row_span,
             selected_actions=selected_actions,
             selected_tab=selected_tab,
             separator_color=separator_color,
             separator_paddings=separator_paddings,
             switch_tabs_by_content_swipe_enabled=switch_tabs_by_content_swipe_enabled,
+            tab_title_delimiter=tab_title_delimiter,
             tab_title_style=tab_title_style,
             title_paddings=title_paddings,
             tooltips=tooltips,
             transform=transform,
             transition_change=transition_change,
             transition_in=transition_in,
             transition_out=transition_out,
@@ -229,14 +231,17 @@
             "Indents from the separating line. Not used if "
             "`has_separator = false`."
         ),
     )
     switch_tabs_by_content_swipe_enabled: typing.Optional[typing.Union[Expr, bool]] = Field(
         description="Switching tabs by scrolling through the contents.",
     )
+    tab_title_delimiter: typing.Optional[DivTabsTabTitleDelimiter] = Field(
+        description="Style of delimiters between tab titles.",
+    )
     tab_title_style: typing.Optional[DivTabsTabTitleStyle] = Field(
         description="Design style of tab titles.",
     )
     title_paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="Indents in the tab name.",
     )
     tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = Field(
@@ -324,14 +329,51 @@
         description="Action when clicking on the active tab title.",
     )
 
 
 DivTabsItem.update_forward_refs()
 
 
+# Style of delimiters between tab titles.
+class DivTabsTabTitleDelimiter(BaseDiv):
+
+    def __init__(
+        self, *,
+        height: typing.Optional[div_fixed_size.DivFixedSize] = None,
+        image_url: typing.Optional[typing.Union[Expr, str]] = None,
+        width: typing.Optional[div_fixed_size.DivFixedSize] = None,
+        **kwargs: typing.Any,
+    ):
+        super().__init__(
+            height=height,
+            image_url=image_url,
+            width=width,
+            **kwargs,
+        )
+
+    height: typing.Optional[div_fixed_size.DivFixedSize] = Field(
+        description=(
+            "Element height. For Android: if there is text in this or in "
+            "a child element,specify height in `sp` to scale the element "
+            "together with the text. To learn moreabout units of size "
+            "measurement, see [Layout inside the card](../../layout)."
+        ),
+    )
+    image_url: typing.Union[Expr, str] = Field(
+        format="uri", 
+        description="Direct URL to an image.",
+    )
+    width: typing.Optional[div_fixed_size.DivFixedSize] = Field(
+        description="Element width.",
+    )
+
+
+DivTabsTabTitleDelimiter.update_forward_refs()
+
+
 # Design style of tab titles.
 class DivTabsTabTitleStyle(BaseDiv):
 
     def __init__(
         self, *,
         active_background_color: typing.Optional[typing.Union[Expr, str]] = None,
         active_font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = None,
```

### Comparing `pydivkit-30.1.0/pydivkit/div/div_text.py` & `pydivkit-30.2.0/pydivkit/div/div_text.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_text_range_border.py` & `pydivkit-30.2.0/pydivkit/div/div_text_range_border.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_timer.py` & `pydivkit-30.2.0/pydivkit/div/div_timer.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_tooltip.py` & `pydivkit-30.2.0/pydivkit/div/div_tooltip.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_transform.py` & `pydivkit-30.2.0/pydivkit/div/div_transform.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_transition_base.py` & `pydivkit-30.2.0/pydivkit/div/div_transition_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_trigger.py` & `pydivkit-30.2.0/pydivkit/div/div_trigger.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_typed_value.py` & `pydivkit-30.2.0/pydivkit/div/div_typed_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_variable.py` & `pydivkit-30.2.0/pydivkit/div/div_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_video.py` & `pydivkit-30.2.0/pydivkit/div/div_video.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_video_source.py` & `pydivkit-30.2.0/pydivkit/div/div_video_source.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_visibility_action.py` & `pydivkit-30.2.0/pydivkit/div/div_visibility_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/div_wrap_content_size.py` & `pydivkit-30.2.0/pydivkit/div/div_wrap_content_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/integer_value.py` & `pydivkit-30.2.0/pydivkit/div/integer_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/integer_variable.py` & `pydivkit-30.2.0/pydivkit/div/integer_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/number_value.py` & `pydivkit-30.2.0/pydivkit/div/number_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/number_variable.py` & `pydivkit-30.2.0/pydivkit/div/number_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/string_value.py` & `pydivkit-30.2.0/pydivkit/div/string_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/string_variable.py` & `pydivkit-30.2.0/pydivkit/div/string_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/url_value.py` & `pydivkit-30.2.0/pydivkit/div/url_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pydivkit/div/url_variable.py` & `pydivkit-30.2.0/pydivkit/div/url_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-30.1.0/pyproject.toml` & `pydivkit-30.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydivkit"
-version = "30.1.0"
+version = "30.2.0"
 description = "DivKit python library"
 readme = "README.md"
 repository = "https://github.com/divkit/divkit/tree/main/json-builder/python"
 keywords = ["divkit", "sdk"]
 authors = [
     "Vladislav Bakaev <bakaev-vlad@yandex-team.ru>",
     "Pavel Mosein <p-mosein@yandex-team.ru>",
```

### Comparing `pydivkit-30.1.0/PKG-INFO` & `pydivkit-30.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydivkit
-Version: 30.1.0
+Version: 30.2.0
 Summary: DivKit python library
 Home-page: https://github.com/divkit/divkit/tree/main/json-builder/python
 Keywords: divkit,sdk
 Author: Vladislav Bakaev
 Author-email: bakaev-vlad@yandex-team.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

