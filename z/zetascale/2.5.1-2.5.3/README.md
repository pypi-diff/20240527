# Comparing `tmp/zetascale-2.5.1.tar.gz` & `tmp/zetascale-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zetascale-2.5.1.tar", max compression
+gzip compressed data, was "zetascale-2.5.3.tar", max compression
```

## Comparing `zetascale-2.5.1.tar` & `zetascale-2.5.3.tar`

### file list

```diff
@@ -1,388 +1,390 @@
--rw-r--r--   0        0        0    11342 2024-05-21 00:22:21.733285 zetascale-2.5.1/LICENSE
--rw-r--r--   0        0        0    20231 2024-05-21 00:22:21.733369 zetascale-2.5.1/README.md
--rw-r--r--   0        0        0     1333 2024-05-25 22:02:47.085235 zetascale-2.5.1/pyproject.toml
--rw-r--r--   0        0        0      589 2024-05-21 00:22:21.765974 zetascale-2.5.1/zeta/__init__.py
--rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766028 zetascale-2.5.1/zeta/cli/__init__.py
--rw-r--r--   0        0        0     1937 2024-05-21 00:22:21.766088 zetascale-2.5.1/zeta/cli/main.py
--rw-r--r--   0        0        0      157 2024-05-21 00:22:21.766172 zetascale-2.5.1/zeta/cloud/__init__.py
--rw-r--r--   0        0        0     2071 2024-05-21 00:22:21.766216 zetascale-2.5.1/zeta/cloud/main.py
--rw-r--r--   0        0        0     6068 2024-05-21 00:22:21.766270 zetascale-2.5.1/zeta/cloud/sky_api.py
--rw-r--r--   0        0        0       59 2024-05-21 00:22:21.766338 zetascale-2.5.1/zeta/experimental/__init__.py
--rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766382 zetascale-2.5.1/zeta/experimental/triton/__init__.py
--rw-r--r--   0        0        0     1656 2024-05-21 00:22:21.766461 zetascale-2.5.1/zeta/experimental/triton/activations/__init__.py
--rw-r--r--   0        0        0     2600 2024-05-21 00:22:21.766506 zetascale-2.5.1/zeta/experimental/triton/activations/activations.py
--rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766525 zetascale-2.5.1/zeta/experimental/triton/activations/flash_mlp.py
--rw-r--r--   0        0        0     9532 2024-05-21 00:22:21.766605 zetascale-2.5.1/zeta/experimental/triton/activations/functions.py
--rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766648 zetascale-2.5.1/zeta/experimental/triton/triton_modules/__init__.py
--rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766675 zetascale-2.5.1/zeta/experimental/triton/triton_modules/flash_mlp.py
--rw-r--r--   0        0        0     2806 2024-05-21 00:22:21.766729 zetascale-2.5.1/zeta/experimental/triton/triton_modules/linear_proj.py
--rw-r--r--   0        0        0     3311 2024-05-21 00:22:21.766804 zetascale-2.5.1/zeta/models/BEiT3.py
--rw-r--r--   0        0        0     1809 2024-05-21 00:22:21.766856 zetascale-2.5.1/zeta/models/LongNet.py
--rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766873 zetascale-2.5.1/zeta/models/Magneto.py
--rw-r--r--   0        0        0      603 2024-05-21 00:22:21.766925 zetascale-2.5.1/zeta/models/__init__.py
--rw-r--r--   0        0        0     3308 2024-05-21 00:22:21.766969 zetascale-2.5.1/zeta/models/andromeda.py
--rw-r--r--   0        0        0      135 2024-05-21 00:22:21.767013 zetascale-2.5.1/zeta/models/base.py
--rw-r--r--   0        0        0     6752 2024-05-21 00:22:21.767073 zetascale-2.5.1/zeta/models/gpt4.py
--rw-r--r--   0        0        0     4288 2024-05-21 00:22:21.767120 zetascale-2.5.1/zeta/models/kosmos.py
--rw-r--r--   0        0        0      949 2024-05-21 00:22:21.767166 zetascale-2.5.1/zeta/models/llama.py
--rw-r--r--   0        0        0     3639 2024-05-21 00:22:21.767223 zetascale-2.5.1/zeta/models/max_vit.py
--rw-r--r--   0        0        0     6678 2024-05-21 00:22:21.767283 zetascale-2.5.1/zeta/models/mega_vit.py
--rw-r--r--   0        0        0     6927 2024-05-21 00:22:21.767340 zetascale-2.5.1/zeta/models/mm_mamba.py
--rw-r--r--   0        0        0    12991 2024-05-21 00:22:21.767416 zetascale-2.5.1/zeta/models/navit.py
--rw-r--r--   0        0        0     1884 2024-05-21 00:22:21.767454 zetascale-2.5.1/zeta/models/palme.py
--rw-r--r--   0        0        0     2762 2024-05-21 00:22:21.767499 zetascale-2.5.1/zeta/models/vit.py
--rw-r--r--   0        0        0      219 2024-05-21 00:22:21.767567 zetascale-2.5.1/zeta/nn/__init__.py
--rw-r--r--   0        0        0     1895 2024-05-21 00:22:21.767637 zetascale-2.5.1/zeta/nn/attention/__init__.py
--rw-r--r--   0        0        0     4184 2024-05-21 00:22:21.767693 zetascale-2.5.1/zeta/nn/attention/agent_attn.py
--rw-r--r--   0        0        0    14876 2024-05-21 00:22:21.767772 zetascale-2.5.1/zeta/nn/attention/attend.py
--rw-r--r--   0        0        0      244 2024-05-21 00:22:21.767819 zetascale-2.5.1/zeta/nn/attention/base.py
--rw-r--r--   0        0        0     4050 2024-05-21 00:22:21.767875 zetascale-2.5.1/zeta/nn/attention/cross_attention.py
--rw-r--r--   0        0        0     3236 2024-05-21 00:22:21.767922 zetascale-2.5.1/zeta/nn/attention/cross_attn_images.py
--rw-r--r--   0        0        0    10734 2024-05-21 00:22:21.767991 zetascale-2.5.1/zeta/nn/attention/dilated_attention.py
--rw-r--r--   0        0        0     8803 2024-05-21 00:22:21.768136 zetascale-2.5.1/zeta/nn/attention/flash_attention.py
--rw-r--r--   0        0        0     2161 2024-05-21 00:22:21.768183 zetascale-2.5.1/zeta/nn/attention/linear_attention.py
--rw-r--r--   0        0        0     2370 2024-05-21 00:22:21.768231 zetascale-2.5.1/zeta/nn/attention/linear_attn_l.py
--rw-r--r--   0        0        0     2090 2024-05-21 00:37:46.889652 zetascale-2.5.1/zeta/nn/attention/linearized_attention.py
--rw-r--r--   0        0        0     9794 2024-05-21 00:22:21.768347 zetascale-2.5.1/zeta/nn/attention/local_attention.py
--rw-r--r--   0        0        0     1966 2024-05-21 00:22:21.768392 zetascale-2.5.1/zeta/nn/attention/local_attention_mha.py
--rw-r--r--   0        0        0    18990 2024-05-21 00:22:21.768470 zetascale-2.5.1/zeta/nn/attention/mixture_attention.py
--rw-r--r--   0        0        0    12414 2024-05-21 00:22:21.768567 zetascale-2.5.1/zeta/nn/attention/multi_grouped_attn.py
--rw-r--r--   0        0        0     2729 2024-05-21 00:22:21.768617 zetascale-2.5.1/zeta/nn/attention/multi_modal_causal_attention.py
--rw-r--r--   0        0        0     3879 2024-05-21 00:22:21.768670 zetascale-2.5.1/zeta/nn/attention/multi_modal_cross_attn.py
--rw-r--r--   0        0        0     5769 2024-05-21 00:22:21.768725 zetascale-2.5.1/zeta/nn/attention/multihead_attention.py
--rw-r--r--   0        0        0    25310 2024-05-21 00:37:47.151935 zetascale-2.5.1/zeta/nn/attention/multiquery_attention.py
--rw-r--r--   0        0        0     3979 2024-05-21 00:22:21.768851 zetascale-2.5.1/zeta/nn/attention/scalable_img_self_attn.py
--rw-r--r--   0        0        0     2198 2024-05-21 00:22:21.768897 zetascale-2.5.1/zeta/nn/attention/shaped_attention.py
--rw-r--r--   0        0        0     4672 2024-05-21 00:22:21.768952 zetascale-2.5.1/zeta/nn/attention/sparse_attention.py
--rw-r--r--   0        0        0     1741 2024-05-21 00:22:21.768998 zetascale-2.5.1/zeta/nn/attention/spatial_linear_attention.py
--rw-r--r--   0        0        0     2973 2024-05-21 00:22:21.769048 zetascale-2.5.1/zeta/nn/attention/xc_attention.py
--rw-r--r--   0        0        0      482 2024-05-21 00:22:21.769118 zetascale-2.5.1/zeta/nn/biases/__init__.py
--rw-r--r--   0        0        0     3951 2024-05-21 00:22:21.769171 zetascale-2.5.1/zeta/nn/biases/alibi.py
--rw-r--r--   0        0        0      245 2024-05-21 00:22:21.769209 zetascale-2.5.1/zeta/nn/biases/base.py
--rw-r--r--   0        0        0     1348 2024-05-21 00:22:21.769251 zetascale-2.5.1/zeta/nn/biases/dynamic_position_bias.py
--rw-r--r--   0        0        0     2886 2024-05-21 00:22:21.769300 zetascale-2.5.1/zeta/nn/biases/relative_position_bias.py
--rw-r--r--   0        0        0     2069 2024-05-21 00:22:21.769370 zetascale-2.5.1/zeta/nn/embeddings/__init__.py
--rw-r--r--   0        0        0     1231 2024-05-21 00:22:21.769427 zetascale-2.5.1/zeta/nn/embeddings/abc_pos_emb.py
--rw-r--r--   0        0        0      255 2024-05-21 00:22:21.769468 zetascale-2.5.1/zeta/nn/embeddings/base.py
--rw-r--r--   0        0        0      723 2024-05-21 00:22:21.769514 zetascale-2.5.1/zeta/nn/embeddings/embedding.py
--rw-r--r--   0        0        0     2509 2024-05-21 00:22:21.769562 zetascale-2.5.1/zeta/nn/embeddings/multiway_network.py
--rw-r--r--   0        0        0      358 2024-05-21 00:22:21.769604 zetascale-2.5.1/zeta/nn/embeddings/nominal_embeddings.py
--rw-r--r--   0        0        0      900 2024-05-21 00:22:21.769647 zetascale-2.5.1/zeta/nn/embeddings/patch_embedding.py
--rw-r--r--   0        0        0     3120 2024-05-21 00:22:21.769692 zetascale-2.5.1/zeta/nn/embeddings/pi.md
--rw-r--r--   0        0        0     1996 2024-05-21 00:22:21.769737 zetascale-2.5.1/zeta/nn/embeddings/positional.py
--rw-r--r--   0        0        0     2584 2024-05-21 00:22:21.769792 zetascale-2.5.1/zeta/nn/embeddings/positional_interpolation.py
--rw-r--r--   0        0        0     3021 2024-05-21 00:22:21.769839 zetascale-2.5.1/zeta/nn/embeddings/qfsp_embeddings.py
--rw-r--r--   0        0        0     1668 2024-05-21 00:22:21.769891 zetascale-2.5.1/zeta/nn/embeddings/qft_embeddings.py
--rw-r--r--   0        0        0     2250 2024-05-21 00:22:21.769967 zetascale-2.5.1/zeta/nn/embeddings/rope.py
--rw-r--r--   0        0        0     1570 2024-05-21 00:22:21.770017 zetascale-2.5.1/zeta/nn/embeddings/scaled_sinusoidal_embeddings.py
--rw-r--r--   0        0        0     2345 2024-05-21 00:22:21.770062 zetascale-2.5.1/zeta/nn/embeddings/sine_positional.py
--rw-r--r--   0        0        0     2650 2024-05-21 00:22:21.770108 zetascale-2.5.1/zeta/nn/embeddings/sinusoidal.py
--rw-r--r--   0        0        0     1810 2024-05-21 00:22:21.770156 zetascale-2.5.1/zeta/nn/embeddings/truncated_rope.py
--rw-r--r--   0        0        0     1003 2024-05-21 00:22:21.770199 zetascale-2.5.1/zeta/nn/embeddings/vis_lang_emb.py
--rw-r--r--   0        0        0     3195 2024-05-21 00:22:21.770249 zetascale-2.5.1/zeta/nn/embeddings/vision_emb.py
--rw-r--r--   0        0        0     3208 2024-05-21 00:22:21.770299 zetascale-2.5.1/zeta/nn/embeddings/xpos_relative_position.py
--rw-r--r--   0        0        0     6685 2024-05-21 00:22:21.770353 zetascale-2.5.1/zeta/nn/embeddings/yarn.py
--rw-r--r--   0        0        0     1150 2024-05-21 00:22:21.770425 zetascale-2.5.1/zeta/nn/masks/__init__.py
--rw-r--r--   0        0        0    31987 2024-05-21 00:22:21.770499 zetascale-2.5.1/zeta/nn/masks/attn_masks.py
--rw-r--r--   0        0        0     1248 2024-05-21 00:22:21.770558 zetascale-2.5.1/zeta/nn/masks/block_diagonal.py
--rw-r--r--   0        0        0    15253 2024-05-21 00:22:21.770674 zetascale-2.5.1/zeta/nn/modules/README.md
--rw-r--r--   0        0        0    14062 2024-05-25 22:02:37.978001 zetascale-2.5.1/zeta/nn/modules/__init__.py
--rw-r--r--   0        0        0     7658 2024-05-21 00:22:21.770820 zetascale-2.5.1/zeta/nn/modules/_activations.py
--rw-r--r--   0        0        0     3561 2024-05-21 00:22:21.770869 zetascale-2.5.1/zeta/nn/modules/adaptive_conv.py
--rw-r--r--   0        0        0     1572 2024-05-21 00:22:21.770917 zetascale-2.5.1/zeta/nn/modules/adaptive_layernorm.py
--rw-r--r--   0        0        0     1506 2024-05-21 00:22:21.770965 zetascale-2.5.1/zeta/nn/modules/adaptive_parameter_list.py
--rw-r--r--   0        0        0     2181 2024-05-21 00:22:21.771010 zetascale-2.5.1/zeta/nn/modules/adaptive_rmsnorm.py
--rw-r--r--   0        0        0      465 2024-05-21 00:22:21.771057 zetascale-2.5.1/zeta/nn/modules/add_norm.py
--rw-r--r--   0        0        0     1969 2024-05-21 00:22:21.771101 zetascale-2.5.1/zeta/nn/modules/alr_block.py
--rw-r--r--   0        0        0     1885 2024-05-21 00:22:21.771145 zetascale-2.5.1/zeta/nn/modules/attn.py
--rw-r--r--   0        0        0     1170 2024-05-21 00:22:21.771188 zetascale-2.5.1/zeta/nn/modules/audio_to_text.py
--rw-r--r--   0        0        0     2927 2024-05-21 00:22:21.771233 zetascale-2.5.1/zeta/nn/modules/avg_model_merger.py
--rw-r--r--   0        0        0      200 2024-05-21 00:22:21.771283 zetascale-2.5.1/zeta/nn/modules/batched_dp.py
--rw-r--r--   0        0        0     2355 2024-05-21 00:22:21.771334 zetascale-2.5.1/zeta/nn/modules/block_butterfly_mlp.py
--rw-r--r--   0        0        0    12691 2024-05-21 00:37:47.719254 zetascale-2.5.1/zeta/nn/modules/blockdiag_butterfly.py
--rw-r--r--   0        0        0      986 2024-05-21 00:22:21.771470 zetascale-2.5.1/zeta/nn/modules/chan_layer_norm.py
--rw-r--r--   0        0        0     7693 2024-05-21 00:22:21.771536 zetascale-2.5.1/zeta/nn/modules/clex.py
--rw-r--r--   0        0        0     2522 2024-05-21 00:22:21.771589 zetascale-2.5.1/zeta/nn/modules/clip_bottleneck.py
--rw-r--r--   0        0        0     1530 2024-05-21 00:22:21.771639 zetascale-2.5.1/zeta/nn/modules/cnn_text.py
--rw-r--r--   0        0        0     4281 2024-05-21 00:22:21.771705 zetascale-2.5.1/zeta/nn/modules/combined_linear.py
--rw-r--r--   0        0        0     1026 2024-05-21 00:22:21.771761 zetascale-2.5.1/zeta/nn/modules/conv_bn_relu.py
--rw-r--r--   0        0        0     2422 2024-05-21 00:37:46.940310 zetascale-2.5.1/zeta/nn/modules/conv_mlp.py
--rw-r--r--   0        0        0      888 2024-05-21 00:22:21.771867 zetascale-2.5.1/zeta/nn/modules/convnet.py
--rw-r--r--   0        0        0     1723 2024-05-21 00:22:21.771923 zetascale-2.5.1/zeta/nn/modules/cross_embed_layer.py
--rw-r--r--   0        0        0     7316 2024-05-21 00:22:21.771989 zetascale-2.5.1/zeta/nn/modules/cross_modal_reparametization.py
--rw-r--r--   0        0        0     3540 2024-05-21 00:22:21.772043 zetascale-2.5.1/zeta/nn/modules/decision_tree.py
--rw-r--r--   0        0        0     2648 2024-05-21 00:22:21.772100 zetascale-2.5.1/zeta/nn/modules/deepseek_moe.py
--rw-r--r--   0        0        0      794 2024-05-21 00:22:21.772158 zetascale-2.5.1/zeta/nn/modules/dense_connect.py
--rw-r--r--   0        0        0     2371 2024-05-21 00:22:21.772210 zetascale-2.5.1/zeta/nn/modules/diffusion.py
--rw-r--r--   0        0        0     1538 2024-05-21 00:22:21.772263 zetascale-2.5.1/zeta/nn/modules/droppath.py
--rw-r--r--   0        0        0      796 2024-05-21 00:22:21.772319 zetascale-2.5.1/zeta/nn/modules/dual_path_block.py
--rw-r--r--   0        0        0     4687 2024-05-21 00:22:21.772383 zetascale-2.5.1/zeta/nn/modules/dyna_conv.py
--rw-r--r--   0        0        0     2064 2024-05-21 00:22:21.772435 zetascale-2.5.1/zeta/nn/modules/dynamic_module.py
--rw-r--r--   0        0        0      980 2024-05-21 00:22:21.772485 zetascale-2.5.1/zeta/nn/modules/dynamic_routing_block.py
--rw-r--r--   0        0        0      786 2024-05-21 00:22:21.772538 zetascale-2.5.1/zeta/nn/modules/embedding_to_grid.py
--rw-r--r--   0        0        0    11202 2024-05-21 00:22:21.772616 zetascale-2.5.1/zeta/nn/modules/ether.py
--rw-r--r--   0        0        0     5338 2024-05-21 00:22:21.772683 zetascale-2.5.1/zeta/nn/modules/exo.py
--rw-r--r--   0        0        0       92 2024-05-21 00:22:21.772729 zetascale-2.5.1/zeta/nn/modules/expand.py
--rw-r--r--   0        0        0      888 2024-05-21 00:22:21.772777 zetascale-2.5.1/zeta/nn/modules/expand_channels.py
--rw-r--r--   0        0        0     1184 2024-05-21 00:22:21.772828 zetascale-2.5.1/zeta/nn/modules/expert.py
--rw-r--r--   0        0        0      678 2024-05-21 00:22:21.772881 zetascale-2.5.1/zeta/nn/modules/fast_text.py
--rw-r--r--   0        0        0     1004 2024-05-21 00:22:21.772931 zetascale-2.5.1/zeta/nn/modules/feedback_block.py
--rw-r--r--   0        0        0     4666 2024-05-21 00:22:21.772994 zetascale-2.5.1/zeta/nn/modules/feedforward.py
--rw-r--r--   0        0        0     4396 2024-05-21 00:22:21.773060 zetascale-2.5.1/zeta/nn/modules/feedforward_network.py
--rw-r--r--   0        0        0     3153 2024-05-21 00:22:21.773107 zetascale-2.5.1/zeta/nn/modules/film.py
--rw-r--r--   0        0        0     2607 2024-05-21 00:22:21.773167 zetascale-2.5.1/zeta/nn/modules/film_conditioning.py
--rw-r--r--   0        0        0     2657 2024-05-21 00:22:21.773220 zetascale-2.5.1/zeta/nn/modules/film_efficient_metb3.py
--rw-r--r--   0        0        0      363 2024-05-21 00:22:21.773275 zetascale-2.5.1/zeta/nn/modules/flash_conv.py
--rw-r--r--   0        0        0      817 2024-05-21 00:22:21.773327 zetascale-2.5.1/zeta/nn/modules/flatten_features.py
--rw-r--r--   0        0        0     3528 2024-05-21 00:22:21.773378 zetascale-2.5.1/zeta/nn/modules/flex_conv.py
--rw-r--r--   0        0        0     2694 2024-05-21 00:22:21.773439 zetascale-2.5.1/zeta/nn/modules/flexible_mlp.py
--rw-r--r--   0        0        0      845 2024-05-21 00:22:21.773492 zetascale-2.5.1/zeta/nn/modules/fractoral_norm.py
--rw-r--r--   0        0        0     2552 2024-05-21 00:22:21.773545 zetascale-2.5.1/zeta/nn/modules/fractorial_net.py
--rw-r--r--   0        0        0      769 2024-05-21 00:22:21.773599 zetascale-2.5.1/zeta/nn/modules/freeze_layers.py
--rw-r--r--   0        0        0     2408 2024-05-21 00:22:21.773650 zetascale-2.5.1/zeta/nn/modules/fused_dropout_add.py
--rw-r--r--   0        0        0     1223 2024-05-21 00:22:21.773701 zetascale-2.5.1/zeta/nn/modules/fused_dropout_layernom.py
--rw-r--r--   0        0        0     2268 2024-05-21 00:22:21.773755 zetascale-2.5.1/zeta/nn/modules/fused_gelu_dense.py
--rw-r--r--   0        0        0     1006 2024-05-21 00:22:21.773804 zetascale-2.5.1/zeta/nn/modules/fusion_ffn.py
--rw-r--r--   0        0        0    33392 2024-05-21 00:22:21.773904 zetascale-2.5.1/zeta/nn/modules/g_shard_moe.py
--rw-r--r--   0        0        0     1800 2024-05-25 18:14:50.721305 zetascale-2.5.1/zeta/nn/modules/gated_cnn_block.py
--rw-r--r--   0        0        0      707 2024-05-21 00:22:21.773969 zetascale-2.5.1/zeta/nn/modules/gated_residual_block.py
--rw-r--r--   0        0        0     4104 2024-05-21 00:22:21.774037 zetascale-2.5.1/zeta/nn/modules/gill_mapper.py
--rw-r--r--   0        0        0      920 2024-05-21 00:22:21.774094 zetascale-2.5.1/zeta/nn/modules/glu.py
--rw-r--r--   0        0        0     1826 2024-05-21 00:22:21.774153 zetascale-2.5.1/zeta/nn/modules/gru_gating.py
--rw-r--r--   0        0        0     2634 2024-05-21 00:22:21.774210 zetascale-2.5.1/zeta/nn/modules/h3.py
--rw-r--r--   0        0        0     2078 2024-05-21 00:22:21.774272 zetascale-2.5.1/zeta/nn/modules/hebbian.py
--rw-r--r--   0        0        0      809 2024-05-21 00:22:21.774328 zetascale-2.5.1/zeta/nn/modules/highway_layer.py
--rw-r--r--   0        0        0     3527 2024-05-21 00:22:21.774388 zetascale-2.5.1/zeta/nn/modules/image_projector.py
--rw-r--r--   0        0        0     1049 2024-05-21 00:22:21.774442 zetascale-2.5.1/zeta/nn/modules/image_to_text.py
--rw-r--r--   0        0        0     1385 2024-05-21 00:22:21.774487 zetascale-2.5.1/zeta/nn/modules/img_or_video_to_time.py
--rw-r--r--   0        0        0     1197 2024-05-21 00:22:21.774532 zetascale-2.5.1/zeta/nn/modules/img_patch_embed.py
--rw-r--r--   0        0        0      763 2024-05-21 00:22:21.774576 zetascale-2.5.1/zeta/nn/modules/img_reshape.py
--rw-r--r--   0        0        0     4024 2024-05-21 00:22:21.774623 zetascale-2.5.1/zeta/nn/modules/itca.py
--rw-r--r--   0        0        0    12420 2024-05-21 00:22:21.774693 zetascale-2.5.1/zeta/nn/modules/kan.py
--rw-r--r--   0        0        0     4656 2024-05-21 00:22:21.774746 zetascale-2.5.1/zeta/nn/modules/kv_cache.py
--rw-r--r--   0        0        0     2586 2024-05-21 00:22:21.774792 zetascale-2.5.1/zeta/nn/modules/kv_cache_update.py
--rw-r--r--   0        0        0     6221 2024-05-21 00:22:21.774846 zetascale-2.5.1/zeta/nn/modules/lambda_mask.py
--rw-r--r--   0        0        0     3504 2024-05-21 00:22:21.774895 zetascale-2.5.1/zeta/nn/modules/lang_conv_module.py
--rw-r--r--   0        0        0     2760 2024-05-21 00:22:21.774942 zetascale-2.5.1/zeta/nn/modules/laser.py
--rw-r--r--   0        0        0      919 2024-05-21 00:22:21.774987 zetascale-2.5.1/zeta/nn/modules/layer_scale.py
--rw-r--r--   0        0        0     2379 2024-05-21 00:22:21.775034 zetascale-2.5.1/zeta/nn/modules/layernorm.py
--rw-r--r--   0        0        0     1132 2024-05-21 00:22:21.775081 zetascale-2.5.1/zeta/nn/modules/leaky_relu.py
--rw-r--r--   0        0        0    24514 2024-05-21 00:22:21.775141 zetascale-2.5.1/zeta/nn/modules/log_ff.py
--rw-r--r--   0        0        0     1747 2024-05-21 00:22:21.775199 zetascale-2.5.1/zeta/nn/modules/lora.py
--rw-r--r--   0        0        0     3240 2024-05-21 00:22:21.775247 zetascale-2.5.1/zeta/nn/modules/matrix.py
--rw-r--r--   0        0        0     2993 2024-05-21 00:22:21.775291 zetascale-2.5.1/zeta/nn/modules/mbconv.py
--rw-r--r--   0        0        0     3127 2024-05-21 00:22:21.775334 zetascale-2.5.1/zeta/nn/modules/mixtape.py
--rw-r--r--   0        0        0     2125 2024-05-21 00:22:21.775378 zetascale-2.5.1/zeta/nn/modules/mixtral_expert.py
--rw-r--r--   0        0        0     1884 2024-05-21 00:22:21.775424 zetascale-2.5.1/zeta/nn/modules/mlp.py
--rw-r--r--   0        0        0     3729 2024-05-21 00:22:21.775471 zetascale-2.5.1/zeta/nn/modules/mlp_mixer.py
--rw-r--r--   0        0        0     2435 2024-05-21 00:22:21.775520 zetascale-2.5.1/zeta/nn/modules/mm_adapter.py
--rw-r--r--   0        0        0       87 2024-05-21 00:22:21.775561 zetascale-2.5.1/zeta/nn/modules/mm_fusion.py
--rw-r--r--   0        0        0     2340 2024-05-21 00:22:21.775609 zetascale-2.5.1/zeta/nn/modules/mm_layernorm.py
--rw-r--r--   0        0        0     1405 2024-05-21 00:22:21.775649 zetascale-2.5.1/zeta/nn/modules/mm_ops.py
--rw-r--r--   0        0        0     6234 2024-05-21 00:22:21.775711 zetascale-2.5.1/zeta/nn/modules/modality_adaptive_module.py
--rw-r--r--   0        0        0     2930 2024-05-21 00:22:21.775756 zetascale-2.5.1/zeta/nn/modules/moe.py
--rw-r--r--   0        0        0     3228 2024-05-21 00:22:21.775806 zetascale-2.5.1/zeta/nn/modules/moe_router.py
--rw-r--r--   0        0        0      776 2024-05-21 00:22:21.775853 zetascale-2.5.1/zeta/nn/modules/monarch_mlp.py
--rw-r--r--   0        0        0     1564 2024-05-21 00:22:21.775900 zetascale-2.5.1/zeta/nn/modules/mr_adapter.py
--rw-r--r--   0        0        0     6686 2024-05-21 00:22:21.775960 zetascale-2.5.1/zeta/nn/modules/multi_input_multi_output.py
--rw-r--r--   0        0        0      837 2024-05-21 00:22:21.776004 zetascale-2.5.1/zeta/nn/modules/multi_scale_block.py
--rw-r--r--   0        0        0        2 2024-05-21 00:22:21.776046 zetascale-2.5.1/zeta/nn/modules/multiclass_label.py
--rw-r--r--   0        0        0      225 2024-05-21 00:22:21.776089 zetascale-2.5.1/zeta/nn/modules/multimodal_concat.py
--rw-r--r--   0        0        0      472 2024-05-21 00:22:21.776130 zetascale-2.5.1/zeta/nn/modules/nearest_upsample.py
--rw-r--r--   0        0        0     8309 2024-05-21 00:22:21.776199 zetascale-2.5.1/zeta/nn/modules/nebula.py
--rw-r--r--   0        0        0     2590 2024-05-21 00:22:21.776249 zetascale-2.5.1/zeta/nn/modules/nfn_stem.py
--rw-r--r--   0        0        0     1456 2024-05-21 00:22:21.776295 zetascale-2.5.1/zeta/nn/modules/norm_fractorals.py
--rw-r--r--   0        0        0     2034 2024-05-21 00:22:21.776341 zetascale-2.5.1/zeta/nn/modules/norm_utils.py
--rw-r--r--   0        0        0     2842 2024-05-21 00:22:21.776388 zetascale-2.5.1/zeta/nn/modules/omnimodal_fusion.py
--rw-r--r--   0        0        0     3851 2024-05-21 00:22:21.776438 zetascale-2.5.1/zeta/nn/modules/p_scan.py
--rw-r--r--   0        0        0     2571 2024-05-21 00:22:21.776486 zetascale-2.5.1/zeta/nn/modules/palo_ldp.py
--rw-r--r--   0        0        0      601 2024-05-21 00:22:21.776528 zetascale-2.5.1/zeta/nn/modules/parallel_wrapper.py
--rw-r--r--   0        0        0      200 2024-05-21 00:22:21.776570 zetascale-2.5.1/zeta/nn/modules/patch_img.py
--rw-r--r--   0        0        0     6597 2024-05-21 00:22:21.776626 zetascale-2.5.1/zeta/nn/modules/patch_linear_flatten.py
--rw-r--r--   0        0        0      985 2024-05-21 00:22:21.776673 zetascale-2.5.1/zeta/nn/modules/patch_video.py
--rw-r--r--   0        0        0      783 2024-05-21 00:22:21.776716 zetascale-2.5.1/zeta/nn/modules/peg.py
--rw-r--r--   0        0        0     3180 2024-05-21 00:22:21.776764 zetascale-2.5.1/zeta/nn/modules/perceiver_layer.py
--rw-r--r--   0        0        0     6115 2024-05-21 00:22:21.776830 zetascale-2.5.1/zeta/nn/modules/perceiver_resampler.py
--rw-r--r--   0        0        0     2594 2024-05-21 00:22:21.776877 zetascale-2.5.1/zeta/nn/modules/pixel_shuffling.py
--rw-r--r--   0        0        0     1692 2024-05-21 00:22:21.776921 zetascale-2.5.1/zeta/nn/modules/poly_expert_fusion_network.py
--rw-r--r--   0        0        0     2045 2024-05-21 00:22:21.776970 zetascale-2.5.1/zeta/nn/modules/polymorphic_activation.py
--rw-r--r--   0        0        0     5804 2024-05-21 00:22:21.777026 zetascale-2.5.1/zeta/nn/modules/polymorphic_neuron.py
--rw-r--r--   0        0        0      527 2024-05-21 00:22:21.777070 zetascale-2.5.1/zeta/nn/modules/prenorm.py
--rw-r--r--   0        0        0     1299 2024-05-21 00:22:21.777113 zetascale-2.5.1/zeta/nn/modules/proj_then_softmax.py
--rw-r--r--   0        0        0     7164 2024-05-21 00:22:21.777170 zetascale-2.5.1/zeta/nn/modules/pulsar.py
--rw-r--r--   0        0        0     3451 2024-05-21 00:22:21.777217 zetascale-2.5.1/zeta/nn/modules/pyro.py
--rw-r--r--   0        0        0     9454 2024-05-21 00:22:21.777284 zetascale-2.5.1/zeta/nn/modules/qformer.py
--rw-r--r--   0        0        0      812 2024-05-21 00:22:21.777328 zetascale-2.5.1/zeta/nn/modules/qkv_norm.py
--rw-r--r--   0        0        0     1381 2024-05-21 00:22:21.777374 zetascale-2.5.1/zeta/nn/modules/quantized_layernorm.py
--rw-r--r--   0        0        0      983 2024-05-21 00:22:21.777417 zetascale-2.5.1/zeta/nn/modules/query_proposal.py
--rw-r--r--   0        0        0     1152 2024-05-21 00:22:21.777463 zetascale-2.5.1/zeta/nn/modules/recurrent_model.py
--rw-r--r--   0        0        0      903 2024-05-21 00:22:21.777512 zetascale-2.5.1/zeta/nn/modules/recursive_block.py
--rw-r--r--   0        0        0      369 2024-05-21 00:22:21.777555 zetascale-2.5.1/zeta/nn/modules/relu_squared.py
--rw-r--r--   0        0        0     5037 2024-05-21 00:22:21.777610 zetascale-2.5.1/zeta/nn/modules/res_net.py
--rw-r--r--   0        0        0      492 2024-05-21 00:22:21.777667 zetascale-2.5.1/zeta/nn/modules/residual.py
--rw-r--r--   0        0        0     2238 2024-05-21 00:22:21.777714 zetascale-2.5.1/zeta/nn/modules/resnet.py
--rw-r--r--   0        0        0     5349 2024-05-21 00:22:21.777769 zetascale-2.5.1/zeta/nn/modules/return_loss_text.py
--rw-r--r--   0        0        0      829 2024-05-21 00:22:21.777812 zetascale-2.5.1/zeta/nn/modules/rms_norm.py
--rw-r--r--   0        0        0     1646 2024-05-21 00:22:21.777856 zetascale-2.5.1/zeta/nn/modules/rnn_nlp.py
--rw-r--r--   0        0        0     3106 2024-05-21 00:22:21.777902 zetascale-2.5.1/zeta/nn/modules/s4.py
--rw-r--r--   0        0        0      818 2024-05-21 00:22:21.777947 zetascale-2.5.1/zeta/nn/modules/scale.py
--rw-r--r--   0        0        0      882 2024-05-21 00:22:21.777993 zetascale-2.5.1/zeta/nn/modules/scale_norm.py
--rw-r--r--   0        0        0     1433 2024-05-21 00:22:21.778037 zetascale-2.5.1/zeta/nn/modules/scaled_sinusoidal.py
--rw-r--r--   0        0        0      799 2024-05-21 00:22:21.778086 zetascale-2.5.1/zeta/nn/modules/scalenorm.py
--rw-r--r--   0        0        0     1858 2024-05-21 00:22:21.778139 zetascale-2.5.1/zeta/nn/modules/shift_tokens.py
--rw-r--r--   0        0        0     2877 2024-05-21 00:22:21.778185 zetascale-2.5.1/zeta/nn/modules/shufflenet.py
--rw-r--r--   0        0        0     8939 2024-05-21 00:22:21.778249 zetascale-2.5.1/zeta/nn/modules/sig_lip.py
--rw-r--r--   0        0        0     2659 2024-05-25 16:41:31.796497 zetascale-2.5.1/zeta/nn/modules/sig_lip_loss.py
--rw-r--r--   0        0        0      283 2024-05-21 00:22:21.778291 zetascale-2.5.1/zeta/nn/modules/simple_attention.py
--rw-r--r--   0        0        0      692 2024-05-21 00:22:21.778338 zetascale-2.5.1/zeta/nn/modules/simple_feedforward.py
--rw-r--r--   0        0        0     9719 2024-05-21 00:22:21.778406 zetascale-2.5.1/zeta/nn/modules/simple_mamba.py
--rw-r--r--   0        0        0      764 2024-05-21 00:22:21.778454 zetascale-2.5.1/zeta/nn/modules/simple_res_block.py
--rw-r--r--   0        0        0      978 2024-05-21 00:22:21.778496 zetascale-2.5.1/zeta/nn/modules/simple_resblock.py
--rw-r--r--   0        0        0      638 2024-05-21 00:22:21.778535 zetascale-2.5.1/zeta/nn/modules/simple_rmsnorm.py
--rw-r--r--   0        0        0      509 2024-05-21 00:22:21.778579 zetascale-2.5.1/zeta/nn/modules/skip_connect.py
--rw-r--r--   0        0        0     1194 2024-05-21 00:22:21.778621 zetascale-2.5.1/zeta/nn/modules/skipconnection.py
--rw-r--r--   0        0        0     3553 2024-05-21 00:22:21.778668 zetascale-2.5.1/zeta/nn/modules/slerp_model_merger.py
--rw-r--r--   0        0        0      765 2024-05-21 00:22:21.778715 zetascale-2.5.1/zeta/nn/modules/sp_act.py
--rw-r--r--   0        0        0    22085 2024-05-25 18:14:50.844937 zetascale-2.5.1/zeta/nn/modules/space_time_unet.py
--rw-r--r--   0        0        0     1346 2024-05-21 00:22:21.778853 zetascale-2.5.1/zeta/nn/modules/spacial_transformer.py
--rw-r--r--   0        0        0     4976 2024-05-21 00:22:21.778909 zetascale-2.5.1/zeta/nn/modules/sparq_attn.py
--rw-r--r--   0        0        0    13915 2024-05-21 00:22:21.778984 zetascale-2.5.1/zeta/nn/modules/sparse_moe.py
--rw-r--r--   0        0        0     7355 2024-05-25 22:02:37.956419 zetascale-2.5.1/zeta/nn/modules/sparse_token_integration.py
--rw-r--r--   0        0        0     2021 2024-05-21 00:22:21.779039 zetascale-2.5.1/zeta/nn/modules/spatial_downsample.py
--rw-r--r--   0        0        0     1346 2024-05-21 00:22:21.779080 zetascale-2.5.1/zeta/nn/modules/spatial_transformer.py
--rw-r--r--   0        0        0     5006 2024-05-21 00:22:21.779136 zetascale-2.5.1/zeta/nn/modules/splines.py
--rw-r--r--   0        0        0     1041 2024-05-21 00:22:21.779183 zetascale-2.5.1/zeta/nn/modules/squeeze_excitation.py
--rw-r--r--   0        0        0     4334 2024-05-21 00:22:21.779242 zetascale-2.5.1/zeta/nn/modules/ssm.py
--rw-r--r--   0        0        0     7305 2024-05-21 00:22:21.779306 zetascale-2.5.1/zeta/nn/modules/ssm_language.py
--rw-r--r--   0        0        0      942 2024-05-21 00:22:21.779348 zetascale-2.5.1/zeta/nn/modules/stoch_depth.py
--rw-r--r--   0        0        0      958 2024-05-21 00:22:21.779389 zetascale-2.5.1/zeta/nn/modules/stochastic_depth.py
--rw-r--r--   0        0        0     2032 2024-05-21 00:22:21.779434 zetascale-2.5.1/zeta/nn/modules/subln.py
--rw-r--r--   0        0        0      972 2024-05-21 00:22:21.779478 zetascale-2.5.1/zeta/nn/modules/super_resolution.py
--rw-r--r--   0        0        0     5610 2024-05-21 00:37:47.055302 zetascale-2.5.1/zeta/nn/modules/swarmalator.py
--rw-r--r--   0        0        0     1313 2024-05-21 00:22:21.779579 zetascale-2.5.1/zeta/nn/modules/swiglu.py
--rw-r--r--   0        0        0      715 2024-05-21 00:22:21.779623 zetascale-2.5.1/zeta/nn/modules/tensor.py
--rw-r--r--   0        0        0      865 2024-05-21 00:22:21.779670 zetascale-2.5.1/zeta/nn/modules/tensor_to_int.py
--rw-r--r--   0        0        0     3281 2024-05-21 00:22:21.779722 zetascale-2.5.1/zeta/nn/modules/text_scene_fusion.py
--rw-r--r--   0        0        0     2692 2024-05-21 00:22:21.779769 zetascale-2.5.1/zeta/nn/modules/text_video_fuse.py
--rw-r--r--   0        0        0     2104 2024-05-21 00:22:21.779825 zetascale-2.5.1/zeta/nn/modules/time_up_sample.py
--rw-r--r--   0        0        0      631 2024-05-21 00:22:21.779868 zetascale-2.5.1/zeta/nn/modules/to_logits.py
--rw-r--r--   0        0        0     2158 2024-05-21 00:22:21.779914 zetascale-2.5.1/zeta/nn/modules/token_learner.py
--rw-r--r--   0        0        0     1075 2024-05-21 00:22:21.779962 zetascale-2.5.1/zeta/nn/modules/token_mixer.py
--rw-r--r--   0        0        0      189 2024-05-21 00:22:21.780004 zetascale-2.5.1/zeta/nn/modules/token_shift.py
--rw-r--r--   0        0        0    10310 2024-05-21 00:22:21.780074 zetascale-2.5.1/zeta/nn/modules/top_n_gating.py
--rw-r--r--   0        0        0     4363 2024-05-21 00:22:21.780127 zetascale-2.5.1/zeta/nn/modules/transformations.py
--rw-r--r--   0        0        0      921 2024-05-21 00:22:21.780175 zetascale-2.5.1/zeta/nn/modules/triple_skip.py
--rw-r--r--   0        0        0     2193 2024-05-21 00:22:21.780221 zetascale-2.5.1/zeta/nn/modules/triton_rmsnorm.py
--rw-r--r--   0        0        0     4112 2024-05-21 00:22:21.780276 zetascale-2.5.1/zeta/nn/modules/u_mamba.py
--rw-r--r--   0        0        0     4717 2024-05-21 00:22:21.780330 zetascale-2.5.1/zeta/nn/modules/unet.py
--rw-r--r--   0        0        0      974 2024-05-21 00:22:21.780381 zetascale-2.5.1/zeta/nn/modules/v_layernorm.py
--rw-r--r--   0        0        0     1686 2024-05-21 00:22:21.780429 zetascale-2.5.1/zeta/nn/modules/v_pool.py
--rw-r--r--   0        0        0     2809 2024-05-21 00:22:21.780472 zetascale-2.5.1/zeta/nn/modules/video_autoencoder.py
--rw-r--r--   0        0        0     9239 2024-05-21 00:22:21.780539 zetascale-2.5.1/zeta/nn/modules/video_diffusion_modules.py
--rw-r--r--   0        0        0     1497 2024-05-21 00:22:21.780583 zetascale-2.5.1/zeta/nn/modules/video_to_tensor.py
--rw-r--r--   0        0        0     1067 2024-05-21 00:22:21.780629 zetascale-2.5.1/zeta/nn/modules/video_to_text.py
--rw-r--r--   0        0        0     2702 2024-05-21 00:22:21.780681 zetascale-2.5.1/zeta/nn/modules/vision_mamba.py
--rw-r--r--   0        0        0     2018 2024-05-21 00:22:21.780733 zetascale-2.5.1/zeta/nn/modules/vision_weighted_permute_mlp.py
--rw-r--r--   0        0        0     5445 2024-05-21 00:22:21.780804 zetascale-2.5.1/zeta/nn/modules/visual_expert.py
--rw-r--r--   0        0        0     6103 2024-05-25 18:23:29.115939 zetascale-2.5.1/zeta/nn/modules/vit_denoiser.py
--rw-r--r--   0        0        0     3099 2024-05-21 00:22:21.780910 zetascale-2.5.1/zeta/nn/modules/vss_block.py
--rw-r--r--   0        0        0     2775 2024-05-21 00:22:21.780963 zetascale-2.5.1/zeta/nn/modules/ws_conv2d.py
--rw-r--r--   0        0        0       86 2024-05-21 00:22:21.781034 zetascale-2.5.1/zeta/nn/modules/xmoe/__init__.py
--rw-r--r--   0        0        0     2351 2024-05-21 00:22:21.781081 zetascale-2.5.1/zeta/nn/modules/xmoe/global_groups.py
--rw-r--r--   0        0        0    12458 2024-05-21 00:22:21.781157 zetascale-2.5.1/zeta/nn/modules/xmoe/moe_layer.py
--rw-r--r--   0        0        0    18694 2024-05-21 00:22:21.781205 zetascale-2.5.1/zeta/nn/modules/xmoe/routing.py
--rw-r--r--   0        0        0     2302 2024-05-21 00:22:21.781262 zetascale-2.5.1/zeta/nn/modules/yolo.py
--rw-r--r--   0        0        0     2595 2024-05-21 00:22:21.781338 zetascale-2.5.1/zeta/ops/__Init__.py
--rw-r--r--   0        0        0      287 2024-05-21 00:22:21.781384 zetascale-2.5.1/zeta/ops/absmax.py
--rw-r--r--   0        0        0     2652 2024-05-21 00:22:21.781432 zetascale-2.5.1/zeta/ops/async_softmax.py
--rw-r--r--   0        0        0     2054 2024-05-21 00:22:21.781475 zetascale-2.5.1/zeta/ops/dilated_attn_ops.py
--rw-r--r--   0        0        0     2017 2024-05-21 00:22:21.781530 zetascale-2.5.1/zeta/ops/einops_from_to.py
--rw-r--r--   0        0        0     1876 2024-05-21 00:22:21.781580 zetascale-2.5.1/zeta/ops/einops_poly.py
--rw-r--r--   0        0        0     2150 2024-05-21 00:22:21.781631 zetascale-2.5.1/zeta/ops/expand.py
--rw-r--r--   0        0        0     1262 2024-05-21 00:22:21.781685 zetascale-2.5.1/zeta/ops/laplace.py
--rw-r--r--   0        0        0    16114 2024-05-21 00:37:47.171297 zetascale-2.5.1/zeta/ops/main.py
--rw-r--r--   0        0        0     1392 2024-05-21 00:22:21.781830 zetascale-2.5.1/zeta/ops/misc_act.py
--rw-r--r--   0        0        0     1671 2024-05-21 00:22:21.781882 zetascale-2.5.1/zeta/ops/mm_rearranges.py
--rw-r--r--   0        0        0      996 2024-05-21 00:22:21.781933 zetascale-2.5.1/zeta/ops/mm_softmax.py
--rw-r--r--   0        0        0     1851 2024-05-21 00:22:21.781984 zetascale-2.5.1/zeta/ops/mos.py
--rw-r--r--   0        0        0      995 2024-05-21 00:22:21.782043 zetascale-2.5.1/zeta/ops/nonlinear.py
--rw-r--r--   0        0        0     5070 2024-05-21 00:22:21.782115 zetascale-2.5.1/zeta/ops/softmax.py
--rw-r--r--   0        0        0     1086 2024-05-21 00:22:21.782171 zetascale-2.5.1/zeta/ops/sparsemax.py
--rw-r--r--   0        0        0      453 2024-05-21 00:22:21.782225 zetascale-2.5.1/zeta/ops/unitwise_norm.py
--rw-r--r--   0        0        0      814 2024-05-21 00:22:21.782317 zetascale-2.5.1/zeta/optim/__init__.py
--rw-r--r--   0        0        0    41040 2024-05-21 00:37:47.266975 zetascale-2.5.1/zeta/optim/batched_optimizer.py
--rw-r--r--   0        0        0    10142 2024-05-21 00:22:21.782511 zetascale-2.5.1/zeta/optim/decoupled_lion.py
--rw-r--r--   0        0        0     6448 2024-05-21 00:22:21.782568 zetascale-2.5.1/zeta/optim/decoupled_optimizer.py
--rw-r--r--   0        0        0    12445 2024-05-21 00:22:21.782643 zetascale-2.5.1/zeta/optim/decoupled_sophia.py
--rw-r--r--   0        0        0     4709 2024-05-21 00:22:21.782696 zetascale-2.5.1/zeta/optim/gradient_ascent.py
--rw-r--r--   0        0        0     2752 2024-05-21 00:22:21.782748 zetascale-2.5.1/zeta/optim/gradient_equillibrum.py
--rw-r--r--   0        0        0    19017 2024-05-21 00:22:21.782817 zetascale-2.5.1/zeta/optim/lion8b.py
--rw-r--r--   0        0        0     3387 2024-05-21 00:22:21.782876 zetascale-2.5.1/zeta/optim/parallel_gradient_descent.py
--rw-r--r--   0        0        0     4456 2024-05-21 00:37:47.112761 zetascale-2.5.1/zeta/optim/stable_adam.py
--rw-r--r--   0        0        0      453 2024-05-21 00:22:21.782994 zetascale-2.5.1/zeta/quant/__init__.py
--rw-r--r--   0        0        0      405 2024-05-21 00:22:21.783040 zetascale-2.5.1/zeta/quant/absmax.py
--rw-r--r--   0        0        0     2098 2024-05-21 00:22:21.783091 zetascale-2.5.1/zeta/quant/bitlinear.py
--rw-r--r--   0        0        0     1947 2024-05-21 00:22:21.783141 zetascale-2.5.1/zeta/quant/half_bit_linear.py
--rw-r--r--   0        0        0    10942 2024-05-21 00:22:21.783220 zetascale-2.5.1/zeta/quant/lfq.py
--rw-r--r--   0        0        0     3126 2024-05-21 00:22:21.783269 zetascale-2.5.1/zeta/quant/niva.py
--rw-r--r--   0        0        0    25173 2024-05-21 00:22:21.783337 zetascale-2.5.1/zeta/quant/qlora.py
--rw-r--r--   0        0        0     6010 2024-05-21 00:22:21.783405 zetascale-2.5.1/zeta/quant/qmoe.py
--rw-r--r--   0        0        0     3785 2024-05-21 00:22:21.783451 zetascale-2.5.1/zeta/quant/quick.py
--rw-r--r--   0        0        0        0 2024-05-21 00:22:21.783469 zetascale-2.5.1/zeta/quant/random_proj_quan.py
--rw-r--r--   0        0        0     1602 2024-05-21 00:22:21.783524 zetascale-2.5.1/zeta/quant/residual_vq.py
--rw-r--r--   0        0        0     1547 2024-05-21 00:22:21.783574 zetascale-2.5.1/zeta/quant/ste.py
--rw-r--r--   0        0        0      522 2024-05-21 00:22:21.783655 zetascale-2.5.1/zeta/rl/__init__.py
--rw-r--r--   0        0        0     4286 2024-05-21 00:22:21.783724 zetascale-2.5.1/zeta/rl/actor_critic.py
--rw-r--r--   0        0        0     2509 2024-05-21 00:22:21.783780 zetascale-2.5.1/zeta/rl/dpo.py
--rw-r--r--   0        0        0     3381 2024-05-21 00:22:21.783837 zetascale-2.5.1/zeta/rl/hindsight_replay.py
--rw-r--r--   0        0        0     2033 2024-05-21 00:22:21.783886 zetascale-2.5.1/zeta/rl/language_reward.py
--rw-r--r--   0        0        0     4130 2024-05-21 00:22:21.783936 zetascale-2.5.1/zeta/rl/ppo.py
--rw-r--r--   0        0        0     4513 2024-05-21 00:22:21.784007 zetascale-2.5.1/zeta/rl/priortized_replay_buffer.py
--rw-r--r--   0        0        0     5765 2024-05-21 00:22:21.784062 zetascale-2.5.1/zeta/rl/priortized_rps.py
--rw-r--r--   0        0        0      128 2024-05-21 00:22:21.784116 zetascale-2.5.1/zeta/rl/rest.py
--rw-r--r--   0        0        0     4585 2024-05-21 00:22:21.784178 zetascale-2.5.1/zeta/rl/reward_model.py
--rw-r--r--   0        0        0     2987 2024-05-21 00:22:21.784233 zetascale-2.5.1/zeta/rl/sumtree.py
--rw-r--r--   0        0        0     3185 2024-05-21 00:22:21.784290 zetascale-2.5.1/zeta/rl/vision_model_rl.py
--rw-r--r--   0        0        0     1227 2024-05-21 00:22:21.784375 zetascale-2.5.1/zeta/structs/__init__.py
--rw-r--r--   0        0        0    11731 2024-05-21 00:22:21.784455 zetascale-2.5.1/zeta/structs/auto_regressive_wrapper.py
--rw-r--r--   0        0        0     3505 2024-05-21 00:22:21.784512 zetascale-2.5.1/zeta/structs/clip_encoder.py
--rw-r--r--   0        0        0     6600 2024-05-21 00:22:21.784570 zetascale-2.5.1/zeta/structs/efficient_net.py
--rw-r--r--   0        0        0     3219 2024-05-21 00:22:21.784620 zetascale-2.5.1/zeta/structs/encoder_decoder.py
--rw-r--r--   0        0        0    28639 2024-05-21 00:22:21.784698 zetascale-2.5.1/zeta/structs/hierarchical_transformer.py
--rw-r--r--   0        0        0     5946 2024-05-21 00:22:21.784771 zetascale-2.5.1/zeta/structs/local_transformer.py
--rw-r--r--   0        0        0     1665 2024-05-21 00:22:21.784824 zetascale-2.5.1/zeta/structs/multi_modal_projector.py
--rw-r--r--   0        0        0    10839 2024-05-21 00:22:21.784890 zetascale-2.5.1/zeta/structs/simple_transformer.py
--rw-r--r--   0        0        0     2468 2024-05-21 00:22:21.784940 zetascale-2.5.1/zeta/structs/simple_vision_encoder.py
--rw-r--r--   0        0        0    68945 2024-05-21 00:22:21.785012 zetascale-2.5.1/zeta/structs/transformer.py
--rw-r--r--   0        0        0     4490 2024-05-21 00:22:21.785085 zetascale-2.5.1/zeta/structs/transformer_block.py
--rw-r--r--   0        0        0      485 2024-05-21 00:22:21.785165 zetascale-2.5.1/zeta/tokenizers/__init__.py
--rw-r--r--   0        0        0     1438 2024-05-21 00:22:21.785219 zetascale-2.5.1/zeta/tokenizers/gptx_tokenizer.py
--rw-r--r--   0        0        0     3079 2024-05-21 00:22:21.785272 zetascale-2.5.1/zeta/tokenizers/llama_sentencepiece.py
--rw-r--r--   0        0        0     3651 2024-05-21 00:22:21.785332 zetascale-2.5.1/zeta/tokenizers/multi_modal_tokenizer.py
--rw-r--r--   0        0        0     3720 2024-05-21 00:22:21.785394 zetascale-2.5.1/zeta/tokenizers/sentence_piece.py
--rw-r--r--   0        0        0     9771 2024-05-21 00:22:21.785468 zetascale-2.5.1/zeta/tokenizers/tokenmonster.py
--rw-r--r--   0        0        0      460 2024-05-21 00:22:21.785556 zetascale-2.5.1/zeta/training/__init__.py
--rw-r--r--   0        0        0     5400 2024-05-21 00:22:21.785622 zetascale-2.5.1/zeta/training/activation_checkpoint.py
--rw-r--r--   0        0        0     2576 2024-05-21 00:22:21.785674 zetascale-2.5.1/zeta/training/dataloader.py
--rw-r--r--   0        0        0     3496 2024-05-21 00:22:21.785729 zetascale-2.5.1/zeta/training/fsdp.py
--rw-r--r--   0        0        0     3186 2024-05-21 00:22:21.785785 zetascale-2.5.1/zeta/training/galore.py
--rw-r--r--   0        0        0     6054 2024-05-21 00:22:21.785852 zetascale-2.5.1/zeta/training/hive_trainer.py
--rw-r--r--   0        0        0     1626 2024-05-21 00:22:21.785901 zetascale-2.5.1/zeta/training/parallel_wrapper.py
--rw-r--r--   0        0        0     2076 2024-05-21 00:37:47.158519 zetascale-2.5.1/zeta/training/scheduler.py
--rw-r--r--   0        0        0     9273 2024-05-21 00:22:21.786034 zetascale-2.5.1/zeta/training/train.py
--rw-r--r--   0        0        0     2347 2024-05-21 00:22:21.786126 zetascale-2.5.1/zeta/utils/__init__.py
--rw-r--r--   0        0        0     3464 2024-05-21 00:22:21.786186 zetascale-2.5.1/zeta/utils/benchmark.py
--rw-r--r--   0        0        0     1347 2024-05-21 00:22:21.786243 zetascale-2.5.1/zeta/utils/cuda_memory_wrapper.py
--rw-r--r--   0        0        0     6424 2024-05-21 00:22:21.786310 zetascale-2.5.1/zeta/utils/cuda_wrapper.py
--rw-r--r--   0        0        0     1337 2024-05-21 00:22:21.786368 zetascale-2.5.1/zeta/utils/disable_logging.py
--rw-r--r--   0        0        0     1184 2024-05-21 00:22:21.786416 zetascale-2.5.1/zeta/utils/enforce_types.py
--rw-r--r--   0        0        0     1110 2024-05-21 00:22:21.786470 zetascale-2.5.1/zeta/utils/img_to_tensor.py
--rw-r--r--   0        0        0     2953 2024-05-21 00:22:21.786528 zetascale-2.5.1/zeta/utils/log_pytorch_op.py
--rw-r--r--   0        0        0    19874 2024-05-21 00:22:21.786616 zetascale-2.5.1/zeta/utils/main.py
--rw-r--r--   0        0        0     1798 2024-05-21 00:22:21.786682 zetascale-2.5.1/zeta/utils/module_device.py
--rw-r--r--   0        0        0      703 2024-05-21 00:22:21.786733 zetascale-2.5.1/zeta/utils/params.py
--rw-r--r--   0        0        0     3966 2024-05-21 00:22:21.786789 zetascale-2.5.1/zeta/utils/save_load_wrapper.py
--rw-r--r--   0        0        0      846 2024-05-21 00:22:21.786844 zetascale-2.5.1/zeta/utils/text_to_tensor.py
--rw-r--r--   0        0        0      751 2024-05-21 00:22:21.786904 zetascale-2.5.1/zeta/utils/verbose_execution.py
--rw-r--r--   0        0        0    25931 2024-05-21 00:22:21.786981 zetascale-2.5.1/zeta/utils/vision_utils.py
--rw-r--r--   0        0        0    21443 1970-01-01 00:00:00.000000 zetascale-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11342 2024-05-21 00:22:21.733285 zetascale-2.5.3/LICENSE
+-rw-r--r--   0        0        0    20231 2024-05-21 00:22:21.733369 zetascale-2.5.3/README.md
+-rw-r--r--   0        0        0     1317 2024-05-27 00:58:33.365882 zetascale-2.5.3/pyproject.toml
+-rw-r--r--   0        0        0      589 2024-05-21 00:22:21.765974 zetascale-2.5.3/zeta/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766028 zetascale-2.5.3/zeta/cli/__init__.py
+-rw-r--r--   0        0        0     1937 2024-05-21 00:22:21.766088 zetascale-2.5.3/zeta/cli/main.py
+-rw-r--r--   0        0        0      157 2024-05-21 00:22:21.766172 zetascale-2.5.3/zeta/cloud/__init__.py
+-rw-r--r--   0        0        0     2071 2024-05-21 00:22:21.766216 zetascale-2.5.3/zeta/cloud/main.py
+-rw-r--r--   0        0        0     6068 2024-05-21 00:22:21.766270 zetascale-2.5.3/zeta/cloud/sky_api.py
+-rw-r--r--   0        0        0       59 2024-05-21 00:22:21.766338 zetascale-2.5.3/zeta/experimental/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766382 zetascale-2.5.3/zeta/experimental/triton/__init__.py
+-rw-r--r--   0        0        0     1656 2024-05-21 00:22:21.766461 zetascale-2.5.3/zeta/experimental/triton/activations/__init__.py
+-rw-r--r--   0        0        0     2600 2024-05-21 00:22:21.766506 zetascale-2.5.3/zeta/experimental/triton/activations/activations.py
+-rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766525 zetascale-2.5.3/zeta/experimental/triton/activations/flash_mlp.py
+-rw-r--r--   0        0        0     9532 2024-05-21 00:22:21.766605 zetascale-2.5.3/zeta/experimental/triton/activations/functions.py
+-rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766648 zetascale-2.5.3/zeta/experimental/triton/triton_modules/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766675 zetascale-2.5.3/zeta/experimental/triton/triton_modules/flash_mlp.py
+-rw-r--r--   0        0        0     2806 2024-05-21 00:22:21.766729 zetascale-2.5.3/zeta/experimental/triton/triton_modules/linear_proj.py
+-rw-r--r--   0        0        0     3311 2024-05-21 00:22:21.766804 zetascale-2.5.3/zeta/models/BEiT3.py
+-rw-r--r--   0        0        0     1809 2024-05-21 00:22:21.766856 zetascale-2.5.3/zeta/models/LongNet.py
+-rw-r--r--   0        0        0        0 2024-05-21 00:22:21.766873 zetascale-2.5.3/zeta/models/Magneto.py
+-rw-r--r--   0        0        0      603 2024-05-21 00:22:21.766925 zetascale-2.5.3/zeta/models/__init__.py
+-rw-r--r--   0        0        0     3308 2024-05-21 00:22:21.766969 zetascale-2.5.3/zeta/models/andromeda.py
+-rw-r--r--   0        0        0      135 2024-05-21 00:22:21.767013 zetascale-2.5.3/zeta/models/base.py
+-rw-r--r--   0        0        0     6752 2024-05-21 00:22:21.767073 zetascale-2.5.3/zeta/models/gpt4.py
+-rw-r--r--   0        0        0     4288 2024-05-21 00:22:21.767120 zetascale-2.5.3/zeta/models/kosmos.py
+-rw-r--r--   0        0        0      949 2024-05-21 00:22:21.767166 zetascale-2.5.3/zeta/models/llama.py
+-rw-r--r--   0        0        0     3639 2024-05-21 00:22:21.767223 zetascale-2.5.3/zeta/models/max_vit.py
+-rw-r--r--   0        0        0     6678 2024-05-21 00:22:21.767283 zetascale-2.5.3/zeta/models/mega_vit.py
+-rw-r--r--   0        0        0     6927 2024-05-21 00:22:21.767340 zetascale-2.5.3/zeta/models/mm_mamba.py
+-rw-r--r--   0        0        0    12991 2024-05-21 00:22:21.767416 zetascale-2.5.3/zeta/models/navit.py
+-rw-r--r--   0        0        0     1884 2024-05-21 00:22:21.767454 zetascale-2.5.3/zeta/models/palme.py
+-rw-r--r--   0        0        0     2762 2024-05-21 00:22:21.767499 zetascale-2.5.3/zeta/models/vit.py
+-rw-r--r--   0        0        0      219 2024-05-21 00:22:21.767567 zetascale-2.5.3/zeta/nn/__init__.py
+-rw-r--r--   0        0        0     1895 2024-05-21 00:22:21.767637 zetascale-2.5.3/zeta/nn/attention/__init__.py
+-rw-r--r--   0        0        0     4184 2024-05-21 00:22:21.767693 zetascale-2.5.3/zeta/nn/attention/agent_attn.py
+-rw-r--r--   0        0        0    14876 2024-05-21 00:22:21.767772 zetascale-2.5.3/zeta/nn/attention/attend.py
+-rw-r--r--   0        0        0      244 2024-05-21 00:22:21.767819 zetascale-2.5.3/zeta/nn/attention/base.py
+-rw-r--r--   0        0        0     4050 2024-05-21 00:22:21.767875 zetascale-2.5.3/zeta/nn/attention/cross_attention.py
+-rw-r--r--   0        0        0     3236 2024-05-21 00:22:21.767922 zetascale-2.5.3/zeta/nn/attention/cross_attn_images.py
+-rw-r--r--   0        0        0    10734 2024-05-21 00:22:21.767991 zetascale-2.5.3/zeta/nn/attention/dilated_attention.py
+-rw-r--r--   0        0        0     8803 2024-05-21 00:22:21.768136 zetascale-2.5.3/zeta/nn/attention/flash_attention.py
+-rw-r--r--   0        0        0     2161 2024-05-21 00:22:21.768183 zetascale-2.5.3/zeta/nn/attention/linear_attention.py
+-rw-r--r--   0        0        0     2370 2024-05-21 00:22:21.768231 zetascale-2.5.3/zeta/nn/attention/linear_attn_l.py
+-rw-r--r--   0        0        0     2090 2024-05-21 00:37:46.889652 zetascale-2.5.3/zeta/nn/attention/linearized_attention.py
+-rw-r--r--   0        0        0     9794 2024-05-21 00:22:21.768347 zetascale-2.5.3/zeta/nn/attention/local_attention.py
+-rw-r--r--   0        0        0     1966 2024-05-21 00:22:21.768392 zetascale-2.5.3/zeta/nn/attention/local_attention_mha.py
+-rw-r--r--   0        0        0    18990 2024-05-21 00:22:21.768470 zetascale-2.5.3/zeta/nn/attention/mixture_attention.py
+-rw-r--r--   0        0        0    12414 2024-05-21 00:22:21.768567 zetascale-2.5.3/zeta/nn/attention/multi_grouped_attn.py
+-rw-r--r--   0        0        0     2729 2024-05-21 00:22:21.768617 zetascale-2.5.3/zeta/nn/attention/multi_modal_causal_attention.py
+-rw-r--r--   0        0        0     3879 2024-05-21 00:22:21.768670 zetascale-2.5.3/zeta/nn/attention/multi_modal_cross_attn.py
+-rw-r--r--   0        0        0     5769 2024-05-21 00:22:21.768725 zetascale-2.5.3/zeta/nn/attention/multihead_attention.py
+-rw-r--r--   0        0        0    25310 2024-05-21 00:37:47.151935 zetascale-2.5.3/zeta/nn/attention/multiquery_attention.py
+-rw-r--r--   0        0        0     3979 2024-05-21 00:22:21.768851 zetascale-2.5.3/zeta/nn/attention/scalable_img_self_attn.py
+-rw-r--r--   0        0        0     2198 2024-05-21 00:22:21.768897 zetascale-2.5.3/zeta/nn/attention/shaped_attention.py
+-rw-r--r--   0        0        0     4672 2024-05-21 00:22:21.768952 zetascale-2.5.3/zeta/nn/attention/sparse_attention.py
+-rw-r--r--   0        0        0     1741 2024-05-21 00:22:21.768998 zetascale-2.5.3/zeta/nn/attention/spatial_linear_attention.py
+-rw-r--r--   0        0        0     2973 2024-05-21 00:22:21.769048 zetascale-2.5.3/zeta/nn/attention/xc_attention.py
+-rw-r--r--   0        0        0      482 2024-05-21 00:22:21.769118 zetascale-2.5.3/zeta/nn/biases/__init__.py
+-rw-r--r--   0        0        0     3951 2024-05-21 00:22:21.769171 zetascale-2.5.3/zeta/nn/biases/alibi.py
+-rw-r--r--   0        0        0      245 2024-05-21 00:22:21.769209 zetascale-2.5.3/zeta/nn/biases/base.py
+-rw-r--r--   0        0        0     1348 2024-05-21 00:22:21.769251 zetascale-2.5.3/zeta/nn/biases/dynamic_position_bias.py
+-rw-r--r--   0        0        0     2886 2024-05-21 00:22:21.769300 zetascale-2.5.3/zeta/nn/biases/relative_position_bias.py
+-rw-r--r--   0        0        0     2069 2024-05-21 00:22:21.769370 zetascale-2.5.3/zeta/nn/embeddings/__init__.py
+-rw-r--r--   0        0        0     1231 2024-05-21 00:22:21.769427 zetascale-2.5.3/zeta/nn/embeddings/abc_pos_emb.py
+-rw-r--r--   0        0        0      255 2024-05-21 00:22:21.769468 zetascale-2.5.3/zeta/nn/embeddings/base.py
+-rw-r--r--   0        0        0      723 2024-05-21 00:22:21.769514 zetascale-2.5.3/zeta/nn/embeddings/embedding.py
+-rw-r--r--   0        0        0     2509 2024-05-21 00:22:21.769562 zetascale-2.5.3/zeta/nn/embeddings/multiway_network.py
+-rw-r--r--   0        0        0      358 2024-05-21 00:22:21.769604 zetascale-2.5.3/zeta/nn/embeddings/nominal_embeddings.py
+-rw-r--r--   0        0        0      900 2024-05-21 00:22:21.769647 zetascale-2.5.3/zeta/nn/embeddings/patch_embedding.py
+-rw-r--r--   0        0        0     3120 2024-05-21 00:22:21.769692 zetascale-2.5.3/zeta/nn/embeddings/pi.md
+-rw-r--r--   0        0        0     1996 2024-05-21 00:22:21.769737 zetascale-2.5.3/zeta/nn/embeddings/positional.py
+-rw-r--r--   0        0        0     2584 2024-05-21 00:22:21.769792 zetascale-2.5.3/zeta/nn/embeddings/positional_interpolation.py
+-rw-r--r--   0        0        0     3021 2024-05-21 00:22:21.769839 zetascale-2.5.3/zeta/nn/embeddings/qfsp_embeddings.py
+-rw-r--r--   0        0        0     1668 2024-05-21 00:22:21.769891 zetascale-2.5.3/zeta/nn/embeddings/qft_embeddings.py
+-rw-r--r--   0        0        0     2339 2024-05-25 23:43:49.883932 zetascale-2.5.3/zeta/nn/embeddings/rope.py
+-rw-r--r--   0        0        0     1570 2024-05-21 00:22:21.770017 zetascale-2.5.3/zeta/nn/embeddings/scaled_sinusoidal_embeddings.py
+-rw-r--r--   0        0        0     2345 2024-05-21 00:22:21.770062 zetascale-2.5.3/zeta/nn/embeddings/sine_positional.py
+-rw-r--r--   0        0        0     2650 2024-05-21 00:22:21.770108 zetascale-2.5.3/zeta/nn/embeddings/sinusoidal.py
+-rw-r--r--   0        0        0     1810 2024-05-21 00:22:21.770156 zetascale-2.5.3/zeta/nn/embeddings/truncated_rope.py
+-rw-r--r--   0        0        0     1003 2024-05-21 00:22:21.770199 zetascale-2.5.3/zeta/nn/embeddings/vis_lang_emb.py
+-rw-r--r--   0        0        0     3195 2024-05-21 00:22:21.770249 zetascale-2.5.3/zeta/nn/embeddings/vision_emb.py
+-rw-r--r--   0        0        0     3208 2024-05-21 00:22:21.770299 zetascale-2.5.3/zeta/nn/embeddings/xpos_relative_position.py
+-rw-r--r--   0        0        0     6685 2024-05-21 00:22:21.770353 zetascale-2.5.3/zeta/nn/embeddings/yarn.py
+-rw-r--r--   0        0        0     1150 2024-05-21 00:22:21.770425 zetascale-2.5.3/zeta/nn/masks/__init__.py
+-rw-r--r--   0        0        0    31987 2024-05-21 00:22:21.770499 zetascale-2.5.3/zeta/nn/masks/attn_masks.py
+-rw-r--r--   0        0        0     1248 2024-05-21 00:22:21.770558 zetascale-2.5.3/zeta/nn/masks/block_diagonal.py
+-rw-r--r--   0        0        0    15253 2024-05-21 00:22:21.770674 zetascale-2.5.3/zeta/nn/modules/README.md
+-rw-r--r--   0        0        0    14174 2024-05-25 23:48:50.017331 zetascale-2.5.3/zeta/nn/modules/__init__.py
+-rw-r--r--   0        0        0     7658 2024-05-21 00:22:21.770820 zetascale-2.5.3/zeta/nn/modules/_activations.py
+-rw-r--r--   0        0        0     3561 2024-05-21 00:22:21.770869 zetascale-2.5.3/zeta/nn/modules/adaptive_conv.py
+-rw-r--r--   0        0        0     1572 2024-05-21 00:22:21.770917 zetascale-2.5.3/zeta/nn/modules/adaptive_layernorm.py
+-rw-r--r--   0        0        0     1506 2024-05-21 00:22:21.770965 zetascale-2.5.3/zeta/nn/modules/adaptive_parameter_list.py
+-rw-r--r--   0        0        0     2181 2024-05-21 00:22:21.771010 zetascale-2.5.3/zeta/nn/modules/adaptive_rmsnorm.py
+-rw-r--r--   0        0        0      465 2024-05-21 00:22:21.771057 zetascale-2.5.3/zeta/nn/modules/add_norm.py
+-rw-r--r--   0        0        0     1969 2024-05-21 00:22:21.771101 zetascale-2.5.3/zeta/nn/modules/alr_block.py
+-rw-r--r--   0        0        0     1885 2024-05-21 00:22:21.771145 zetascale-2.5.3/zeta/nn/modules/attn.py
+-rw-r--r--   0        0        0     1170 2024-05-21 00:22:21.771188 zetascale-2.5.3/zeta/nn/modules/audio_to_text.py
+-rw-r--r--   0        0        0     2927 2024-05-21 00:22:21.771233 zetascale-2.5.3/zeta/nn/modules/avg_model_merger.py
+-rw-r--r--   0        0        0      200 2024-05-21 00:22:21.771283 zetascale-2.5.3/zeta/nn/modules/batched_dp.py
+-rw-r--r--   0        0        0     2355 2024-05-21 00:22:21.771334 zetascale-2.5.3/zeta/nn/modules/block_butterfly_mlp.py
+-rw-r--r--   0        0        0    12691 2024-05-21 00:37:47.719254 zetascale-2.5.3/zeta/nn/modules/blockdiag_butterfly.py
+-rw-r--r--   0        0        0      986 2024-05-21 00:22:21.771470 zetascale-2.5.3/zeta/nn/modules/chan_layer_norm.py
+-rw-r--r--   0        0        0     7693 2024-05-21 00:22:21.771536 zetascale-2.5.3/zeta/nn/modules/clex.py
+-rw-r--r--   0        0        0     2522 2024-05-21 00:22:21.771589 zetascale-2.5.3/zeta/nn/modules/clip_bottleneck.py
+-rw-r--r--   0        0        0     1530 2024-05-21 00:22:21.771639 zetascale-2.5.3/zeta/nn/modules/cnn_text.py
+-rw-r--r--   0        0        0     4281 2024-05-21 00:22:21.771705 zetascale-2.5.3/zeta/nn/modules/combined_linear.py
+-rw-r--r--   0        0        0     1026 2024-05-21 00:22:21.771761 zetascale-2.5.3/zeta/nn/modules/conv_bn_relu.py
+-rw-r--r--   0        0        0     2422 2024-05-21 00:37:46.940310 zetascale-2.5.3/zeta/nn/modules/conv_mlp.py
+-rw-r--r--   0        0        0      888 2024-05-21 00:22:21.771867 zetascale-2.5.3/zeta/nn/modules/convnet.py
+-rw-r--r--   0        0        0     1723 2024-05-21 00:22:21.771923 zetascale-2.5.3/zeta/nn/modules/cross_embed_layer.py
+-rw-r--r--   0        0        0     7316 2024-05-21 00:22:21.771989 zetascale-2.5.3/zeta/nn/modules/cross_modal_reparametization.py
+-rw-r--r--   0        0        0     3540 2024-05-21 00:22:21.772043 zetascale-2.5.3/zeta/nn/modules/decision_tree.py
+-rw-r--r--   0        0        0     2648 2024-05-21 00:22:21.772100 zetascale-2.5.3/zeta/nn/modules/deepseek_moe.py
+-rw-r--r--   0        0        0      794 2024-05-21 00:22:21.772158 zetascale-2.5.3/zeta/nn/modules/dense_connect.py
+-rw-r--r--   0        0        0     2371 2024-05-21 00:22:21.772210 zetascale-2.5.3/zeta/nn/modules/diffusion.py
+-rw-r--r--   0        0        0     1538 2024-05-21 00:22:21.772263 zetascale-2.5.3/zeta/nn/modules/droppath.py
+-rw-r--r--   0        0        0      796 2024-05-21 00:22:21.772319 zetascale-2.5.3/zeta/nn/modules/dual_path_block.py
+-rw-r--r--   0        0        0     4687 2024-05-21 00:22:21.772383 zetascale-2.5.3/zeta/nn/modules/dyna_conv.py
+-rw-r--r--   0        0        0     2064 2024-05-21 00:22:21.772435 zetascale-2.5.3/zeta/nn/modules/dynamic_module.py
+-rw-r--r--   0        0        0      980 2024-05-21 00:22:21.772485 zetascale-2.5.3/zeta/nn/modules/dynamic_routing_block.py
+-rw-r--r--   0        0        0      786 2024-05-21 00:22:21.772538 zetascale-2.5.3/zeta/nn/modules/embedding_to_grid.py
+-rw-r--r--   0        0        0    11202 2024-05-21 00:22:21.772616 zetascale-2.5.3/zeta/nn/modules/ether.py
+-rw-r--r--   0        0        0     5338 2024-05-21 00:22:21.772683 zetascale-2.5.3/zeta/nn/modules/exo.py
+-rw-r--r--   0        0        0       92 2024-05-21 00:22:21.772729 zetascale-2.5.3/zeta/nn/modules/expand.py
+-rw-r--r--   0        0        0      888 2024-05-21 00:22:21.772777 zetascale-2.5.3/zeta/nn/modules/expand_channels.py
+-rw-r--r--   0        0        0     1184 2024-05-21 00:22:21.772828 zetascale-2.5.3/zeta/nn/modules/expert.py
+-rw-r--r--   0        0        0      678 2024-05-21 00:22:21.772881 zetascale-2.5.3/zeta/nn/modules/fast_text.py
+-rw-r--r--   0        0        0     1004 2024-05-21 00:22:21.772931 zetascale-2.5.3/zeta/nn/modules/feedback_block.py
+-rw-r--r--   0        0        0     4666 2024-05-21 00:22:21.772994 zetascale-2.5.3/zeta/nn/modules/feedforward.py
+-rw-r--r--   0        0        0     4396 2024-05-21 00:22:21.773060 zetascale-2.5.3/zeta/nn/modules/feedforward_network.py
+-rw-r--r--   0        0        0     3153 2024-05-21 00:22:21.773107 zetascale-2.5.3/zeta/nn/modules/film.py
+-rw-r--r--   0        0        0     2607 2024-05-21 00:22:21.773167 zetascale-2.5.3/zeta/nn/modules/film_conditioning.py
+-rw-r--r--   0        0        0     2657 2024-05-21 00:22:21.773220 zetascale-2.5.3/zeta/nn/modules/film_efficient_metb3.py
+-rw-r--r--   0        0        0      363 2024-05-21 00:22:21.773275 zetascale-2.5.3/zeta/nn/modules/flash_conv.py
+-rw-r--r--   0        0        0      817 2024-05-21 00:22:21.773327 zetascale-2.5.3/zeta/nn/modules/flatten_features.py
+-rw-r--r--   0        0        0     3528 2024-05-21 00:22:21.773378 zetascale-2.5.3/zeta/nn/modules/flex_conv.py
+-rw-r--r--   0        0        0     2694 2024-05-21 00:22:21.773439 zetascale-2.5.3/zeta/nn/modules/flexible_mlp.py
+-rw-r--r--   0        0        0      845 2024-05-21 00:22:21.773492 zetascale-2.5.3/zeta/nn/modules/fractoral_norm.py
+-rw-r--r--   0        0        0     2552 2024-05-21 00:22:21.773545 zetascale-2.5.3/zeta/nn/modules/fractorial_net.py
+-rw-r--r--   0        0        0      769 2024-05-21 00:22:21.773599 zetascale-2.5.3/zeta/nn/modules/freeze_layers.py
+-rw-r--r--   0        0        0     2408 2024-05-21 00:22:21.773650 zetascale-2.5.3/zeta/nn/modules/fused_dropout_add.py
+-rw-r--r--   0        0        0     1223 2024-05-21 00:22:21.773701 zetascale-2.5.3/zeta/nn/modules/fused_dropout_layernom.py
+-rw-r--r--   0        0        0     2268 2024-05-21 00:22:21.773755 zetascale-2.5.3/zeta/nn/modules/fused_gelu_dense.py
+-rw-r--r--   0        0        0     1006 2024-05-21 00:22:21.773804 zetascale-2.5.3/zeta/nn/modules/fusion_ffn.py
+-rw-r--r--   0        0        0    33392 2024-05-21 00:22:21.773904 zetascale-2.5.3/zeta/nn/modules/g_shard_moe.py
+-rw-r--r--   0        0        0     1800 2024-05-25 18:14:50.721305 zetascale-2.5.3/zeta/nn/modules/gated_cnn_block.py
+-rw-r--r--   0        0        0      707 2024-05-21 00:22:21.773969 zetascale-2.5.3/zeta/nn/modules/gated_residual_block.py
+-rw-r--r--   0        0        0     4104 2024-05-21 00:22:21.774037 zetascale-2.5.3/zeta/nn/modules/gill_mapper.py
+-rw-r--r--   0        0        0      920 2024-05-21 00:22:21.774094 zetascale-2.5.3/zeta/nn/modules/glu.py
+-rw-r--r--   0        0        0     1826 2024-05-21 00:22:21.774153 zetascale-2.5.3/zeta/nn/modules/gru_gating.py
+-rw-r--r--   0        0        0     2634 2024-05-21 00:22:21.774210 zetascale-2.5.3/zeta/nn/modules/h3.py
+-rw-r--r--   0        0        0     2078 2024-05-21 00:22:21.774272 zetascale-2.5.3/zeta/nn/modules/hebbian.py
+-rw-r--r--   0        0        0      809 2024-05-21 00:22:21.774328 zetascale-2.5.3/zeta/nn/modules/highway_layer.py
+-rw-r--r--   0        0        0     3527 2024-05-21 00:22:21.774388 zetascale-2.5.3/zeta/nn/modules/image_projector.py
+-rw-r--r--   0        0        0     1049 2024-05-21 00:22:21.774442 zetascale-2.5.3/zeta/nn/modules/image_to_text.py
+-rw-r--r--   0        0        0     1385 2024-05-21 00:22:21.774487 zetascale-2.5.3/zeta/nn/modules/img_or_video_to_time.py
+-rw-r--r--   0        0        0     1197 2024-05-21 00:22:21.774532 zetascale-2.5.3/zeta/nn/modules/img_patch_embed.py
+-rw-r--r--   0        0        0      763 2024-05-21 00:22:21.774576 zetascale-2.5.3/zeta/nn/modules/img_reshape.py
+-rw-r--r--   0        0        0     4024 2024-05-21 00:22:21.774623 zetascale-2.5.3/zeta/nn/modules/itca.py
+-rw-r--r--   0        0        0    12420 2024-05-21 00:22:21.774693 zetascale-2.5.3/zeta/nn/modules/kan.py
+-rw-r--r--   0        0        0     4656 2024-05-21 00:22:21.774746 zetascale-2.5.3/zeta/nn/modules/kv_cache.py
+-rw-r--r--   0        0        0     2586 2024-05-21 00:22:21.774792 zetascale-2.5.3/zeta/nn/modules/kv_cache_update.py
+-rw-r--r--   0        0        0     6221 2024-05-21 00:22:21.774846 zetascale-2.5.3/zeta/nn/modules/lambda_mask.py
+-rw-r--r--   0        0        0     3504 2024-05-21 00:22:21.774895 zetascale-2.5.3/zeta/nn/modules/lang_conv_module.py
+-rw-r--r--   0        0        0     2760 2024-05-21 00:22:21.774942 zetascale-2.5.3/zeta/nn/modules/laser.py
+-rw-r--r--   0        0        0      919 2024-05-21 00:22:21.774987 zetascale-2.5.3/zeta/nn/modules/layer_scale.py
+-rw-r--r--   0        0        0     2379 2024-05-21 00:22:21.775034 zetascale-2.5.3/zeta/nn/modules/layernorm.py
+-rw-r--r--   0        0        0     1132 2024-05-21 00:22:21.775081 zetascale-2.5.3/zeta/nn/modules/leaky_relu.py
+-rw-r--r--   0        0        0    24514 2024-05-21 00:22:21.775141 zetascale-2.5.3/zeta/nn/modules/log_ff.py
+-rw-r--r--   0        0        0     1747 2024-05-21 00:22:21.775199 zetascale-2.5.3/zeta/nn/modules/lora.py
+-rw-r--r--   0        0        0     3240 2024-05-21 00:22:21.775247 zetascale-2.5.3/zeta/nn/modules/matrix.py
+-rw-r--r--   0        0        0     2993 2024-05-21 00:22:21.775291 zetascale-2.5.3/zeta/nn/modules/mbconv.py
+-rw-r--r--   0        0        0     3127 2024-05-21 00:22:21.775334 zetascale-2.5.3/zeta/nn/modules/mixtape.py
+-rw-r--r--   0        0        0     2125 2024-05-21 00:22:21.775378 zetascale-2.5.3/zeta/nn/modules/mixtral_expert.py
+-rw-r--r--   0        0        0     1884 2024-05-21 00:22:21.775424 zetascale-2.5.3/zeta/nn/modules/mlp.py
+-rw-r--r--   0        0        0     3729 2024-05-21 00:22:21.775471 zetascale-2.5.3/zeta/nn/modules/mlp_mixer.py
+-rw-r--r--   0        0        0     2435 2024-05-21 00:22:21.775520 zetascale-2.5.3/zeta/nn/modules/mm_adapter.py
+-rw-r--r--   0        0        0       87 2024-05-21 00:22:21.775561 zetascale-2.5.3/zeta/nn/modules/mm_fusion.py
+-rw-r--r--   0        0        0     2340 2024-05-21 00:22:21.775609 zetascale-2.5.3/zeta/nn/modules/mm_layernorm.py
+-rw-r--r--   0        0        0     1405 2024-05-21 00:22:21.775649 zetascale-2.5.3/zeta/nn/modules/mm_ops.py
+-rw-r--r--   0        0        0     6234 2024-05-21 00:22:21.775711 zetascale-2.5.3/zeta/nn/modules/modality_adaptive_module.py
+-rw-r--r--   0        0        0     2930 2024-05-21 00:22:21.775756 zetascale-2.5.3/zeta/nn/modules/moe.py
+-rw-r--r--   0        0        0     3228 2024-05-21 00:22:21.775806 zetascale-2.5.3/zeta/nn/modules/moe_router.py
+-rw-r--r--   0        0        0      776 2024-05-21 00:22:21.775853 zetascale-2.5.3/zeta/nn/modules/monarch_mlp.py
+-rw-r--r--   0        0        0     1564 2024-05-21 00:22:21.775900 zetascale-2.5.3/zeta/nn/modules/mr_adapter.py
+-rw-r--r--   0        0        0     6686 2024-05-21 00:22:21.775960 zetascale-2.5.3/zeta/nn/modules/multi_input_multi_output.py
+-rw-r--r--   0        0        0      837 2024-05-21 00:22:21.776004 zetascale-2.5.3/zeta/nn/modules/multi_scale_block.py
+-rw-r--r--   0        0        0        2 2024-05-21 00:22:21.776046 zetascale-2.5.3/zeta/nn/modules/multiclass_label.py
+-rw-r--r--   0        0        0      225 2024-05-21 00:22:21.776089 zetascale-2.5.3/zeta/nn/modules/multimodal_concat.py
+-rw-r--r--   0        0        0      472 2024-05-21 00:22:21.776130 zetascale-2.5.3/zeta/nn/modules/nearest_upsample.py
+-rw-r--r--   0        0        0     8309 2024-05-21 00:22:21.776199 zetascale-2.5.3/zeta/nn/modules/nebula.py
+-rw-r--r--   0        0        0     2590 2024-05-21 00:22:21.776249 zetascale-2.5.3/zeta/nn/modules/nfn_stem.py
+-rw-r--r--   0        0        0     1456 2024-05-21 00:22:21.776295 zetascale-2.5.3/zeta/nn/modules/norm_fractorals.py
+-rw-r--r--   0        0        0     2034 2024-05-21 00:22:21.776341 zetascale-2.5.3/zeta/nn/modules/norm_utils.py
+-rw-r--r--   0        0        0     2842 2024-05-21 00:22:21.776388 zetascale-2.5.3/zeta/nn/modules/omnimodal_fusion.py
+-rw-r--r--   0        0        0     3851 2024-05-21 00:22:21.776438 zetascale-2.5.3/zeta/nn/modules/p_scan.py
+-rw-r--r--   0        0        0     2571 2024-05-21 00:22:21.776486 zetascale-2.5.3/zeta/nn/modules/palo_ldp.py
+-rw-r--r--   0        0        0      601 2024-05-21 00:22:21.776528 zetascale-2.5.3/zeta/nn/modules/parallel_wrapper.py
+-rw-r--r--   0        0        0      200 2024-05-21 00:22:21.776570 zetascale-2.5.3/zeta/nn/modules/patch_img.py
+-rw-r--r--   0        0        0     6597 2024-05-21 00:22:21.776626 zetascale-2.5.3/zeta/nn/modules/patch_linear_flatten.py
+-rw-r--r--   0        0        0      985 2024-05-21 00:22:21.776673 zetascale-2.5.3/zeta/nn/modules/patch_video.py
+-rw-r--r--   0        0        0      783 2024-05-21 00:22:21.776716 zetascale-2.5.3/zeta/nn/modules/peg.py
+-rw-r--r--   0        0        0     3180 2024-05-21 00:22:21.776764 zetascale-2.5.3/zeta/nn/modules/perceiver_layer.py
+-rw-r--r--   0        0        0     6115 2024-05-21 00:22:21.776830 zetascale-2.5.3/zeta/nn/modules/perceiver_resampler.py
+-rw-r--r--   0        0        0     2594 2024-05-21 00:22:21.776877 zetascale-2.5.3/zeta/nn/modules/pixel_shuffling.py
+-rw-r--r--   0        0        0     1692 2024-05-21 00:22:21.776921 zetascale-2.5.3/zeta/nn/modules/poly_expert_fusion_network.py
+-rw-r--r--   0        0        0     2045 2024-05-21 00:22:21.776970 zetascale-2.5.3/zeta/nn/modules/polymorphic_activation.py
+-rw-r--r--   0        0        0     5804 2024-05-21 00:22:21.777026 zetascale-2.5.3/zeta/nn/modules/polymorphic_neuron.py
+-rw-r--r--   0        0        0      527 2024-05-21 00:22:21.777070 zetascale-2.5.3/zeta/nn/modules/prenorm.py
+-rw-r--r--   0        0        0     1299 2024-05-21 00:22:21.777113 zetascale-2.5.3/zeta/nn/modules/proj_then_softmax.py
+-rw-r--r--   0        0        0     7164 2024-05-21 00:22:21.777170 zetascale-2.5.3/zeta/nn/modules/pulsar.py
+-rw-r--r--   0        0        0     3451 2024-05-21 00:22:21.777217 zetascale-2.5.3/zeta/nn/modules/pyro.py
+-rw-r--r--   0        0        0     9454 2024-05-21 00:22:21.777284 zetascale-2.5.3/zeta/nn/modules/qformer.py
+-rw-r--r--   0        0        0      812 2024-05-21 00:22:21.777328 zetascale-2.5.3/zeta/nn/modules/qkv_norm.py
+-rw-r--r--   0        0        0     1381 2024-05-21 00:22:21.777374 zetascale-2.5.3/zeta/nn/modules/quantized_layernorm.py
+-rw-r--r--   0        0        0      983 2024-05-21 00:22:21.777417 zetascale-2.5.3/zeta/nn/modules/query_proposal.py
+-rw-r--r--   0        0        0     1152 2024-05-21 00:22:21.777463 zetascale-2.5.3/zeta/nn/modules/recurrent_model.py
+-rw-r--r--   0        0        0      903 2024-05-21 00:22:21.777512 zetascale-2.5.3/zeta/nn/modules/recursive_block.py
+-rw-r--r--   0        0        0      369 2024-05-21 00:22:21.777555 zetascale-2.5.3/zeta/nn/modules/relu_squared.py
+-rw-r--r--   0        0        0     5037 2024-05-21 00:22:21.777610 zetascale-2.5.3/zeta/nn/modules/res_net.py
+-rw-r--r--   0        0        0      492 2024-05-21 00:22:21.777667 zetascale-2.5.3/zeta/nn/modules/residual.py
+-rw-r--r--   0        0        0     2238 2024-05-21 00:22:21.777714 zetascale-2.5.3/zeta/nn/modules/resnet.py
+-rw-r--r--   0        0        0     5349 2024-05-21 00:22:21.777769 zetascale-2.5.3/zeta/nn/modules/return_loss_text.py
+-rw-r--r--   0        0        0      829 2024-05-21 00:22:21.777812 zetascale-2.5.3/zeta/nn/modules/rms_norm.py
+-rw-r--r--   0        0        0     1646 2024-05-21 00:22:21.777856 zetascale-2.5.3/zeta/nn/modules/rnn_nlp.py
+-rw-r--r--   0        0        0     3106 2024-05-21 00:22:21.777902 zetascale-2.5.3/zeta/nn/modules/s4.py
+-rw-r--r--   0        0        0      818 2024-05-21 00:22:21.777947 zetascale-2.5.3/zeta/nn/modules/scale.py
+-rw-r--r--   0        0        0      882 2024-05-21 00:22:21.777993 zetascale-2.5.3/zeta/nn/modules/scale_norm.py
+-rw-r--r--   0        0        0     1433 2024-05-21 00:22:21.778037 zetascale-2.5.3/zeta/nn/modules/scaled_sinusoidal.py
+-rw-r--r--   0        0        0      799 2024-05-21 00:22:21.778086 zetascale-2.5.3/zeta/nn/modules/scalenorm.py
+-rw-r--r--   0        0        0     1858 2024-05-21 00:22:21.778139 zetascale-2.5.3/zeta/nn/modules/shift_tokens.py
+-rw-r--r--   0        0        0     2877 2024-05-21 00:22:21.778185 zetascale-2.5.3/zeta/nn/modules/shufflenet.py
+-rw-r--r--   0        0        0     8939 2024-05-21 00:22:21.778249 zetascale-2.5.3/zeta/nn/modules/sig_lip.py
+-rw-r--r--   0        0        0     2659 2024-05-25 16:41:31.796497 zetascale-2.5.3/zeta/nn/modules/sig_lip_loss.py
+-rw-r--r--   0        0        0      283 2024-05-21 00:22:21.778291 zetascale-2.5.3/zeta/nn/modules/simple_attention.py
+-rw-r--r--   0        0        0      692 2024-05-21 00:22:21.778338 zetascale-2.5.3/zeta/nn/modules/simple_feedforward.py
+-rw-r--r--   0        0        0     4795 2024-05-26 19:02:17.194033 zetascale-2.5.3/zeta/nn/modules/simple_lstm.py
+-rw-r--r--   0        0        0     9719 2024-05-21 00:22:21.778406 zetascale-2.5.3/zeta/nn/modules/simple_mamba.py
+-rw-r--r--   0        0        0      764 2024-05-21 00:22:21.778454 zetascale-2.5.3/zeta/nn/modules/simple_res_block.py
+-rw-r--r--   0        0        0      978 2024-05-21 00:22:21.778496 zetascale-2.5.3/zeta/nn/modules/simple_resblock.py
+-rw-r--r--   0        0        0      638 2024-05-21 00:22:21.778535 zetascale-2.5.3/zeta/nn/modules/simple_rmsnorm.py
+-rw-r--r--   0        0        0     1011 2024-05-25 23:43:51.977951 zetascale-2.5.3/zeta/nn/modules/simple_rnn.py
+-rw-r--r--   0        0        0      509 2024-05-21 00:22:21.778579 zetascale-2.5.3/zeta/nn/modules/skip_connect.py
+-rw-r--r--   0        0        0     1194 2024-05-21 00:22:21.778621 zetascale-2.5.3/zeta/nn/modules/skipconnection.py
+-rw-r--r--   0        0        0     3553 2024-05-21 00:22:21.778668 zetascale-2.5.3/zeta/nn/modules/slerp_model_merger.py
+-rw-r--r--   0        0        0      765 2024-05-21 00:22:21.778715 zetascale-2.5.3/zeta/nn/modules/sp_act.py
+-rw-r--r--   0        0        0    22085 2024-05-25 18:14:50.844937 zetascale-2.5.3/zeta/nn/modules/space_time_unet.py
+-rw-r--r--   0        0        0     1346 2024-05-21 00:22:21.778853 zetascale-2.5.3/zeta/nn/modules/spacial_transformer.py
+-rw-r--r--   0        0        0     4976 2024-05-21 00:22:21.778909 zetascale-2.5.3/zeta/nn/modules/sparq_attn.py
+-rw-r--r--   0        0        0    13915 2024-05-21 00:22:21.778984 zetascale-2.5.3/zeta/nn/modules/sparse_moe.py
+-rw-r--r--   0        0        0     7355 2024-05-25 22:02:37.956419 zetascale-2.5.3/zeta/nn/modules/sparse_token_integration.py
+-rw-r--r--   0        0        0     2021 2024-05-21 00:22:21.779039 zetascale-2.5.3/zeta/nn/modules/spatial_downsample.py
+-rw-r--r--   0        0        0     1346 2024-05-21 00:22:21.779080 zetascale-2.5.3/zeta/nn/modules/spatial_transformer.py
+-rw-r--r--   0        0        0     5006 2024-05-21 00:22:21.779136 zetascale-2.5.3/zeta/nn/modules/splines.py
+-rw-r--r--   0        0        0     1041 2024-05-21 00:22:21.779183 zetascale-2.5.3/zeta/nn/modules/squeeze_excitation.py
+-rw-r--r--   0        0        0     4334 2024-05-21 00:22:21.779242 zetascale-2.5.3/zeta/nn/modules/ssm.py
+-rw-r--r--   0        0        0     7305 2024-05-21 00:22:21.779306 zetascale-2.5.3/zeta/nn/modules/ssm_language.py
+-rw-r--r--   0        0        0      942 2024-05-21 00:22:21.779348 zetascale-2.5.3/zeta/nn/modules/stoch_depth.py
+-rw-r--r--   0        0        0      958 2024-05-21 00:22:21.779389 zetascale-2.5.3/zeta/nn/modules/stochastic_depth.py
+-rw-r--r--   0        0        0     2032 2024-05-21 00:22:21.779434 zetascale-2.5.3/zeta/nn/modules/subln.py
+-rw-r--r--   0        0        0      972 2024-05-21 00:22:21.779478 zetascale-2.5.3/zeta/nn/modules/super_resolution.py
+-rw-r--r--   0        0        0     5610 2024-05-21 00:37:47.055302 zetascale-2.5.3/zeta/nn/modules/swarmalator.py
+-rw-r--r--   0        0        0     1313 2024-05-21 00:22:21.779579 zetascale-2.5.3/zeta/nn/modules/swiglu.py
+-rw-r--r--   0        0        0      715 2024-05-21 00:22:21.779623 zetascale-2.5.3/zeta/nn/modules/tensor.py
+-rw-r--r--   0        0        0      865 2024-05-21 00:22:21.779670 zetascale-2.5.3/zeta/nn/modules/tensor_to_int.py
+-rw-r--r--   0        0        0     3281 2024-05-21 00:22:21.779722 zetascale-2.5.3/zeta/nn/modules/text_scene_fusion.py
+-rw-r--r--   0        0        0     2692 2024-05-21 00:22:21.779769 zetascale-2.5.3/zeta/nn/modules/text_video_fuse.py
+-rw-r--r--   0        0        0     2104 2024-05-21 00:22:21.779825 zetascale-2.5.3/zeta/nn/modules/time_up_sample.py
+-rw-r--r--   0        0        0      631 2024-05-21 00:22:21.779868 zetascale-2.5.3/zeta/nn/modules/to_logits.py
+-rw-r--r--   0        0        0     2158 2024-05-21 00:22:21.779914 zetascale-2.5.3/zeta/nn/modules/token_learner.py
+-rw-r--r--   0        0        0     1075 2024-05-21 00:22:21.779962 zetascale-2.5.3/zeta/nn/modules/token_mixer.py
+-rw-r--r--   0        0        0      189 2024-05-21 00:22:21.780004 zetascale-2.5.3/zeta/nn/modules/token_shift.py
+-rw-r--r--   0        0        0    10310 2024-05-21 00:22:21.780074 zetascale-2.5.3/zeta/nn/modules/top_n_gating.py
+-rw-r--r--   0        0        0     4363 2024-05-21 00:22:21.780127 zetascale-2.5.3/zeta/nn/modules/transformations.py
+-rw-r--r--   0        0        0      921 2024-05-21 00:22:21.780175 zetascale-2.5.3/zeta/nn/modules/triple_skip.py
+-rw-r--r--   0        0        0     2193 2024-05-21 00:22:21.780221 zetascale-2.5.3/zeta/nn/modules/triton_rmsnorm.py
+-rw-r--r--   0        0        0     4112 2024-05-21 00:22:21.780276 zetascale-2.5.3/zeta/nn/modules/u_mamba.py
+-rw-r--r--   0        0        0     4717 2024-05-21 00:22:21.780330 zetascale-2.5.3/zeta/nn/modules/unet.py
+-rw-r--r--   0        0        0      974 2024-05-21 00:22:21.780381 zetascale-2.5.3/zeta/nn/modules/v_layernorm.py
+-rw-r--r--   0        0        0     1686 2024-05-21 00:22:21.780429 zetascale-2.5.3/zeta/nn/modules/v_pool.py
+-rw-r--r--   0        0        0     2809 2024-05-21 00:22:21.780472 zetascale-2.5.3/zeta/nn/modules/video_autoencoder.py
+-rw-r--r--   0        0        0     9239 2024-05-21 00:22:21.780539 zetascale-2.5.3/zeta/nn/modules/video_diffusion_modules.py
+-rw-r--r--   0        0        0     1497 2024-05-21 00:22:21.780583 zetascale-2.5.3/zeta/nn/modules/video_to_tensor.py
+-rw-r--r--   0        0        0     1067 2024-05-21 00:22:21.780629 zetascale-2.5.3/zeta/nn/modules/video_to_text.py
+-rw-r--r--   0        0        0     2702 2024-05-21 00:22:21.780681 zetascale-2.5.3/zeta/nn/modules/vision_mamba.py
+-rw-r--r--   0        0        0     2018 2024-05-21 00:22:21.780733 zetascale-2.5.3/zeta/nn/modules/vision_weighted_permute_mlp.py
+-rw-r--r--   0        0        0     5445 2024-05-21 00:22:21.780804 zetascale-2.5.3/zeta/nn/modules/visual_expert.py
+-rw-r--r--   0        0        0     6103 2024-05-25 18:23:29.115939 zetascale-2.5.3/zeta/nn/modules/vit_denoiser.py
+-rw-r--r--   0        0        0     3099 2024-05-21 00:22:21.780910 zetascale-2.5.3/zeta/nn/modules/vss_block.py
+-rw-r--r--   0        0        0     2775 2024-05-21 00:22:21.780963 zetascale-2.5.3/zeta/nn/modules/ws_conv2d.py
+-rw-r--r--   0        0        0       86 2024-05-21 00:22:21.781034 zetascale-2.5.3/zeta/nn/modules/xmoe/__init__.py
+-rw-r--r--   0        0        0     2351 2024-05-21 00:22:21.781081 zetascale-2.5.3/zeta/nn/modules/xmoe/global_groups.py
+-rw-r--r--   0        0        0    12458 2024-05-21 00:22:21.781157 zetascale-2.5.3/zeta/nn/modules/xmoe/moe_layer.py
+-rw-r--r--   0        0        0    18694 2024-05-21 00:22:21.781205 zetascale-2.5.3/zeta/nn/modules/xmoe/routing.py
+-rw-r--r--   0        0        0     2302 2024-05-21 00:22:21.781262 zetascale-2.5.3/zeta/nn/modules/yolo.py
+-rw-r--r--   0        0        0     2595 2024-05-21 00:22:21.781338 zetascale-2.5.3/zeta/ops/__Init__.py
+-rw-r--r--   0        0        0      287 2024-05-21 00:22:21.781384 zetascale-2.5.3/zeta/ops/absmax.py
+-rw-r--r--   0        0        0     2652 2024-05-21 00:22:21.781432 zetascale-2.5.3/zeta/ops/async_softmax.py
+-rw-r--r--   0        0        0     2054 2024-05-21 00:22:21.781475 zetascale-2.5.3/zeta/ops/dilated_attn_ops.py
+-rw-r--r--   0        0        0     2017 2024-05-21 00:22:21.781530 zetascale-2.5.3/zeta/ops/einops_from_to.py
+-rw-r--r--   0        0        0     1876 2024-05-21 00:22:21.781580 zetascale-2.5.3/zeta/ops/einops_poly.py
+-rw-r--r--   0        0        0     2150 2024-05-21 00:22:21.781631 zetascale-2.5.3/zeta/ops/expand.py
+-rw-r--r--   0        0        0     1262 2024-05-21 00:22:21.781685 zetascale-2.5.3/zeta/ops/laplace.py
+-rw-r--r--   0        0        0    16114 2024-05-21 00:37:47.171297 zetascale-2.5.3/zeta/ops/main.py
+-rw-r--r--   0        0        0     1392 2024-05-21 00:22:21.781830 zetascale-2.5.3/zeta/ops/misc_act.py
+-rw-r--r--   0        0        0     1671 2024-05-21 00:22:21.781882 zetascale-2.5.3/zeta/ops/mm_rearranges.py
+-rw-r--r--   0        0        0      996 2024-05-21 00:22:21.781933 zetascale-2.5.3/zeta/ops/mm_softmax.py
+-rw-r--r--   0        0        0     1851 2024-05-21 00:22:21.781984 zetascale-2.5.3/zeta/ops/mos.py
+-rw-r--r--   0        0        0      995 2024-05-21 00:22:21.782043 zetascale-2.5.3/zeta/ops/nonlinear.py
+-rw-r--r--   0        0        0     5070 2024-05-21 00:22:21.782115 zetascale-2.5.3/zeta/ops/softmax.py
+-rw-r--r--   0        0        0     1086 2024-05-21 00:22:21.782171 zetascale-2.5.3/zeta/ops/sparsemax.py
+-rw-r--r--   0        0        0      453 2024-05-21 00:22:21.782225 zetascale-2.5.3/zeta/ops/unitwise_norm.py
+-rw-r--r--   0        0        0      814 2024-05-21 00:22:21.782317 zetascale-2.5.3/zeta/optim/__init__.py
+-rw-r--r--   0        0        0    41040 2024-05-21 00:37:47.266975 zetascale-2.5.3/zeta/optim/batched_optimizer.py
+-rw-r--r--   0        0        0    10142 2024-05-21 00:22:21.782511 zetascale-2.5.3/zeta/optim/decoupled_lion.py
+-rw-r--r--   0        0        0     6448 2024-05-21 00:22:21.782568 zetascale-2.5.3/zeta/optim/decoupled_optimizer.py
+-rw-r--r--   0        0        0    12445 2024-05-21 00:22:21.782643 zetascale-2.5.3/zeta/optim/decoupled_sophia.py
+-rw-r--r--   0        0        0     4709 2024-05-21 00:22:21.782696 zetascale-2.5.3/zeta/optim/gradient_ascent.py
+-rw-r--r--   0        0        0     2752 2024-05-21 00:22:21.782748 zetascale-2.5.3/zeta/optim/gradient_equillibrum.py
+-rw-r--r--   0        0        0    19017 2024-05-21 00:22:21.782817 zetascale-2.5.3/zeta/optim/lion8b.py
+-rw-r--r--   0        0        0     3387 2024-05-21 00:22:21.782876 zetascale-2.5.3/zeta/optim/parallel_gradient_descent.py
+-rw-r--r--   0        0        0     4456 2024-05-21 00:37:47.112761 zetascale-2.5.3/zeta/optim/stable_adam.py
+-rw-r--r--   0        0        0      453 2024-05-21 00:22:21.782994 zetascale-2.5.3/zeta/quant/__init__.py
+-rw-r--r--   0        0        0      405 2024-05-21 00:22:21.783040 zetascale-2.5.3/zeta/quant/absmax.py
+-rw-r--r--   0        0        0     2098 2024-05-21 00:22:21.783091 zetascale-2.5.3/zeta/quant/bitlinear.py
+-rw-r--r--   0        0        0     1947 2024-05-21 00:22:21.783141 zetascale-2.5.3/zeta/quant/half_bit_linear.py
+-rw-r--r--   0        0        0    10942 2024-05-21 00:22:21.783220 zetascale-2.5.3/zeta/quant/lfq.py
+-rw-r--r--   0        0        0     3126 2024-05-21 00:22:21.783269 zetascale-2.5.3/zeta/quant/niva.py
+-rw-r--r--   0        0        0    25154 2024-05-27 00:58:21.081993 zetascale-2.5.3/zeta/quant/qlora.py
+-rw-r--r--   0        0        0     6010 2024-05-21 00:22:21.783405 zetascale-2.5.3/zeta/quant/qmoe.py
+-rw-r--r--   0        0        0     3785 2024-05-21 00:22:21.783451 zetascale-2.5.3/zeta/quant/quick.py
+-rw-r--r--   0        0        0        0 2024-05-21 00:22:21.783469 zetascale-2.5.3/zeta/quant/random_proj_quan.py
+-rw-r--r--   0        0        0     1602 2024-05-21 00:22:21.783524 zetascale-2.5.3/zeta/quant/residual_vq.py
+-rw-r--r--   0        0        0     1547 2024-05-21 00:22:21.783574 zetascale-2.5.3/zeta/quant/ste.py
+-rw-r--r--   0        0        0      522 2024-05-21 00:22:21.783655 zetascale-2.5.3/zeta/rl/__init__.py
+-rw-r--r--   0        0        0     4286 2024-05-21 00:22:21.783724 zetascale-2.5.3/zeta/rl/actor_critic.py
+-rw-r--r--   0        0        0     2509 2024-05-21 00:22:21.783780 zetascale-2.5.3/zeta/rl/dpo.py
+-rw-r--r--   0        0        0     3381 2024-05-21 00:22:21.783837 zetascale-2.5.3/zeta/rl/hindsight_replay.py
+-rw-r--r--   0        0        0     2033 2024-05-21 00:22:21.783886 zetascale-2.5.3/zeta/rl/language_reward.py
+-rw-r--r--   0        0        0     4130 2024-05-21 00:22:21.783936 zetascale-2.5.3/zeta/rl/ppo.py
+-rw-r--r--   0        0        0     4513 2024-05-21 00:22:21.784007 zetascale-2.5.3/zeta/rl/priortized_replay_buffer.py
+-rw-r--r--   0        0        0     5765 2024-05-21 00:22:21.784062 zetascale-2.5.3/zeta/rl/priortized_rps.py
+-rw-r--r--   0        0        0      128 2024-05-21 00:22:21.784116 zetascale-2.5.3/zeta/rl/rest.py
+-rw-r--r--   0        0        0     4585 2024-05-21 00:22:21.784178 zetascale-2.5.3/zeta/rl/reward_model.py
+-rw-r--r--   0        0        0     2987 2024-05-21 00:22:21.784233 zetascale-2.5.3/zeta/rl/sumtree.py
+-rw-r--r--   0        0        0     3185 2024-05-21 00:22:21.784290 zetascale-2.5.3/zeta/rl/vision_model_rl.py
+-rw-r--r--   0        0        0     1227 2024-05-21 00:22:21.784375 zetascale-2.5.3/zeta/structs/__init__.py
+-rw-r--r--   0        0        0    11731 2024-05-21 00:22:21.784455 zetascale-2.5.3/zeta/structs/auto_regressive_wrapper.py
+-rw-r--r--   0        0        0     3505 2024-05-21 00:22:21.784512 zetascale-2.5.3/zeta/structs/clip_encoder.py
+-rw-r--r--   0        0        0     6600 2024-05-21 00:22:21.784570 zetascale-2.5.3/zeta/structs/efficient_net.py
+-rw-r--r--   0        0        0     3219 2024-05-21 00:22:21.784620 zetascale-2.5.3/zeta/structs/encoder_decoder.py
+-rw-r--r--   0        0        0    28639 2024-05-21 00:22:21.784698 zetascale-2.5.3/zeta/structs/hierarchical_transformer.py
+-rw-r--r--   0        0        0     5946 2024-05-21 00:22:21.784771 zetascale-2.5.3/zeta/structs/local_transformer.py
+-rw-r--r--   0        0        0     1665 2024-05-21 00:22:21.784824 zetascale-2.5.3/zeta/structs/multi_modal_projector.py
+-rw-r--r--   0        0        0    10839 2024-05-21 00:22:21.784890 zetascale-2.5.3/zeta/structs/simple_transformer.py
+-rw-r--r--   0        0        0     2468 2024-05-21 00:22:21.784940 zetascale-2.5.3/zeta/structs/simple_vision_encoder.py
+-rw-r--r--   0        0        0    68945 2024-05-21 00:22:21.785012 zetascale-2.5.3/zeta/structs/transformer.py
+-rw-r--r--   0        0        0     4490 2024-05-21 00:22:21.785085 zetascale-2.5.3/zeta/structs/transformer_block.py
+-rw-r--r--   0        0        0      485 2024-05-21 00:22:21.785165 zetascale-2.5.3/zeta/tokenizers/__init__.py
+-rw-r--r--   0        0        0     1438 2024-05-21 00:22:21.785219 zetascale-2.5.3/zeta/tokenizers/gptx_tokenizer.py
+-rw-r--r--   0        0        0     3079 2024-05-21 00:22:21.785272 zetascale-2.5.3/zeta/tokenizers/llama_sentencepiece.py
+-rw-r--r--   0        0        0     3651 2024-05-21 00:22:21.785332 zetascale-2.5.3/zeta/tokenizers/multi_modal_tokenizer.py
+-rw-r--r--   0        0        0     3720 2024-05-21 00:22:21.785394 zetascale-2.5.3/zeta/tokenizers/sentence_piece.py
+-rw-r--r--   0        0        0     9771 2024-05-21 00:22:21.785468 zetascale-2.5.3/zeta/tokenizers/tokenmonster.py
+-rw-r--r--   0        0        0      460 2024-05-21 00:22:21.785556 zetascale-2.5.3/zeta/training/__init__.py
+-rw-r--r--   0        0        0     5400 2024-05-21 00:22:21.785622 zetascale-2.5.3/zeta/training/activation_checkpoint.py
+-rw-r--r--   0        0        0     2576 2024-05-21 00:22:21.785674 zetascale-2.5.3/zeta/training/dataloader.py
+-rw-r--r--   0        0        0     3496 2024-05-21 00:22:21.785729 zetascale-2.5.3/zeta/training/fsdp.py
+-rw-r--r--   0        0        0     3186 2024-05-21 00:22:21.785785 zetascale-2.5.3/zeta/training/galore.py
+-rw-r--r--   0        0        0     6054 2024-05-21 00:22:21.785852 zetascale-2.5.3/zeta/training/hive_trainer.py
+-rw-r--r--   0        0        0     1626 2024-05-21 00:22:21.785901 zetascale-2.5.3/zeta/training/parallel_wrapper.py
+-rw-r--r--   0        0        0     2076 2024-05-21 00:37:47.158519 zetascale-2.5.3/zeta/training/scheduler.py
+-rw-r--r--   0        0        0     9273 2024-05-21 00:22:21.786034 zetascale-2.5.3/zeta/training/train.py
+-rw-r--r--   0        0        0     2347 2024-05-21 00:22:21.786126 zetascale-2.5.3/zeta/utils/__init__.py
+-rw-r--r--   0        0        0     3464 2024-05-21 00:22:21.786186 zetascale-2.5.3/zeta/utils/benchmark.py
+-rw-r--r--   0        0        0     1347 2024-05-21 00:22:21.786243 zetascale-2.5.3/zeta/utils/cuda_memory_wrapper.py
+-rw-r--r--   0        0        0     6424 2024-05-21 00:22:21.786310 zetascale-2.5.3/zeta/utils/cuda_wrapper.py
+-rw-r--r--   0        0        0     1337 2024-05-21 00:22:21.786368 zetascale-2.5.3/zeta/utils/disable_logging.py
+-rw-r--r--   0        0        0     1184 2024-05-21 00:22:21.786416 zetascale-2.5.3/zeta/utils/enforce_types.py
+-rw-r--r--   0        0        0     1110 2024-05-21 00:22:21.786470 zetascale-2.5.3/zeta/utils/img_to_tensor.py
+-rw-r--r--   0        0        0     2953 2024-05-21 00:22:21.786528 zetascale-2.5.3/zeta/utils/log_pytorch_op.py
+-rw-r--r--   0        0        0    19874 2024-05-21 00:22:21.786616 zetascale-2.5.3/zeta/utils/main.py
+-rw-r--r--   0        0        0     1798 2024-05-21 00:22:21.786682 zetascale-2.5.3/zeta/utils/module_device.py
+-rw-r--r--   0        0        0      703 2024-05-21 00:22:21.786733 zetascale-2.5.3/zeta/utils/params.py
+-rw-r--r--   0        0        0     3966 2024-05-21 00:22:21.786789 zetascale-2.5.3/zeta/utils/save_load_wrapper.py
+-rw-r--r--   0        0        0      846 2024-05-21 00:22:21.786844 zetascale-2.5.3/zeta/utils/text_to_tensor.py
+-rw-r--r--   0        0        0      751 2024-05-21 00:22:21.786904 zetascale-2.5.3/zeta/utils/verbose_execution.py
+-rw-r--r--   0        0        0    25931 2024-05-21 00:22:21.786981 zetascale-2.5.3/zeta/utils/vision_utils.py
+-rw-r--r--   0        0        0    21412 1970-01-01 00:00:00.000000 zetascale-2.5.3/PKG-INFO
```

### Comparing `zetascale-2.5.1/LICENSE` & `zetascale-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/README.md` & `zetascale-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/pyproject.toml` & `zetascale-2.5.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zetascale"
-version = "2.5.1"
+version = "2.5.3"
 description = "Rapidly Build, Optimize, and Deploy SOTA AI Models"
 authors = ["Zeta Team <kye@apac.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kyegomez/zeta"
 keywords = ["Transformers", "zeta scale"]
 classifiers = [
@@ -25,15 +25,14 @@
 transformers = "4.41.0"
 einops-exts = "0.0.4"
 torchvision = "0.18.0"
 accelerate = "0.30.1"
 datasets = "*"
 loguru = "*"
 vector-quantize-pytorch = "1.14.7"
-scipy = "1.9.3"
 beartype = "0.17.2"
 tqdm = "4.66.3"
 rich = "13.7.1"
 colt5-attention = "*"
 argparse = "^1.4.0"
 local-attention = "*"
```

### Comparing `zetascale-2.5.1/zeta/__init__.py` & `zetascale-2.5.3/zeta/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/cli/main.py` & `zetascale-2.5.3/zeta/cli/main.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/cloud/main.py` & `zetascale-2.5.3/zeta/cloud/main.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/cloud/sky_api.py` & `zetascale-2.5.3/zeta/cloud/sky_api.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/experimental/triton/activations/__init__.py` & `zetascale-2.5.3/zeta/experimental/triton/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/experimental/triton/activations/activations.py` & `zetascale-2.5.3/zeta/experimental/triton/activations/activations.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/experimental/triton/activations/functions.py` & `zetascale-2.5.3/zeta/experimental/triton/activations/functions.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/experimental/triton/triton_modules/linear_proj.py` & `zetascale-2.5.3/zeta/experimental/triton/triton_modules/linear_proj.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/models/BEiT3.py` & `zetascale-2.5.3/zeta/models/BEiT3.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/models/LongNet.py` & `zetascale-2.5.3/zeta/models/LongNet.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/models/__init__.py` & `zetascale-2.5.3/zeta/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/models/andromeda.py` & `zetascale-2.5.3/zeta/models/andromeda.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/models/gpt4.py` & `zetascale-2.5.3/zeta/models/gpt4.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/models/kosmos.py` & `zetascale-2.5.3/zeta/models/kosmos.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/models/llama.py` & `zetascale-2.5.3/zeta/models/llama.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/models/max_vit.py` & `zetascale-2.5.3/zeta/models/max_vit.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/models/mega_vit.py` & `zetascale-2.5.3/zeta/models/mega_vit.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/models/mm_mamba.py` & `zetascale-2.5.3/zeta/models/mm_mamba.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/models/navit.py` & `zetascale-2.5.3/zeta/models/navit.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/models/palme.py` & `zetascale-2.5.3/zeta/models/palme.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/models/vit.py` & `zetascale-2.5.3/zeta/models/vit.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/__init__.py` & `zetascale-2.5.3/zeta/nn/attention/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/agent_attn.py` & `zetascale-2.5.3/zeta/nn/attention/agent_attn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/attend.py` & `zetascale-2.5.3/zeta/nn/attention/attend.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/cross_attention.py` & `zetascale-2.5.3/zeta/nn/attention/cross_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/cross_attn_images.py` & `zetascale-2.5.3/zeta/nn/attention/cross_attn_images.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/dilated_attention.py` & `zetascale-2.5.3/zeta/nn/attention/dilated_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/flash_attention.py` & `zetascale-2.5.3/zeta/nn/attention/flash_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/linear_attention.py` & `zetascale-2.5.3/zeta/nn/attention/linear_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/linear_attn_l.py` & `zetascale-2.5.3/zeta/nn/attention/linear_attn_l.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/linearized_attention.py` & `zetascale-2.5.3/zeta/nn/attention/linearized_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/local_attention.py` & `zetascale-2.5.3/zeta/nn/attention/local_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/local_attention_mha.py` & `zetascale-2.5.3/zeta/nn/attention/local_attention_mha.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/mixture_attention.py` & `zetascale-2.5.3/zeta/nn/attention/mixture_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/multi_grouped_attn.py` & `zetascale-2.5.3/zeta/nn/attention/multi_grouped_attn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/multi_modal_causal_attention.py` & `zetascale-2.5.3/zeta/nn/attention/multi_modal_causal_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/multi_modal_cross_attn.py` & `zetascale-2.5.3/zeta/nn/attention/multi_modal_cross_attn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/multihead_attention.py` & `zetascale-2.5.3/zeta/nn/attention/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/multiquery_attention.py` & `zetascale-2.5.3/zeta/nn/attention/multiquery_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/scalable_img_self_attn.py` & `zetascale-2.5.3/zeta/nn/attention/scalable_img_self_attn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/shaped_attention.py` & `zetascale-2.5.3/zeta/nn/attention/shaped_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/sparse_attention.py` & `zetascale-2.5.3/zeta/nn/attention/sparse_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/spatial_linear_attention.py` & `zetascale-2.5.3/zeta/nn/attention/spatial_linear_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/attention/xc_attention.py` & `zetascale-2.5.3/zeta/nn/attention/xc_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/biases/alibi.py` & `zetascale-2.5.3/zeta/nn/biases/alibi.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/biases/dynamic_position_bias.py` & `zetascale-2.5.3/zeta/nn/biases/dynamic_position_bias.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/biases/relative_position_bias.py` & `zetascale-2.5.3/zeta/nn/biases/relative_position_bias.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/__init__.py` & `zetascale-2.5.3/zeta/nn/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/abc_pos_emb.py` & `zetascale-2.5.3/zeta/nn/embeddings/abc_pos_emb.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/embedding.py` & `zetascale-2.5.3/zeta/nn/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/multiway_network.py` & `zetascale-2.5.3/zeta/nn/embeddings/multiway_network.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/patch_embedding.py` & `zetascale-2.5.3/zeta/nn/embeddings/patch_embedding.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/pi.md` & `zetascale-2.5.3/zeta/nn/embeddings/pi.md`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/positional.py` & `zetascale-2.5.3/zeta/nn/embeddings/positional.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/positional_interpolation.py` & `zetascale-2.5.3/zeta/nn/embeddings/positional_interpolation.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/qfsp_embeddings.py` & `zetascale-2.5.3/zeta/nn/embeddings/qfsp_embeddings.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/qft_embeddings.py` & `zetascale-2.5.3/zeta/nn/embeddings/qft_embeddings.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/rope.py` & `zetascale-2.5.3/zeta/nn/embeddings/rope.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,17 +63,19 @@
         ) / self.scale_base
         scale = self.scale ** rearrange(power, "n -> n 1")
         scale = torch.cat((scale, scale), dim=-1)
 
         return freqs, scale
 
 
-def rotate_half(x):
+def rotate_half(x: torch.Tensor) -> torch.Tensor:
     x = rearrange(x, "... (j d) -> ... j d", j=2)
     x1, x2 = x.unbind(dim=-1)
     return torch.cat((-x2, x1), dim=-1)
 
 
-def apply_rotary_pos_emb(t, freqs, scale=1):
+def apply_rotary_pos_emb(
+    t: torch.Tensor, freqs: torch.Tensor, scale: float = 1
+) -> torch.Tensor:
     seq_len = t.shape[-2]
     freqs = freqs[-seq_len:, :]
     return (t * freqs.cos() * scale) + (rotate_half(t) * freqs.sin() * scale)
```

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/scaled_sinusoidal_embeddings.py` & `zetascale-2.5.3/zeta/nn/embeddings/scaled_sinusoidal_embeddings.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/sine_positional.py` & `zetascale-2.5.3/zeta/nn/embeddings/sine_positional.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/sinusoidal.py` & `zetascale-2.5.3/zeta/nn/embeddings/sinusoidal.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/truncated_rope.py` & `zetascale-2.5.3/zeta/nn/embeddings/truncated_rope.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/vis_lang_emb.py` & `zetascale-2.5.3/zeta/nn/embeddings/vis_lang_emb.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/vision_emb.py` & `zetascale-2.5.3/zeta/nn/embeddings/vision_emb.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/xpos_relative_position.py` & `zetascale-2.5.3/zeta/nn/embeddings/xpos_relative_position.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/embeddings/yarn.py` & `zetascale-2.5.3/zeta/nn/embeddings/yarn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/masks/__init__.py` & `zetascale-2.5.3/zeta/nn/masks/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/masks/attn_masks.py` & `zetascale-2.5.3/zeta/nn/masks/attn_masks.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/masks/block_diagonal.py` & `zetascale-2.5.3/zeta/nn/masks/block_diagonal.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/README.md` & `zetascale-2.5.3/zeta/nn/modules/README.md`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/__init__.py` & `zetascale-2.5.3/zeta/nn/modules/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,34 +118,28 @@
 from zeta.nn.modules.polymorphic_neuron import PolymorphicNeuronLayer
 from zeta.nn.modules.prenorm import PreNorm
 from zeta.nn.modules.proj_then_softmax import FusedProjSoftmax
 from zeta.nn.modules.pulsar import Pulsar
 from zeta.nn.modules.pyro import hyper_optimize
 from zeta.nn.modules.qformer import QFormer
 from zeta.nn.modules.qkv_norm import qk_norm, qkv_norm
-
-#######
 from zeta.nn.modules.quantized_layernorm import QuantizedLN
 from zeta.nn.modules.recursive_block import RecursiveBlock
 from zeta.nn.modules.residual import Residual
 from zeta.nn.modules.resnet import ResNet
 from zeta.nn.modules.rms_norm import RMSNorm
 from zeta.nn.modules.rnn_nlp import RNNL
 from zeta.nn.modules.shufflenet import ShuffleNet
 from zeta.nn.modules.sig_lip import SigLipLoss
 from zeta.nn.modules.simple_attention import simple_attention
 from zeta.nn.modules.simple_feedforward import SimpleFeedForward
-
-######
 from zeta.nn.modules.simple_mamba import Mamba, MambaBlock
 from zeta.nn.modules.simple_res_block import SimpleResBlock
 from zeta.nn.modules.skipconnection import SkipConnection
 from zeta.nn.modules.slerp_model_merger import SLERPModelMerger
-
-####
 from zeta.nn.modules.space_time_unet import (
     ContinuousPositionBias,
     Downsample,
     FeedForwardV,
     PseudoConv3d,
     ResnetBlock,
     SpaceTimeUnet,
@@ -219,14 +213,16 @@
 from zeta.nn.modules.kv_cache_update import kv_cache_with_update
 from zeta.nn.modules.expand import expand
 from zeta.nn.modules.sig_lip_loss import SigLipSigmoidLoss
 from zeta.nn.modules.sparse_token_integration import (
     SparseTokenIntegration,
     SparseChannelIntegration,
 )
+from zeta.nn.modules.simple_lstm import SimpleLSTM
+from zeta.nn.modules.simple_rnn import SimpleRNN
 
 # from zeta.nn.modules.img_reshape import image_reshape
 # from zeta.nn.modules.flatten_features import flatten_features
 # from zeta.nn.modules.scaled_sinusoidal import ScaledSinuosidalEmbedding
 # from zeta.nn.modules.scale import Scale
 # from zeta.nn.modules.scalenorm import ScaleNorm
 # from zeta.nn.modules.simple_rmsnorm import SimpleRMSNorm
@@ -438,8 +434,10 @@
     "LayerScale",
     "FractoralNorm",
     "kv_cache_with_update",
     "expand",
     "SigLipSigmoidLoss",
     "SparseTokenIntegration",
     "SparseChannelIntegration",
+    "SimpleLSTM",
+    "SimpleRNN",
 ]
```

### Comparing `zetascale-2.5.1/zeta/nn/modules/_activations.py` & `zetascale-2.5.3/zeta/nn/modules/_activations.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/adaptive_conv.py` & `zetascale-2.5.3/zeta/nn/modules/adaptive_conv.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/adaptive_layernorm.py` & `zetascale-2.5.3/zeta/nn/modules/adaptive_layernorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/adaptive_parameter_list.py` & `zetascale-2.5.3/zeta/nn/modules/adaptive_parameter_list.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/adaptive_rmsnorm.py` & `zetascale-2.5.3/zeta/nn/modules/adaptive_rmsnorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/alr_block.py` & `zetascale-2.5.3/zeta/nn/modules/alr_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/attn.py` & `zetascale-2.5.3/zeta/nn/modules/attn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/audio_to_text.py` & `zetascale-2.5.3/zeta/nn/modules/audio_to_text.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/avg_model_merger.py` & `zetascale-2.5.3/zeta/nn/modules/avg_model_merger.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/block_butterfly_mlp.py` & `zetascale-2.5.3/zeta/nn/modules/block_butterfly_mlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/blockdiag_butterfly.py` & `zetascale-2.5.3/zeta/nn/modules/blockdiag_butterfly.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/chan_layer_norm.py` & `zetascale-2.5.3/zeta/nn/modules/chan_layer_norm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/clex.py` & `zetascale-2.5.3/zeta/nn/modules/clex.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/clip_bottleneck.py` & `zetascale-2.5.3/zeta/nn/modules/clip_bottleneck.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/cnn_text.py` & `zetascale-2.5.3/zeta/nn/modules/cnn_text.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/combined_linear.py` & `zetascale-2.5.3/zeta/nn/modules/combined_linear.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/conv_bn_relu.py` & `zetascale-2.5.3/zeta/nn/modules/conv_bn_relu.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/conv_mlp.py` & `zetascale-2.5.3/zeta/nn/modules/conv_mlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/convnet.py` & `zetascale-2.5.3/zeta/nn/modules/convnet.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/cross_embed_layer.py` & `zetascale-2.5.3/zeta/nn/modules/cross_embed_layer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/cross_modal_reparametization.py` & `zetascale-2.5.3/zeta/nn/modules/cross_modal_reparametization.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/decision_tree.py` & `zetascale-2.5.3/zeta/nn/modules/decision_tree.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/deepseek_moe.py` & `zetascale-2.5.3/zeta/nn/modules/deepseek_moe.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/dense_connect.py` & `zetascale-2.5.3/zeta/nn/modules/dense_connect.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/diffusion.py` & `zetascale-2.5.3/zeta/nn/modules/diffusion.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/droppath.py` & `zetascale-2.5.3/zeta/nn/modules/droppath.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/dual_path_block.py` & `zetascale-2.5.3/zeta/nn/modules/dual_path_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/dyna_conv.py` & `zetascale-2.5.3/zeta/nn/modules/dyna_conv.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/dynamic_module.py` & `zetascale-2.5.3/zeta/nn/modules/dynamic_module.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/dynamic_routing_block.py` & `zetascale-2.5.3/zeta/nn/modules/dynamic_routing_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/embedding_to_grid.py` & `zetascale-2.5.3/zeta/nn/modules/embedding_to_grid.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/ether.py` & `zetascale-2.5.3/zeta/nn/modules/ether.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/exo.py` & `zetascale-2.5.3/zeta/nn/modules/exo.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/expand_channels.py` & `zetascale-2.5.3/zeta/nn/modules/expand_channels.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/expert.py` & `zetascale-2.5.3/zeta/nn/modules/expert.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/fast_text.py` & `zetascale-2.5.3/zeta/nn/modules/fast_text.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/feedback_block.py` & `zetascale-2.5.3/zeta/nn/modules/feedback_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/feedforward.py` & `zetascale-2.5.3/zeta/nn/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/feedforward_network.py` & `zetascale-2.5.3/zeta/nn/modules/feedforward_network.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/film.py` & `zetascale-2.5.3/zeta/nn/modules/film.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/film_conditioning.py` & `zetascale-2.5.3/zeta/nn/modules/film_conditioning.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/film_efficient_metb3.py` & `zetascale-2.5.3/zeta/nn/modules/film_efficient_metb3.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/flatten_features.py` & `zetascale-2.5.3/zeta/nn/modules/flatten_features.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/flex_conv.py` & `zetascale-2.5.3/zeta/nn/modules/flex_conv.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/flexible_mlp.py` & `zetascale-2.5.3/zeta/nn/modules/flexible_mlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/fractoral_norm.py` & `zetascale-2.5.3/zeta/nn/modules/fractoral_norm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/fractorial_net.py` & `zetascale-2.5.3/zeta/nn/modules/fractorial_net.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/freeze_layers.py` & `zetascale-2.5.3/zeta/nn/modules/freeze_layers.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/fused_dropout_add.py` & `zetascale-2.5.3/zeta/nn/modules/fused_dropout_add.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/fused_dropout_layernom.py` & `zetascale-2.5.3/zeta/nn/modules/fused_dropout_layernom.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/fused_gelu_dense.py` & `zetascale-2.5.3/zeta/nn/modules/fused_gelu_dense.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/fusion_ffn.py` & `zetascale-2.5.3/zeta/nn/modules/fusion_ffn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/g_shard_moe.py` & `zetascale-2.5.3/zeta/nn/modules/g_shard_moe.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/gated_cnn_block.py` & `zetascale-2.5.3/zeta/nn/modules/gated_cnn_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/gated_residual_block.py` & `zetascale-2.5.3/zeta/nn/modules/gated_residual_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/gill_mapper.py` & `zetascale-2.5.3/zeta/nn/modules/gill_mapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/glu.py` & `zetascale-2.5.3/zeta/nn/modules/glu.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/gru_gating.py` & `zetascale-2.5.3/zeta/nn/modules/gru_gating.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/h3.py` & `zetascale-2.5.3/zeta/nn/modules/h3.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/hebbian.py` & `zetascale-2.5.3/zeta/nn/modules/hebbian.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/highway_layer.py` & `zetascale-2.5.3/zeta/nn/modules/highway_layer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/image_projector.py` & `zetascale-2.5.3/zeta/nn/modules/image_projector.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/image_to_text.py` & `zetascale-2.5.3/zeta/nn/modules/image_to_text.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/img_or_video_to_time.py` & `zetascale-2.5.3/zeta/nn/modules/img_or_video_to_time.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/img_patch_embed.py` & `zetascale-2.5.3/zeta/nn/modules/img_patch_embed.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/img_reshape.py` & `zetascale-2.5.3/zeta/nn/modules/img_reshape.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/itca.py` & `zetascale-2.5.3/zeta/nn/modules/itca.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/kan.py` & `zetascale-2.5.3/zeta/nn/modules/kan.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/kv_cache.py` & `zetascale-2.5.3/zeta/nn/modules/kv_cache.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/kv_cache_update.py` & `zetascale-2.5.3/zeta/nn/modules/kv_cache_update.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/lambda_mask.py` & `zetascale-2.5.3/zeta/nn/modules/lambda_mask.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/lang_conv_module.py` & `zetascale-2.5.3/zeta/nn/modules/lang_conv_module.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/laser.py` & `zetascale-2.5.3/zeta/nn/modules/laser.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/layer_scale.py` & `zetascale-2.5.3/zeta/nn/modules/layer_scale.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/layernorm.py` & `zetascale-2.5.3/zeta/nn/modules/layernorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/leaky_relu.py` & `zetascale-2.5.3/zeta/nn/modules/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/log_ff.py` & `zetascale-2.5.3/zeta/nn/modules/log_ff.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/lora.py` & `zetascale-2.5.3/zeta/nn/modules/lora.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/matrix.py` & `zetascale-2.5.3/zeta/nn/modules/matrix.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/mbconv.py` & `zetascale-2.5.3/zeta/nn/modules/mbconv.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/mixtape.py` & `zetascale-2.5.3/zeta/nn/modules/mixtape.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/mixtral_expert.py` & `zetascale-2.5.3/zeta/nn/modules/mixtral_expert.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/mlp.py` & `zetascale-2.5.3/zeta/nn/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/mlp_mixer.py` & `zetascale-2.5.3/zeta/nn/modules/mlp_mixer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/mm_adapter.py` & `zetascale-2.5.3/zeta/nn/modules/mm_adapter.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/mm_layernorm.py` & `zetascale-2.5.3/zeta/nn/modules/mm_layernorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/mm_ops.py` & `zetascale-2.5.3/zeta/nn/modules/mm_ops.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/modality_adaptive_module.py` & `zetascale-2.5.3/zeta/nn/modules/modality_adaptive_module.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/moe.py` & `zetascale-2.5.3/zeta/nn/modules/moe.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/moe_router.py` & `zetascale-2.5.3/zeta/nn/modules/moe_router.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/monarch_mlp.py` & `zetascale-2.5.3/zeta/nn/modules/monarch_mlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/mr_adapter.py` & `zetascale-2.5.3/zeta/nn/modules/mr_adapter.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/multi_input_multi_output.py` & `zetascale-2.5.3/zeta/nn/modules/multi_input_multi_output.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/multi_scale_block.py` & `zetascale-2.5.3/zeta/nn/modules/multi_scale_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/nebula.py` & `zetascale-2.5.3/zeta/nn/modules/nebula.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/nfn_stem.py` & `zetascale-2.5.3/zeta/nn/modules/nfn_stem.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/norm_fractorals.py` & `zetascale-2.5.3/zeta/nn/modules/norm_fractorals.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/norm_utils.py` & `zetascale-2.5.3/zeta/nn/modules/norm_utils.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/omnimodal_fusion.py` & `zetascale-2.5.3/zeta/nn/modules/omnimodal_fusion.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/p_scan.py` & `zetascale-2.5.3/zeta/nn/modules/p_scan.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/palo_ldp.py` & `zetascale-2.5.3/zeta/nn/modules/palo_ldp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/parallel_wrapper.py` & `zetascale-2.5.3/zeta/nn/modules/parallel_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/patch_linear_flatten.py` & `zetascale-2.5.3/zeta/nn/modules/patch_linear_flatten.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/patch_video.py` & `zetascale-2.5.3/zeta/nn/modules/patch_video.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/peg.py` & `zetascale-2.5.3/zeta/nn/modules/peg.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/perceiver_layer.py` & `zetascale-2.5.3/zeta/nn/modules/perceiver_layer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/perceiver_resampler.py` & `zetascale-2.5.3/zeta/nn/modules/perceiver_resampler.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/pixel_shuffling.py` & `zetascale-2.5.3/zeta/nn/modules/pixel_shuffling.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/poly_expert_fusion_network.py` & `zetascale-2.5.3/zeta/nn/modules/poly_expert_fusion_network.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/polymorphic_activation.py` & `zetascale-2.5.3/zeta/nn/modules/polymorphic_activation.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/polymorphic_neuron.py` & `zetascale-2.5.3/zeta/nn/modules/polymorphic_neuron.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/prenorm.py` & `zetascale-2.5.3/zeta/nn/modules/prenorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/proj_then_softmax.py` & `zetascale-2.5.3/zeta/nn/modules/proj_then_softmax.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/pulsar.py` & `zetascale-2.5.3/zeta/nn/modules/pulsar.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/pyro.py` & `zetascale-2.5.3/zeta/nn/modules/pyro.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/qformer.py` & `zetascale-2.5.3/zeta/nn/modules/qformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/qkv_norm.py` & `zetascale-2.5.3/zeta/nn/modules/qkv_norm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/quantized_layernorm.py` & `zetascale-2.5.3/zeta/nn/modules/quantized_layernorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/query_proposal.py` & `zetascale-2.5.3/zeta/nn/modules/query_proposal.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/recurrent_model.py` & `zetascale-2.5.3/zeta/nn/modules/recurrent_model.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/recursive_block.py` & `zetascale-2.5.3/zeta/nn/modules/recursive_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/res_net.py` & `zetascale-2.5.3/zeta/nn/modules/res_net.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/resnet.py` & `zetascale-2.5.3/zeta/nn/modules/resnet.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/return_loss_text.py` & `zetascale-2.5.3/zeta/nn/modules/return_loss_text.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/rms_norm.py` & `zetascale-2.5.3/zeta/nn/modules/rms_norm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/rnn_nlp.py` & `zetascale-2.5.3/zeta/nn/modules/rnn_nlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/s4.py` & `zetascale-2.5.3/zeta/nn/modules/s4.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/scale.py` & `zetascale-2.5.3/zeta/nn/modules/scale.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/scale_norm.py` & `zetascale-2.5.3/zeta/nn/modules/scale_norm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/scaled_sinusoidal.py` & `zetascale-2.5.3/zeta/nn/modules/scaled_sinusoidal.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/scalenorm.py` & `zetascale-2.5.3/zeta/nn/modules/scalenorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/shift_tokens.py` & `zetascale-2.5.3/zeta/nn/modules/shift_tokens.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/shufflenet.py` & `zetascale-2.5.3/zeta/nn/modules/shufflenet.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/sig_lip.py` & `zetascale-2.5.3/zeta/nn/modules/sig_lip.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/sig_lip_loss.py` & `zetascale-2.5.3/zeta/nn/modules/sig_lip_loss.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/simple_feedforward.py` & `zetascale-2.5.3/zeta/nn/modules/simple_feedforward.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/simple_mamba.py` & `zetascale-2.5.3/zeta/nn/modules/simple_mamba.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/simple_res_block.py` & `zetascale-2.5.3/zeta/nn/modules/simple_res_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/simple_resblock.py` & `zetascale-2.5.3/zeta/nn/modules/simple_resblock.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/simple_rmsnorm.py` & `zetascale-2.5.3/zeta/nn/modules/simple_rmsnorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/skipconnection.py` & `zetascale-2.5.3/zeta/nn/modules/skipconnection.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/slerp_model_merger.py` & `zetascale-2.5.3/zeta/nn/modules/slerp_model_merger.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/sp_act.py` & `zetascale-2.5.3/zeta/nn/modules/sp_act.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/space_time_unet.py` & `zetascale-2.5.3/zeta/nn/modules/space_time_unet.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/spacial_transformer.py` & `zetascale-2.5.3/zeta/nn/modules/spacial_transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/sparq_attn.py` & `zetascale-2.5.3/zeta/nn/modules/sparq_attn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/sparse_moe.py` & `zetascale-2.5.3/zeta/nn/modules/sparse_moe.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/sparse_token_integration.py` & `zetascale-2.5.3/zeta/nn/modules/sparse_token_integration.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/spatial_downsample.py` & `zetascale-2.5.3/zeta/nn/modules/spatial_downsample.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/spatial_transformer.py` & `zetascale-2.5.3/zeta/nn/modules/spatial_transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/splines.py` & `zetascale-2.5.3/zeta/nn/modules/splines.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/squeeze_excitation.py` & `zetascale-2.5.3/zeta/nn/modules/squeeze_excitation.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/ssm.py` & `zetascale-2.5.3/zeta/nn/modules/ssm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/ssm_language.py` & `zetascale-2.5.3/zeta/nn/modules/ssm_language.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/stoch_depth.py` & `zetascale-2.5.3/zeta/nn/modules/stoch_depth.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/stochastic_depth.py` & `zetascale-2.5.3/zeta/nn/modules/stochastic_depth.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/subln.py` & `zetascale-2.5.3/zeta/nn/modules/subln.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/super_resolution.py` & `zetascale-2.5.3/zeta/nn/modules/super_resolution.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/swarmalator.py` & `zetascale-2.5.3/zeta/nn/modules/swarmalator.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/swiglu.py` & `zetascale-2.5.3/zeta/nn/modules/swiglu.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/tensor.py` & `zetascale-2.5.3/zeta/nn/modules/tensor.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/tensor_to_int.py` & `zetascale-2.5.3/zeta/nn/modules/tensor_to_int.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/text_scene_fusion.py` & `zetascale-2.5.3/zeta/nn/modules/text_scene_fusion.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/text_video_fuse.py` & `zetascale-2.5.3/zeta/nn/modules/text_video_fuse.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/time_up_sample.py` & `zetascale-2.5.3/zeta/nn/modules/time_up_sample.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/to_logits.py` & `zetascale-2.5.3/zeta/nn/modules/to_logits.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/token_learner.py` & `zetascale-2.5.3/zeta/nn/modules/token_learner.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/token_mixer.py` & `zetascale-2.5.3/zeta/nn/modules/token_mixer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/top_n_gating.py` & `zetascale-2.5.3/zeta/nn/modules/top_n_gating.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/transformations.py` & `zetascale-2.5.3/zeta/nn/modules/transformations.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/triple_skip.py` & `zetascale-2.5.3/zeta/nn/modules/triple_skip.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/triton_rmsnorm.py` & `zetascale-2.5.3/zeta/nn/modules/triton_rmsnorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/u_mamba.py` & `zetascale-2.5.3/zeta/nn/modules/u_mamba.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/unet.py` & `zetascale-2.5.3/zeta/nn/modules/unet.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/v_layernorm.py` & `zetascale-2.5.3/zeta/nn/modules/v_layernorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/v_pool.py` & `zetascale-2.5.3/zeta/nn/modules/v_pool.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/video_autoencoder.py` & `zetascale-2.5.3/zeta/nn/modules/video_autoencoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/video_diffusion_modules.py` & `zetascale-2.5.3/zeta/nn/modules/video_diffusion_modules.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/video_to_tensor.py` & `zetascale-2.5.3/zeta/nn/modules/video_to_tensor.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/video_to_text.py` & `zetascale-2.5.3/zeta/nn/modules/video_to_text.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/vision_mamba.py` & `zetascale-2.5.3/zeta/nn/modules/vision_mamba.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/vision_weighted_permute_mlp.py` & `zetascale-2.5.3/zeta/nn/modules/vision_weighted_permute_mlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/visual_expert.py` & `zetascale-2.5.3/zeta/nn/modules/visual_expert.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/vit_denoiser.py` & `zetascale-2.5.3/zeta/nn/modules/vit_denoiser.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/vss_block.py` & `zetascale-2.5.3/zeta/nn/modules/vss_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/ws_conv2d.py` & `zetascale-2.5.3/zeta/nn/modules/ws_conv2d.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/xmoe/global_groups.py` & `zetascale-2.5.3/zeta/nn/modules/xmoe/global_groups.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/xmoe/moe_layer.py` & `zetascale-2.5.3/zeta/nn/modules/xmoe/moe_layer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/xmoe/routing.py` & `zetascale-2.5.3/zeta/nn/modules/xmoe/routing.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/nn/modules/yolo.py` & `zetascale-2.5.3/zeta/nn/modules/yolo.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/ops/__Init__.py` & `zetascale-2.5.3/zeta/ops/__Init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/ops/async_softmax.py` & `zetascale-2.5.3/zeta/ops/async_softmax.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/ops/dilated_attn_ops.py` & `zetascale-2.5.3/zeta/ops/dilated_attn_ops.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/ops/einops_from_to.py` & `zetascale-2.5.3/zeta/ops/einops_from_to.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/ops/einops_poly.py` & `zetascale-2.5.3/zeta/ops/einops_poly.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/ops/expand.py` & `zetascale-2.5.3/zeta/ops/expand.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/ops/laplace.py` & `zetascale-2.5.3/zeta/ops/laplace.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/ops/main.py` & `zetascale-2.5.3/zeta/ops/main.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/ops/misc_act.py` & `zetascale-2.5.3/zeta/ops/misc_act.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/ops/mm_rearranges.py` & `zetascale-2.5.3/zeta/ops/mm_rearranges.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/ops/mm_softmax.py` & `zetascale-2.5.3/zeta/ops/mm_softmax.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/ops/mos.py` & `zetascale-2.5.3/zeta/ops/mos.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/ops/nonlinear.py` & `zetascale-2.5.3/zeta/ops/nonlinear.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/ops/softmax.py` & `zetascale-2.5.3/zeta/ops/softmax.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/ops/sparsemax.py` & `zetascale-2.5.3/zeta/ops/sparsemax.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/optim/__init__.py` & `zetascale-2.5.3/zeta/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/optim/batched_optimizer.py` & `zetascale-2.5.3/zeta/optim/batched_optimizer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/optim/decoupled_lion.py` & `zetascale-2.5.3/zeta/optim/decoupled_lion.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/optim/decoupled_optimizer.py` & `zetascale-2.5.3/zeta/optim/decoupled_optimizer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/optim/decoupled_sophia.py` & `zetascale-2.5.3/zeta/optim/decoupled_sophia.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/optim/gradient_ascent.py` & `zetascale-2.5.3/zeta/optim/gradient_ascent.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/optim/gradient_equillibrum.py` & `zetascale-2.5.3/zeta/optim/gradient_equillibrum.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/optim/lion8b.py` & `zetascale-2.5.3/zeta/optim/lion8b.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/optim/parallel_gradient_descent.py` & `zetascale-2.5.3/zeta/optim/parallel_gradient_descent.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/optim/stable_adam.py` & `zetascale-2.5.3/zeta/optim/stable_adam.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/quant/bitlinear.py` & `zetascale-2.5.3/zeta/quant/bitlinear.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/quant/half_bit_linear.py` & `zetascale-2.5.3/zeta/quant/half_bit_linear.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/quant/lfq.py` & `zetascale-2.5.3/zeta/quant/lfq.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/quant/niva.py` & `zetascale-2.5.3/zeta/quant/niva.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/quant/qlora.py` & `zetascale-2.5.3/zeta/quant/qlora.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 from typing import Tuple
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from scipy.stats import norm
+# from scipy.stats import norm
 from tqdm import tqdm
 
 bnb_available = False
 
 
 def get_block_absmax(
     inpt_tensor: torch.Tensor, block_size: int
@@ -358,17 +358,17 @@
                     0.5626,
                     0.7230,
                     1.0000,
                 ]
             )
 
         offset = 0.9677083
-        v1 = norm.ppf(torch.linspace(offset, 0.5, 9)[:-1]).tolist()
+        v1 = torch.linspace(offset, 0.5, 9)[:-1].tolist()
         # v2 = [0]*(256-15)
-        v3 = (-norm.ppf(torch.linspace(offset, 0.5, 8)[:-1])).tolist()
+        v3 = (torch.linspace(offset, 0.5, 8)[:-1]).tolist()
         # v = v1 + v3 + 0.0
         nkf = torch.tensor(v1 + v3 + [0.0])
         nkf = nkf.sort().values
         nkf /= nkf.max()
         return nkf
 
     @staticmethod
```

### Comparing `zetascale-2.5.1/zeta/quant/qmoe.py` & `zetascale-2.5.3/zeta/quant/qmoe.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/quant/quick.py` & `zetascale-2.5.3/zeta/quant/quick.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/quant/residual_vq.py` & `zetascale-2.5.3/zeta/quant/residual_vq.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/quant/ste.py` & `zetascale-2.5.3/zeta/quant/ste.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/rl/__init__.py` & `zetascale-2.5.3/zeta/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/rl/actor_critic.py` & `zetascale-2.5.3/zeta/rl/actor_critic.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/rl/dpo.py` & `zetascale-2.5.3/zeta/rl/dpo.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/rl/hindsight_replay.py` & `zetascale-2.5.3/zeta/rl/hindsight_replay.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/rl/language_reward.py` & `zetascale-2.5.3/zeta/rl/language_reward.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/rl/ppo.py` & `zetascale-2.5.3/zeta/rl/ppo.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/rl/priortized_replay_buffer.py` & `zetascale-2.5.3/zeta/rl/priortized_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/rl/priortized_rps.py` & `zetascale-2.5.3/zeta/rl/priortized_rps.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/rl/reward_model.py` & `zetascale-2.5.3/zeta/rl/reward_model.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/rl/sumtree.py` & `zetascale-2.5.3/zeta/rl/sumtree.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/rl/vision_model_rl.py` & `zetascale-2.5.3/zeta/rl/vision_model_rl.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/structs/__init__.py` & `zetascale-2.5.3/zeta/structs/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/structs/auto_regressive_wrapper.py` & `zetascale-2.5.3/zeta/structs/auto_regressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/structs/clip_encoder.py` & `zetascale-2.5.3/zeta/structs/clip_encoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/structs/efficient_net.py` & `zetascale-2.5.3/zeta/structs/efficient_net.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/structs/encoder_decoder.py` & `zetascale-2.5.3/zeta/structs/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/structs/hierarchical_transformer.py` & `zetascale-2.5.3/zeta/structs/hierarchical_transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/structs/local_transformer.py` & `zetascale-2.5.3/zeta/structs/local_transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/structs/multi_modal_projector.py` & `zetascale-2.5.3/zeta/structs/multi_modal_projector.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/structs/simple_transformer.py` & `zetascale-2.5.3/zeta/structs/simple_transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/structs/simple_vision_encoder.py` & `zetascale-2.5.3/zeta/structs/simple_vision_encoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/structs/transformer.py` & `zetascale-2.5.3/zeta/structs/transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/structs/transformer_block.py` & `zetascale-2.5.3/zeta/structs/transformer_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/tokenizers/gptx_tokenizer.py` & `zetascale-2.5.3/zeta/tokenizers/gptx_tokenizer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/tokenizers/llama_sentencepiece.py` & `zetascale-2.5.3/zeta/tokenizers/llama_sentencepiece.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/tokenizers/multi_modal_tokenizer.py` & `zetascale-2.5.3/zeta/tokenizers/multi_modal_tokenizer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/tokenizers/sentence_piece.py` & `zetascale-2.5.3/zeta/tokenizers/sentence_piece.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/tokenizers/tokenmonster.py` & `zetascale-2.5.3/zeta/tokenizers/tokenmonster.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/training/activation_checkpoint.py` & `zetascale-2.5.3/zeta/training/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/training/dataloader.py` & `zetascale-2.5.3/zeta/training/dataloader.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/training/fsdp.py` & `zetascale-2.5.3/zeta/training/fsdp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/training/galore.py` & `zetascale-2.5.3/zeta/training/galore.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/training/hive_trainer.py` & `zetascale-2.5.3/zeta/training/hive_trainer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/training/parallel_wrapper.py` & `zetascale-2.5.3/zeta/training/parallel_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/training/scheduler.py` & `zetascale-2.5.3/zeta/training/scheduler.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/training/train.py` & `zetascale-2.5.3/zeta/training/train.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/utils/__init__.py` & `zetascale-2.5.3/zeta/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/utils/benchmark.py` & `zetascale-2.5.3/zeta/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/utils/cuda_memory_wrapper.py` & `zetascale-2.5.3/zeta/utils/cuda_memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/utils/cuda_wrapper.py` & `zetascale-2.5.3/zeta/utils/cuda_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/utils/disable_logging.py` & `zetascale-2.5.3/zeta/utils/disable_logging.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/utils/enforce_types.py` & `zetascale-2.5.3/zeta/utils/enforce_types.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/utils/img_to_tensor.py` & `zetascale-2.5.3/zeta/utils/img_to_tensor.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/utils/log_pytorch_op.py` & `zetascale-2.5.3/zeta/utils/log_pytorch_op.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/utils/main.py` & `zetascale-2.5.3/zeta/utils/main.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/utils/module_device.py` & `zetascale-2.5.3/zeta/utils/module_device.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/utils/params.py` & `zetascale-2.5.3/zeta/utils/params.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/utils/save_load_wrapper.py` & `zetascale-2.5.3/zeta/utils/save_load_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/utils/text_to_tensor.py` & `zetascale-2.5.3/zeta/utils/text_to_tensor.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/utils/verbose_execution.py` & `zetascale-2.5.3/zeta/utils/verbose_execution.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/zeta/utils/vision_utils.py` & `zetascale-2.5.3/zeta/utils/vision_utils.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.5.1/PKG-INFO` & `zetascale-2.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zetascale
-Version: 2.5.1
+Version: 2.5.3
 Summary: Rapidly Build, Optimize, and Deploy SOTA AI Models
 Home-page: https://github.com/kyegomez/zeta
 License: MIT
 Keywords: Transformers,zeta scale
 Author: Zeta Team
 Author-email: kye@apac.ai
 Requires-Python: >=3.10,<4.0
@@ -21,15 +21,14 @@
 Requires-Dist: datasets
 Requires-Dist: einops (==0.7.0)
 Requires-Dist: einops-exts (==0.0.4)
 Requires-Dist: local-attention
 Requires-Dist: loguru
 Requires-Dist: pytest (==8.2.1)
 Requires-Dist: rich (==13.7.1)
-Requires-Dist: scipy (==1.9.3)
 Requires-Dist: torch (>=2.1.1,<3.0)
 Requires-Dist: torchfix
 Requires-Dist: torchvision (==0.18.0)
 Requires-Dist: tqdm (==4.66.3)
 Requires-Dist: transformers (==4.41.0)
 Requires-Dist: vector-quantize-pytorch (==1.14.7)
 Description-Content-Type: text/markdown
```

