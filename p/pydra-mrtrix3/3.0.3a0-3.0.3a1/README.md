# Comparing `tmp/pydra_mrtrix3-3.0.3a0.tar.gz` & `tmp/pydra_mrtrix3-3.0.3a1.tar.gz`

## Comparing `pydra_mrtrix3-3.0.3a0.tar` & `pydra_mrtrix3-3.0.3a1.tar`

### file list

```diff
@@ -1,336 +1,46 @@
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/.gitattributes
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/CHANGELOG.md
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/codecov.yml
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/conftest.py
--rwxr-xr-x   0        0        0    11414 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/generate.py
--rw-r--r--   0        0        0     8828 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/.github/workflows/ci-cd.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/docs/Makefile
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/docs/index.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/docs/make.bat
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/docs/requirements.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/.codespell-ignorewords
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/.flake8
--rw-r--r--   0        0        0    14223 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/LICENSE
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/README.rst
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/conftest.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/pyproject.toml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/pytest.ini
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/__init__.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/dwi.py
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/image.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/in_out.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/track.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/.codespell-ignorewords
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/.flake8
--rw-r--r--   0        0        0    14223 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/LICENSE
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/README.rst
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/conftest.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/pyproject.toml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/pytest.ini
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/__init__.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/converters.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/gradients.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/image.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/tracks.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/tests/test_converters.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/_version.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/latest.py
--rw-r--r--   0        0        0    10680 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/manual/mrcalc_.py
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/__init__.py
--rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/afdconnectivity_.py
--rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/amp2response_.py
--rw-r--r--   0        0        0     8477 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/amp2sh_.py
--rw-r--r--   0        0        0    10754 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/connectome2tck_.py
--rw-r--r--   0        0        0     4641 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/connectomeedit_.py
--rw-r--r--   0        0        0    12733 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/connectomestats_.py
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dcmedit_.py
--rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dcminfo_.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dirflip_.py
--rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dirgen_.py
--rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dirmerge_.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dirorder_.py
--rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dirsplit_.py
--rw-r--r--   0        0        0     8257 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dirstat_.py
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2adc_.py
--rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2fod_.py
--rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2mask_3dautomask_.py
--rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2mask_ants_.py
--rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2mask_b02template_.py
--rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2mask_consensus_.py
--rw-r--r--   0        0        0     6329 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2mask_fslbet_.py
--rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2mask_hdbet_.py
--rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2mask_legacy_.py
--rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2mask_mean_.py
--rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2mask_mtnorm_.py
--rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2mask_synthstrip_.py
--rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2mask_trace_.py
--rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2response_dhollander_.py
--rw-r--r--   0        0        0     7147 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2response_fa_.py
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2response_manual_.py
--rw-r--r--   0        0        0     8602 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2response_msmt_5tt_.py
--rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2response_tax_.py
--rw-r--r--   0        0        0     7390 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2response_tournier_.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwi2tensor_.py
--rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwibiascorrect_ants_.py
--rw-r--r--   0        0        0     6333 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwibiascorrect_fsl_.py
--rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwibiascorrect_mtnorm_.py
--rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwibiasnormmask_.py
--rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwicat_.py
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwidenoise_.py
--rw-r--r--   0        0        0     9935 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwiextract_.py
--rw-r--r--   0        0        0    14217 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwifslpreproc_.py
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwigradcheck_.py
--rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwinormalise_group_.py
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwinormalise_manual_.py
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwinormalise_mtnorm_.py
--rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/dwishellmath_.py
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fivett2gmwmi_.py
--rw-r--r--   0        0        0     5339 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fivett2vis_.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fivettcheck_.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fivettedit_.py
--rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fivettgen_freesurfer_.py
--rw-r--r--   0        0        0     7014 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fivettgen_fsl_.py
--rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fivettgen_gif_.py
--rw-r--r--   0        0        0     7976 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fivettgen_hsvs_.py
--rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fixel2peaks_.py
--rw-r--r--   0        0        0     5133 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fixel2sh_.py
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fixel2tsf_.py
--rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fixel2voxel_.py
--rw-r--r--   0        0        0    13896 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fixelcfestats_.py
--rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fixelconnectivity_.py
--rw-r--r--   0        0        0     7393 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fixelconvert_.py
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fixelcorrespondence_.py
--rw-r--r--   0        0        0     5149 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fixelcrop_.py
--rw-r--r--   0        0        0     6610 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fixelfilter_.py
--rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fixelreorient_.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fod2dec_.py
--rw-r--r--   0        0        0     8988 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/fod2fixel_.py
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/label2colour_.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/label2mesh_.py
--rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/labelconvert_.py
--rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/labelsgmfix_.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/labelstats_.py
--rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mask2glass_.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/maskdump_.py
--rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/maskfilter_.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mesh2voxel_.py
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/meshconvert_.py
--rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/meshfilter_.py
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mraverageheader_.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrcat_.py
--rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrcentroid_.py
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrcheckerboardmask_.py
--rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrclusterstats_.py
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrcolour_.py
--rw-r--r--   0        0        0    20223 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrconvert_.py
--rw-r--r--   0        0        0     8907 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrdegibbs_.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrdump_.py
--rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mredit_.py
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrfilter_.py
--rw-r--r--   0        0        0    14556 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrgrid_.py
--rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrhistmatch_.py
--rw-r--r--   0        0        0     5376 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrhistogram_.py
--rw-r--r--   0        0        0    13641 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrinfo_.py
--rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrmath_.py
--rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrmetric_.py
--rw-r--r--   0        0        0    31417 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrregister_.py
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrstats_.py
--rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrthreshold_.py
--rw-r--r--   0        0        0    17481 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrtransform_.py
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mrtrix_cleanup_.py
--rw-r--r--   0        0        0     9345 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/mtnormalise_.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/peaks2amp_.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/peaks2fixel_.py
--rw-r--r--   0        0        0    18035 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/population_template_.py
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/responsemean_.py
--rw-r--r--   0        0        0     9663 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/sh2amp_.py
--rw-r--r--   0        0        0     6651 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/sh2peaks_.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/sh2power_.py
--rw-r--r--   0        0        0     5839 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/sh2response_.py
--rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/shbasis_.py
--rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/shconv_.py
--rw-r--r--   0        0        0    12727 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tck2connectome_.py
--rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tck2fixel_.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tckconvert_.py
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tckdfc_.py
--rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tckedit_.py
--rw-r--r--   0        0        0    24169 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tckgen_.py
--rw-r--r--   0        0        0    11878 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tckglobal_.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tckinfo_.py
--rw-r--r--   0        0        0    15121 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tckmap_.py
--rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tckresample_.py
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tcksample_.py
--rw-r--r--   0        0        0    13218 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tcksift2_.py
--rw-r--r--   0        0        0    10258 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tcksift_.py
--rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tckstats_.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tcktransform_.py
--rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tensor2metric_.py
--rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/transformcalc_.py
--rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/transformcompose_.py
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/transformconvert_.py
--rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tsfdivide_.py
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tsfinfo_.py
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tsfmult_.py
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tsfsmooth_.py
--rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tsfthreshold_.py
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tsfvalidate_.py
--rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/vectorstats_.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/voxel2fixel_.py
--rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/voxel2mesh_.py
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/warp2metric_.py
--rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/warpconvert_.py
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/warpcorrect_.py
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/warpinit_.py
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/warpinvert_.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_afdconnectivity.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_amp2response.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_amp2sh.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_connectome2tck.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_connectomeedit.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_connectomestats.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dcmedit.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dcminfo.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dirflip.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dirgen.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dirmerge.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dirorder.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dirsplit.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dirstat.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2adc.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2fod.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_3dautomask.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_ants.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_b02template.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_consensus.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_fslbet.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_hdbet.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_legacy.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_mean.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_mtnorm.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_synthstrip.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2mask_trace.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2response_dhollander.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2response_fa.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2response_manual.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2response_msmt_5tt.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2response_tax.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2response_tournier.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwi2tensor.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwibiascorrect_ants.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwibiascorrect_fsl.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwibiascorrect_mtnorm.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwibiasnormmask.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwicat.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwidenoise.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwiextract.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwifslpreproc.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwigradcheck.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwinormalise_group.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwinormalise_manual.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwinormalise_mtnorm.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_dwishellmath.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fivett2gmwmi.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fivett2vis.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fivettcheck.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fivettedit.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fivettgen_freesurfer.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fivettgen_fsl.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fivettgen_gif.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fivettgen_hsvs.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fixel2peaks.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fixel2sh.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fixel2tsf.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fixel2voxel.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fixelcfestats.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fixelconnectivity.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fixelconvert.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fixelcorrespondence.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fixelcrop.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fixelfilter.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fixelreorient.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fod2dec.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_fod2fixel.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_label2colour.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_label2mesh.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_labelconvert.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_labelsgmfix.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_labelstats.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mask2glass.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_maskdump.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_maskfilter.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mesh2voxel.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_meshconvert.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_meshfilter.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mraverageheader.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrcat.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrcentroid.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrcheckerboardmask.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrclusterstats.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrcolour.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrconvert.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrdegibbs.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrdump.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mredit.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrfilter.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrgrid.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrhistmatch.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrhistogram.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrinfo.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrmath.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrmetric.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrregister.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrstats.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrthreshold.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrtransform.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mrtrix_cleanup.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_mtnormalise.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_peaks2amp.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_peaks2fixel.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_population_template.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_responsemean.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_sh2amp.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_sh2peaks.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_sh2power.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_sh2response.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_shbasis.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_shconv.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tck2connectome.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tck2fixel.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tckconvert.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tckdfc.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tckedit.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tckgen.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tckglobal.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tckinfo.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tckmap.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tckresample.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tcksample.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tcksift.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tcksift2.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tckstats.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tcktransform.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tensor2metric.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_transformcalc.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_transformcompose.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_transformconvert.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tsfdivide.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tsfinfo.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tsfmult.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tsfsmooth.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tsfthreshold.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_tsfvalidate.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_vectorstats.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_voxel2fixel.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_voxel2mesh.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_warp2metric.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_warpconvert.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_warpcorrect.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_warpinit.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/v3_0/tests/test_warpinvert.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/.gitignore
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/LICENSE
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/README.rst
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/pyproject.toml
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a0/PKG-INFO
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/.gitattributes
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/CHANGELOG.md
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/codecov.yml
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/conftest.py
+-rwxr-xr-x   0        0        0    11414 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/generate.py
+-rw-r--r--   0        0        0     8828 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/.github/workflows/ci-cd.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/docs/Makefile
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/docs/index.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/docs/make.bat
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/docs/requirements.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/.codespell-ignorewords
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/.flake8
+-rw-r--r--   0        0        0    14223 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/LICENSE
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/README.rst
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/conftest.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/pyproject.toml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/pytest.ini
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/__init__.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/dwi.py
+-rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/image.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/in_out.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/track.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/tests/test_mime.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/.codespell-ignorewords
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/.flake8
+-rw-r--r--   0        0        0    14223 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/LICENSE
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/README.rst
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/conftest.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/pyproject.toml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/pytest.ini
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/__init__.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/converters.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/gradients.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/image.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/tracks.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/tests/test_converters.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/pydra/tasks/mrtrix3/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/pydra/tasks/mrtrix3/_version.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/pydra/tasks/mrtrix3/latest.py
+-rw-r--r--   0        0        0    10680 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/pydra/tasks/mrtrix3/manual/mrcalc_.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/.gitignore
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/LICENSE
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/README.rst
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/pyproject.toml
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 pydra_mrtrix3-3.0.3a1/PKG-INFO
```

