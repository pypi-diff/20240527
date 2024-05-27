# Comparing `tmp/fermo_core-0.2.0.tar.gz` & `tmp/fermo_core-0.2.1.tar.gz`

## Comparing `fermo_core-0.2.0.tar` & `fermo_core-0.2.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 fermo_core-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/__init__.py
--rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/config/__init__.py
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/config/class_default_settings.py
--rw-r--r--   0        0        0    42886 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/config/schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/__init__.py
--rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/class_analysis_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/__init__.py
--rw-r--r--   0        0        0    51559 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_adduct_annotator.py
--rw-r--r--   0        0        0    20380 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_annotation_manager.py
--rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_fragment_annotator.py
--rw-r--r--   0        0        0    11491 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_mod_cos_annotator.py
--rw-r--r--   0        0        0    11818 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_ms2deepscore_annotator.py
--rw-r--r--   0        0        0    12875 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_ms2query_annotator.py
--rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_neutral_loss_annotator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/blank_assigner/__init__.py
--rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/blank_assigner/class_blank_assigner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/chrom_trace_calculator/__init__.py
--rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/chrom_trace_calculator/class_chrom_trace_calculator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/feature_filter/__init__.py
--rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/feature_filter/class_feature_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/group_assigner/__init__.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/group_assigner/class_group_assigner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/group_factor_assigner/__init__.py
--rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/group_factor_assigner/class_group_factor_assigner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/__init__.py
--rw-r--r--   0        0        0     7275 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/class_phen_qual_assigner.py
--rw-r--r--   0        0        0     6681 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/class_phen_quant_conc_assigner.py
--rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/class_phen_quant_perc_assigner.py
--rw-r--r--   0        0        0     7113 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/class_phenotype_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/score_assigner/__init__.py
--rw-r--r--   0        0        0     6718 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/score_assigner/class_score_assigner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/sim_networks_manager/__init__.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/sim_networks_manager/class_mod_cosine_networker.py
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/sim_networks_manager/class_ms2deepscore_networker.py
--rw-r--r--   0        0        0    13360 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/sim_networks_manager/class_sim_networks_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/__init__.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/class_repository.py
--rw-r--r--   0        0        0     9501 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/class_stats.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_feature/__init__.py
--rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_feature/class_feature_builder.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_feature/class_general_feature_director.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_feature/class_specific_feature_director.py
--rw-r--r--   0        0        0    15027 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_feature/dataclass_feature.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_sample/__init__.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_sample/class_sample_builder.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_sample/class_samples_director.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_sample/dataclass_sample.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/__init__.py
--rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/class_general_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/group_metadata_parser/__init__.py
--rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/group_metadata_parser/class_fermo_metadata_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/msms_parser/__init__.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/msms_parser/class_mgf_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/peaktable_parser/__init__.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/peaktable_parser/abc_peaktable_parser.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/peaktable_parser/class_mzmine3_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/phenotype_parser/__init__.py
--rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/phenotype_parser/class_phenotype_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/spec_library_parser/__init__.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/spec_library_parser/class_spec_lib_mgf_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/__init__.py
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/additional_module_parameter_managers.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/class_argparse_manager.py
--rw-r--r--   0        0        0    19464 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/class_export_manager.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/class_file_manager.py
--rw-r--r--   0        0        0    35890 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/class_parameter_manager.py
--rw-r--r--   0        0        0    20145 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/class_summary_writer.py
--rw-r--r--   0        0        0    15453 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/class_validation_manager.py
--rw-r--r--   0        0        0     7717 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/core_module_parameter_managers.py
--rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/input_file_parameter_managers.py
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/output_file_parameter_managers.py
--rw-r--r--   0        0        0    11013 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/frag_libs/aa_m+h_fragment_series.csv
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/loss_libs/generic_bio_pos.csv
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/loss_libs/generic_other_neg.csv
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/loss_libs/generic_other_pos.csv
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/loss_libs/kersten_glycosides.csv
--rw-r--r--   0        0        0    14072 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/loss_libs/kersten_nonribosomal.csv
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/loss_libs/kersten_ribosomal.csv
--rw-r--r--   0        0        0    34102 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/mibig/mibig_cds_count.csv
--rw-r--r--   0        0        0  2878179 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/mibig/pos/mibig_in_silico_spectral_library_3_1.mgf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/ms2deepscore/pos/.placeholder
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/ms2query/neg/.placeholder
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/ms2query/pos/.placeholder
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/utils/__init__.py
--rw-r--r--   0        0        0    12500 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/utils/utility_method_manager.py
--rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 fermo_core-0.2.0/.gitignore
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 fermo_core-0.2.0/LICENSE
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 fermo_core-0.2.0/README.md
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 fermo_core-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 fermo_core-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 fermo_core-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/__init__.py
+-rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/config/__init__.py
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/config/class_default_settings.py
+-rw-r--r--   0        0        0    42886 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/config/schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/__init__.py
+-rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/class_analysis_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/annotation_manager/__init__.py
+-rw-r--r--   0        0        0    51559 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/annotation_manager/class_adduct_annotator.py
+-rw-r--r--   0        0        0    20380 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/annotation_manager/class_annotation_manager.py
+-rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/annotation_manager/class_fragment_annotator.py
+-rw-r--r--   0        0        0    11491 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/annotation_manager/class_mod_cos_annotator.py
+-rw-r--r--   0        0        0    11818 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/annotation_manager/class_ms2deepscore_annotator.py
+-rw-r--r--   0        0        0    12875 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/annotation_manager/class_ms2query_annotator.py
+-rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/annotation_manager/class_neutral_loss_annotator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/blank_assigner/__init__.py
+-rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/blank_assigner/class_blank_assigner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/chrom_trace_calculator/__init__.py
+-rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/chrom_trace_calculator/class_chrom_trace_calculator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/feature_filter/__init__.py
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/feature_filter/class_feature_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/group_assigner/__init__.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/group_assigner/class_group_assigner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/group_factor_assigner/__init__.py
+-rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/group_factor_assigner/class_group_factor_assigner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/phenotype_manager/__init__.py
+-rw-r--r--   0        0        0     7275 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/phenotype_manager/class_phen_qual_assigner.py
+-rw-r--r--   0        0        0     6681 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/phenotype_manager/class_phen_quant_conc_assigner.py
+-rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/phenotype_manager/class_phen_quant_perc_assigner.py
+-rw-r--r--   0        0        0     7113 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/phenotype_manager/class_phenotype_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/score_assigner/__init__.py
+-rw-r--r--   0        0        0     6718 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/score_assigner/class_score_assigner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/sim_networks_manager/__init__.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/sim_networks_manager/class_mod_cosine_networker.py
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/sim_networks_manager/class_ms2deepscore_networker.py
+-rw-r--r--   0        0        0    13360 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_analysis/sim_networks_manager/class_sim_networks_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/__init__.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/class_repository.py
+-rw-r--r--   0        0        0     9501 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/class_stats.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/builder_feature/__init__.py
+-rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/builder_feature/class_feature_builder.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/builder_feature/class_general_feature_director.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/builder_feature/class_specific_feature_director.py
+-rw-r--r--   0        0        0    15027 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/builder_feature/dataclass_feature.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/builder_sample/__init__.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/builder_sample/class_sample_builder.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/builder_sample/class_samples_director.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/builder_sample/dataclass_sample.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/parser/__init__.py
+-rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/parser/class_general_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/parser/group_metadata_parser/__init__.py
+-rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/parser/group_metadata_parser/class_fermo_metadata_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/parser/msms_parser/__init__.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/parser/msms_parser/class_mgf_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/parser/peaktable_parser/__init__.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/parser/peaktable_parser/abc_peaktable_parser.py
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/parser/peaktable_parser/class_mzmine3_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/parser/phenotype_parser/__init__.py
+-rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/parser/phenotype_parser/class_phenotype_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/parser/spec_library_parser/__init__.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/data_processing/parser/spec_library_parser/class_spec_lib_mgf_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/input_output/__init__.py
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/input_output/additional_module_parameter_managers.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/input_output/class_argparse_manager.py
+-rw-r--r--   0        0        0    19464 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/input_output/class_export_manager.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/input_output/class_file_manager.py
+-rw-r--r--   0        0        0    35890 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/input_output/class_parameter_manager.py
+-rw-r--r--   0        0        0    20500 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/input_output/class_summary_writer.py
+-rw-r--r--   0        0        0    15453 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/input_output/class_validation_manager.py
+-rw-r--r--   0        0        0     7717 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/input_output/core_module_parameter_managers.py
+-rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/input_output/input_file_parameter_managers.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/input_output/output_file_parameter_managers.py
+-rw-r--r--   0        0        0    11013 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/libraries/frag_libs/aa_m+h_fragment_series.csv
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/libraries/loss_libs/generic_bio_pos.csv
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/libraries/loss_libs/generic_other_neg.csv
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/libraries/loss_libs/generic_other_pos.csv
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/libraries/loss_libs/kersten_glycosides.csv
+-rw-r--r--   0        0        0    14072 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/libraries/loss_libs/kersten_nonribosomal.csv
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/libraries/loss_libs/kersten_ribosomal.csv
+-rw-r--r--   0        0        0    34102 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/libraries/mibig/mibig_cds_count.csv
+-rw-r--r--   0        0        0  2878179 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/libraries/mibig/pos/mibig_in_silico_spectral_library_3_1.mgf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/libraries/ms2deepscore/pos/.placeholder
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/libraries/ms2query/neg/.placeholder
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/libraries/ms2query/pos/.placeholder
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/utils/__init__.py
+-rw-r--r--   0        0        0    12500 2020-02-02 00:00:00.000000 fermo_core-0.2.1/fermo_core/utils/utility_method_manager.py
+-rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 fermo_core-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 fermo_core-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 fermo_core-0.2.1/README.md
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 fermo_core-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 fermo_core-0.2.1/PKG-INFO
```

### Comparing `fermo_core-0.2.0/CHANGELOG.md` & `fermo_core-0.2.1/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
 ## Unreleased
 
 N/A
 