### Comparing `pydra_mrtrix3-3.0.3a0/CHANGELOG.md` & `pydra_mrtrix3-3.0.3a1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/conftest.py` & `pydra_mrtrix3-3.0.3a1/conftest.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/generate.py` & `pydra_mrtrix3-3.0.3a1/generate.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/.github/workflows/ci-cd.yml` & `pydra_mrtrix3-3.0.3a1/.github/workflows/ci-cd.yml`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/docs/Makefile` & `pydra_mrtrix3-3.0.3a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/docs/make.bat` & `pydra_mrtrix3-3.0.3a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/LICENSE` & `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/README.rst` & `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/README.rst`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/conftest.py` & `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/conftest.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/pyproject.toml` & `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/dwi.py` & `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/dwi.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/image.py` & `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     @property
     def data_file(self):
         return self
 
 
 class ImageFormatGz(Gzip[ImageFormat]):
 
-    iana_mime = None
+    iana_mime = "application/x-image-format-gz"
     ext = ".mif.gz"
 
 
 class ImageHeader(BaseMrtrixImage):
 
     ext = ".mih"
```

### Comparing `pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/in_out.py` & `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3/fileformats/medimage_mrtrix3/in_out.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/LICENSE` & `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/LICENSE`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/README.rst` & `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/README.rst`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/conftest.py` & `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/conftest.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/pyproject.toml` & `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/converters.py` & `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/converters.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 from fileformats.medimage_mrtrix3 import (
     ImageFormat as MrtrixImage,
     ImageHeader as MrtrixImageHeader,
 )
 
 try:
-    from pydra.tasks.mrtrix3.utils import MRConvert
+    from pydra.tasks.mrtrix3.utils import MrConvert
 except ImportError:
-    from pydra.tasks.mrtrix3.latest import mrconvert as MRConvert
+    from pydra.tasks.mrtrix3.latest import mrconvert as MrConvert
 
     in_out_file_kwargs = {"in_file": "input", "out_file": "output"}
 else:
     in_out_file_kwargs = {}
 
 
 @hook.converter(
@@ -33,15 +33,15 @@
         extension of the output file, used by MRConvert to determine the desired format
 
     Returns
     -------
     pydra.ShellCommandTask
         the converter task
     """
-    return MRConvert(name=name, out_file="out" + out_ext, **kwargs)
+    return MrConvert(name=name, out_file="out" + out_ext, **kwargs)
 
 
 @hook.converter(
     source_format=MedicalImage,
     target_format=MrtrixImageHeader,
     out_ext=MrtrixImageHeader.ext,
     **in_out_file_kwargs,
@@ -57,8 +57,8 @@
         extension of the output file, used by MRConvert to determine the desired format
 
     Returns
     -------
     pydra.ShellCommandTask
         the converter task
     """
-    return MRConvert(name=name, out_file="out" + out_ext, **kwargs)
+    return MrConvert(name=name, out_file="out" + out_ext, **kwargs)
```

### Comparing `pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/image.py` & `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/image.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 import os
 from unittest import mock
 import typing as ty
 from pathlib import Path
 import numpy as np
-from random import Random
 from medimages4tests.dummy.nifti import get_image as get_dummy_nifti
-from fileformats.core import FileSet
+from fileformats.core import FileSet, SampleFileGenerator
 from fileformats.medimage import MedicalImage, Nifti1
 from fileformats.medimage_mrtrix3 import ImageFormat
 
 
 @FileSet.generate_sample_data.register
 def generate_mrtrix_sample_data(
     mif: ImageFormat,
-    dest_dir: Path,
-    seed: ty.Union[int, Random] = 0,
-    stem: ty.Optional[str] = None,
+    generator: SampleFileGenerator,
 ) -> ty.Iterable[Path]:
-    nifti = Nifti1(get_dummy_nifti(dest_dir / "nifti.nii"))
+    nifti = Nifti1(get_dummy_nifti(generator.dest_dir / "nifti.nii"))
     with mock.patch.dict(os.environ, {"MRTRIX_CLI_PARSE_ONLY": "0"}):
         mif = ImageFormat.convert(nifti)
     return mif.fspaths
 
 
 @MedicalImage.read_array.register
 def mrtrix_read_array(mif: ImageFormat) -> np.ndarray:
```

### Comparing `pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/tracks.py` & `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/tracks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import time
 import struct
 import math
 from pathlib import Path
 import typing as ty
-from random import Random
-from fileformats.core import FileSet
+from fileformats.core import FileSet, SampleFileGenerator
 from fileformats.medimage_mrtrix3 import Tracks
 
 
 @FileSet.generate_sample_data.register
 def generate_tracks_sample_data(
     tracks: Tracks,
-    dest_dir: Path,
-    seed: ty.Union[int, Random] = 0,
-    stem: ty.Optional[str] = None,
+    generator: SampleFileGenerator,
 ) -> ty.Iterable[Path]:
     """Generate a tracks file with a single straight track of length 10"""
-    fspath = dest_dir / "tracks.tck"
+    fspath = generator.dest_dir / "tracks.tck"
     timestamp = str(time.time() * 1e9 + time.process_time_ns())
     contents = f"""mrtrix tracks
 datatype: Float32BE
 timestamp: {timestamp}
 count: 1
 total_count: 1
 file: . """
```

### Comparing `pydra_mrtrix3-3.0.3a0/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/tests/test_converters.py` & `pydra_mrtrix3-3.0.3a1/fileformats-medimage-mrtrix3-extras/fileformats/extras/medimage_mrtrix3/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/pydra/tasks/mrtrix3/manual/mrcalc_.py` & `pydra_mrtrix3-3.0.3a1/pydra/tasks/mrtrix3/manual/mrcalc_.py`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/.gitignore` & `pydra_mrtrix3-3.0.3a1/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -133,8 +133,8 @@
 
 # VS Code
 .vscode/
 
 # Hatchling
 _version.py
 
-#/pydra/tasks/mrtrix3/v3_0
+/pydra/tasks/mrtrix3/v3_0
```

### Comparing `pydra_mrtrix3-3.0.3a0/LICENSE` & `pydra_mrtrix3-3.0.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/README.rst` & `pydra_mrtrix3-3.0.3a1/README.rst`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/pyproject.toml` & `pydra_mrtrix3-3.0.3a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydra_mrtrix3-3.0.3a0/PKG-INFO` & `pydra_mrtrix3-3.0.3a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydra-mrtrix3
-Version: 3.0.3a0
+Version: 3.0.3a1
 Summary: pydra-mrtrix3 contains Pydra task specifications for MRtrix3 tools
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License:    Copyright 2022 Nipype developers
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
```