+## [0.2.1] 26-05-2024
+
+### Fixed
+
+- Fixed bug in "SummaryWriter": implemented error catching.
+
 ## [0.2.0] 26-05-2024
 
 ### Changed
 
 - Replaced global logger with logger specific for `main_cli()`. `main()` now needs an argument `logger`
 - Reworked output file naming: all output files now start with `out.fermo.` and a suffix specifying their type
 - Removed output directory selection: the output directory is now always `results` located in the directory in which the peaktable resides.
```

### Comparing `fermo_core-0.2.0/fermo_core/main.py` & `fermo_core-0.2.1/fermo_core/main.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/config/class_default_settings.py` & `fermo_core-0.2.1/fermo_core/config/class_default_settings.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/config/schema.json` & `fermo_core-0.2.1/fermo_core/config/schema.json`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/class_analysis_manager.py` & `fermo_core-0.2.1/fermo_core/data_analysis/class_analysis_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_adduct_annotator.py` & `fermo_core-0.2.1/fermo_core/data_analysis/annotation_manager/class_adduct_annotator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_annotation_manager.py` & `fermo_core-0.2.1/fermo_core/data_analysis/annotation_manager/class_annotation_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_fragment_annotator.py` & `fermo_core-0.2.1/fermo_core/data_analysis/annotation_manager/class_fragment_annotator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_mod_cos_annotator.py` & `fermo_core-0.2.1/fermo_core/data_analysis/annotation_manager/class_mod_cos_annotator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_ms2deepscore_annotator.py` & `fermo_core-0.2.1/fermo_core/data_analysis/annotation_manager/class_ms2deepscore_annotator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_ms2query_annotator.py` & `fermo_core-0.2.1/fermo_core/data_analysis/annotation_manager/class_ms2query_annotator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_neutral_loss_annotator.py` & `fermo_core-0.2.1/fermo_core/data_analysis/annotation_manager/class_neutral_loss_annotator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/blank_assigner/class_blank_assigner.py` & `fermo_core-0.2.1/fermo_core/data_analysis/blank_assigner/class_blank_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/chrom_trace_calculator/class_chrom_trace_calculator.py` & `fermo_core-0.2.1/fermo_core/data_analysis/chrom_trace_calculator/class_chrom_trace_calculator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/feature_filter/class_feature_filter.py` & `fermo_core-0.2.1/fermo_core/data_analysis/feature_filter/class_feature_filter.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/group_assigner/class_group_assigner.py` & `fermo_core-0.2.1/fermo_core/data_analysis/group_assigner/class_group_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/group_factor_assigner/class_group_factor_assigner.py` & `fermo_core-0.2.1/fermo_core/data_analysis/group_factor_assigner/class_group_factor_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/class_phen_qual_assigner.py` & `fermo_core-0.2.1/fermo_core/data_analysis/phenotype_manager/class_phen_qual_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/class_phen_quant_conc_assigner.py` & `fermo_core-0.2.1/fermo_core/data_analysis/phenotype_manager/class_phen_quant_conc_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/class_phen_quant_perc_assigner.py` & `fermo_core-0.2.1/fermo_core/data_analysis/phenotype_manager/class_phen_quant_perc_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/class_phenotype_manager.py` & `fermo_core-0.2.1/fermo_core/data_analysis/phenotype_manager/class_phenotype_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/score_assigner/class_score_assigner.py` & `fermo_core-0.2.1/fermo_core/data_analysis/score_assigner/class_score_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/sim_networks_manager/class_mod_cosine_networker.py` & `fermo_core-0.2.1/fermo_core/data_analysis/sim_networks_manager/class_mod_cosine_networker.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/sim_networks_manager/class_ms2deepscore_networker.py` & `fermo_core-0.2.1/fermo_core/data_analysis/sim_networks_manager/class_ms2deepscore_networker.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_analysis/sim_networks_manager/class_sim_networks_manager.py` & `fermo_core-0.2.1/fermo_core/data_analysis/sim_networks_manager/class_sim_networks_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_processing/class_repository.py` & `fermo_core-0.2.1/fermo_core/data_processing/class_repository.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_processing/class_stats.py` & `fermo_core-0.2.1/fermo_core/data_processing/class_stats.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_processing/builder_feature/class_feature_builder.py` & `fermo_core-0.2.1/fermo_core/data_processing/builder_feature/class_feature_builder.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_processing/builder_feature/class_general_feature_director.py` & `fermo_core-0.2.1/fermo_core/data_processing/builder_feature/class_general_feature_director.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_processing/builder_feature/class_specific_feature_director.py` & `fermo_core-0.2.1/fermo_core/data_processing/builder_feature/class_specific_feature_director.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_processing/builder_feature/dataclass_feature.py` & `fermo_core-0.2.1/fermo_core/data_processing/builder_feature/dataclass_feature.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_processing/builder_sample/class_sample_builder.py` & `fermo_core-0.2.1/fermo_core/data_processing/builder_sample/class_sample_builder.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_processing/builder_sample/class_samples_director.py` & `fermo_core-0.2.1/fermo_core/data_processing/builder_sample/class_samples_director.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_processing/builder_sample/dataclass_sample.py` & `fermo_core-0.2.1/fermo_core/data_processing/builder_sample/dataclass_sample.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_processing/parser/class_general_parser.py` & `fermo_core-0.2.1/fermo_core/data_processing/parser/class_general_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_processing/parser/group_metadata_parser/class_fermo_metadata_parser.py` & `fermo_core-0.2.1/fermo_core/data_processing/parser/group_metadata_parser/class_fermo_metadata_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_processing/parser/msms_parser/class_mgf_parser.py` & `fermo_core-0.2.1/fermo_core/data_processing/parser/msms_parser/class_mgf_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_processing/parser/peaktable_parser/abc_peaktable_parser.py` & `fermo_core-0.2.1/fermo_core/data_processing/parser/peaktable_parser/abc_peaktable_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_processing/parser/peaktable_parser/class_mzmine3_parser.py` & `fermo_core-0.2.1/fermo_core/data_processing/parser/peaktable_parser/class_mzmine3_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_processing/parser/phenotype_parser/class_phenotype_parser.py` & `fermo_core-0.2.1/fermo_core/data_processing/parser/phenotype_parser/class_phenotype_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/data_processing/parser/spec_library_parser/class_spec_lib_mgf_parser.py` & `fermo_core-0.2.1/fermo_core/data_processing/parser/spec_library_parser/class_spec_lib_mgf_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/input_output/additional_module_parameter_managers.py` & `fermo_core-0.2.1/fermo_core/input_output/additional_module_parameter_managers.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/input_output/class_argparse_manager.py` & `fermo_core-0.2.1/fermo_core/input_output/class_argparse_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/input_output/class_export_manager.py` & `fermo_core-0.2.1/fermo_core/input_output/class_export_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/input_output/class_file_manager.py` & `fermo_core-0.2.1/fermo_core/input_output/class_file_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/input_output/class_parameter_manager.py` & `fermo_core-0.2.1/fermo_core/input_output/class_parameter_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/input_output/class_summary_writer.py` & `fermo_core-0.2.1/fermo_core/input_output/class_summary_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,17 +129,17 @@
                     f" in at least one sample (relative to the feature with the "
                     f"highest intensity(height) in the sample)."
                 )
             if self.params.FeatureFilteringParameters.filter_rel_area_range is not None:
                 self.summary.append(
                     f"Molecular features were filtered and only retained if they were "
                     f"inside the relative area range of "
-                    f"'{self.params.FeatureFilteringParameters.filter_rel_int_range[0]}"
+                    f"'{self.params.FeatureFilteringParameters.filter_rel_area_range[0]}"
                     f"-"
-                    f"{self.params.FeatureFilteringParameters.filter_rel_int_range[1]}'"
+                    f"{self.params.FeatureFilteringParameters.filter_rel_area_range[1]}'"
                     f" in at least one sample (relative to the feature with the "
                     f"highest area in the sample)."
                 )
 
     def summarize_adductannotationparameters(self: Self):
         if self.params.AdductAnnotationParameters.activate_module:
             self.summary.append(
@@ -345,34 +345,41 @@
                 f"and the maximum precursor m/z difference of "
                 f"'{self.params.AsKcbDeepscoreMatchingParams.max_precursor_mass_diff}"
                 f"' was not exceeded."
             )
 
     def assemble_summary(self: Self):
         """Call methods to assemble the summary file"""
-        logger.debug("'SummaryWriter': Started summary: files")
-        self.summarize_peaktableparameters()
-        self.summarize_msmsparameters()
-        self.summarize_phenotypeparameters()
-        self.summarize_groupmetadataparameters()
-        self.summarize_speclibparameters()
-        self.summarize_ms2queryresultsparameters()
-        self.summarize_asresultsparameters()
-        logger.debug("'SummaryWriter': Completed summary: files")
-        logger.debug("'SummaryWriter': Started summary: analysis modules")
-        self.summarize_featurefilteringparameters()
-        self.summarize_adductannotationparameters()
-        self.summarize_neutrallossparameters()
-        self.summarize_fragmentannparameters()
-        self.summarize_specsimnetworkcosineparameters()
-        self.summarize_specsimnetworkdeepscoreparameters()
-        self.summarize_blankassignmentparameters()
-        self.summarize_groupfactassignmentparameters()
-        self.summarize_phenoqualassgnparams()
-        self.summarize_phenoquantpercentassgnparams()
-        self.summarize_phenoquantconcassgnparams()
-        self.summarize_spectrallibmatchingcosineparameters()
-        self.summarize_spectrallibmatchingdeepscoreparameters()
-        self.summarize_ms2queryannotationparameters()
-        self.summarize_askcbcosinematchingparams()
-        self.summarize_askcbdeepscorematchingparams()
-        logger.debug("'SummaryWriter': Completed summary: analysis modules")
+        try:
+            logger.debug("'SummaryWriter': Started summary: files")
+            self.summarize_peaktableparameters()
+            self.summarize_msmsparameters()
+            self.summarize_phenotypeparameters()
+            self.summarize_groupmetadataparameters()
+            self.summarize_speclibparameters()
+            self.summarize_ms2queryresultsparameters()
+            self.summarize_asresultsparameters()
+            logger.debug("'SummaryWriter': Completed summary: files")
+            logger.debug("'SummaryWriter': Started summary: analysis modules")
+            self.summarize_featurefilteringparameters()
+            self.summarize_adductannotationparameters()
+            self.summarize_neutrallossparameters()
+            self.summarize_fragmentannparameters()
+            self.summarize_specsimnetworkcosineparameters()
+            self.summarize_specsimnetworkdeepscoreparameters()
+            self.summarize_blankassignmentparameters()
+            self.summarize_groupfactassignmentparameters()
+            self.summarize_phenoqualassgnparams()
+            self.summarize_phenoquantpercentassgnparams()
+            self.summarize_phenoquantconcassgnparams()
+            self.summarize_spectrallibmatchingcosineparameters()
+            self.summarize_spectrallibmatchingdeepscoreparameters()
+            self.summarize_ms2queryannotationparameters()
+            self.summarize_askcbcosinematchingparams()
+            self.summarize_askcbdeepscorematchingparams()
+            logger.debug("'SummaryWriter': Completed summary: analysis modules")
+        except Exception as e:
+            logger.error(str(e))
+            logger.error(
+                "SummaryWriter: error occurred during writing of summary. "
+                "Write steps until error occurred."
+            )
```

### Comparing `fermo_core-0.2.0/fermo_core/input_output/class_validation_manager.py` & `fermo_core-0.2.1/fermo_core/input_output/class_validation_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/input_output/core_module_parameter_managers.py` & `fermo_core-0.2.1/fermo_core/input_output/core_module_parameter_managers.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/input_output/input_file_parameter_managers.py` & `fermo_core-0.2.1/fermo_core/input_output/input_file_parameter_managers.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/input_output/output_file_parameter_managers.py` & `fermo_core-0.2.1/fermo_core/input_output/output_file_parameter_managers.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/libraries/frag_libs/aa_m+h_fragment_series.csv` & `fermo_core-0.2.1/fermo_core/libraries/frag_libs/aa_m+h_fragment_series.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/libraries/loss_libs/generic_bio_pos.csv` & `fermo_core-0.2.1/fermo_core/libraries/loss_libs/generic_bio_pos.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/libraries/loss_libs/generic_other_neg.csv` & `fermo_core-0.2.1/fermo_core/libraries/loss_libs/generic_other_neg.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/libraries/loss_libs/generic_other_pos.csv` & `fermo_core-0.2.1/fermo_core/libraries/loss_libs/generic_other_pos.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/libraries/loss_libs/kersten_glycosides.csv` & `fermo_core-0.2.1/fermo_core/libraries/loss_libs/kersten_glycosides.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/libraries/loss_libs/kersten_nonribosomal.csv` & `fermo_core-0.2.1/fermo_core/libraries/loss_libs/kersten_nonribosomal.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/libraries/loss_libs/kersten_ribosomal.csv` & `fermo_core-0.2.1/fermo_core/libraries/loss_libs/kersten_ribosomal.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/libraries/mibig/mibig_cds_count.csv` & `fermo_core-0.2.1/fermo_core/libraries/mibig/mibig_cds_count.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/libraries/mibig/pos/mibig_in_silico_spectral_library_3_1.mgf` & `fermo_core-0.2.1/fermo_core/libraries/mibig/pos/mibig_in_silico_spectral_library_3_1.mgf`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/fermo_core/utils/utility_method_manager.py` & `fermo_core-0.2.1/fermo_core/utils/utility_method_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/.gitignore` & `fermo_core-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/LICENSE` & `fermo_core-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/README.md` & `fermo_core-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fermo_core-0.2.0/pyproject.toml` & `fermo_core-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fermo_core"
-version = "0.2.0"
+version = "0.2.1"
 description = "Data processing/analysis functionality of metabolomics dashboard FERMO"
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 license-files = { paths = ["LICENSE"] }
 authors = [
     { name = "Mitja M. Zdouc", email = "zdoucmm@gmail.com" }
 ]
```

### Comparing `fermo_core-0.2.0/PKG-INFO` & `fermo_core-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fermo_core
-Version: 0.2.0
+Version: 0.2.1
 Summary: Data processing/analysis functionality of metabolomics dashboard FERMO
 Project-URL: Website, https://fermo.bioinformatics.nl/
 Project-URL: Repository, https://github.com/mmzdouc/fermo_core
 Project-URL: Documentation, https://mmzdouc.github.io/fermo_docs/
 Author-email: "Mitja M. Zdouc" <zdoucmm@gmail.com>
 License-File: LICENSE
 Keywords: cheminformatics,genomics,metabolomics
```

