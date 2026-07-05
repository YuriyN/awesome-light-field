# Awesome Light Field: [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)
A curated list of awesome light field resources

> Light field is a scene representation, described as a set of light rays in captured space, created by shifted full-size or micro-lenses 

## Basics
- _Gershun, The Light Field_ — first theorhetical description of a light field
- _Bolles et al., Epipolar-plane image analysis: An approach to determining structure from motion_ — first appearance and theory of epipolar-plane images, the important structure for light field analysis
- _Adelson and Bergen, The Plenoptic Function and the Elements of Early Vision_ — light field reformulation in a more convenient way
- _Levoy and Hanrahan, Light Field Rendering_ — two-plane parameterization of light field
- _Ng et al., Light Field Photography with a Hand-held Plenoptic Camera_ — description of a first plenoptic camera

## Surveys
- [Light field imaging for computer vision: a survey](https://link.springer.com/article/10.1631/FITEE.2100180) (2022)
- [Review of light field technologies](https://link.springer.com/article/10.1186/s42492-021-00096-8) (2021)
- [A survey for light field super-resolution](https://www.sciencedirect.com/science/article/pii/S2667295224000096) (2024)
- [Advances in Light Field Spatial Super-Resolution: A Comprehensive Literature Survey](https://ieeexplore.ieee.org/document/10850612/) (2025)
- [Light Field Super-Resolution: A Critical Review on Challenges and Opportunities](https://arxiv.org/abs/2510.07879) (2025)

## Datasets and benchmarks
- [HCI 4D Light Field Benchmark](https://lightfield-analysis.uni-konstanz.de/) — synthetic 9×9 light fields with ground-truth disparity, the standard depth estimation benchmark
- [Stanford Light Field Archive (Lytro 2016)](https://lightfields.stanford.edu/LF2016.html) — several hundred Lytro Illum captures in various categories
- [EPFL MMSPG Light-Field Image Dataset](https://www.epfl.ch/labs/mmspg/downloads/epfl-light-field-image-dataset/) — Lytro Illum dataset with depth maps
- [UrbanLF](https://github.com/HAWKEYE-Group/UrbanLF) — urban scene light fields for semantic segmentation (2022)
- [4DLFVD: 4D Light Field Video Dataset](https://ieee-dataport.org/open-access/4dlfvd-4d-light-field-video-dataset) — light field video captured with a camera matrix
- [Sintel 4D Light Field Videos](https://ieee-dataport.org/open-access/sintel-4d-light-field-video-dataset) — synthetic light field videos with ground-truth depth
- [DDFF-12](https://github.com/hazirbas/ddff-toolbox) — light field dataset and toolbox for depth from focus (2017)

## Algorithms with available code

### Depth Estimation
| Title | Year | Framework | Link |
|-------|------|-----------|------|
|3D Convolutional Neural Network for Light Field Depth Estimation|||https://github.com/catdance124/3Dconv_LF_depth_estimation|
|Deep Coarse-to-fine Dense Light Field Reconstruction with Flexible Sampling and Geometry-aware Fusion|||https://github.com/jingjin25/LFASR-FS-GAF|
|Depth Estimation from 4D Light Field Videos|||https://github.com/mediaeng-lfv/LFV_Disparity_Estimation|
|Depth from Combining Defocus and Correspondence Using Light-Field Cameras|||https://github.com/Vincentqyw/depth-from-defocus-and-correspondence|
|Depthy|||https://github.com/hahnec/depthy|
|DistgDisp: Disentangling Mechanism for Light Field Disparity Estimation|||https://github.com/YingqianWang/DistgDisp|
|EPINET: A Fully-Convolutional Neural Network using Epipolar Geometry for Depth from Light Field Images|||https://github.com/chshin10/epinet|
|Efficient Light Field Reconstruction via Spatio-Angular Dense Network|||https://github.com/huzexi/SADenseNet|
|Empirical Bayesian Light-Field Stereo Matching by Robust Pseudo Random Field Modeling|||https://www.ee.nthu.edu.tw/chaotsung/rprf/index.html|
|Fast Light-field Disparity Estimation with Multi-disparity-scale Cost Aggregation|||https://github.com/zcong17huang/FastLFnet|
|High-Dimensional Dense Residual Convolutional Neural Network for Light Field Reconstruction|||https://github.com/monaen/LightFieldReconstruction|
|Intrinsic Light Field Decomposition and Disparity Estimation with a Deep Encoder-Decoder Network|||https://github.com/cvia-kn/lf_autoencoder_cvpr2018_code|
|Learning Sheared EPI Structure for Light Field Reconstruction|||https://github.com/GaochangWu/Sheared-EPI|
|Learning to Think Outside the Box: Wide-Baseline Light Field Depth Estimation with EPI-Shift|||https://github.com/titus-leistner/epi-shift|
|LFattNet: Attention-based View Selection Networks for Light-field Disparity Estimation|||https://github.com/LIAGM/LFattNet|
|MANet: Multi-scale Aggregated Network For Light Field Depth Estimation|||https://github.com/YanWQ/MANet|
|OccCasNet: Occlusion-aware Cascade Cost Volume for Light Field Depth Estimation|2023|TensorFlow|https://github.com/chaowentao/OccCasNet|
|Occlusion-Aware Cost Constructor for Light Field Depth Estimation|||https://github.com/YingqianWang/OACC-Net|
|On Linear Structure from Motion for Light Field Cameras|||https://publications.lightfield-analysis.net/|
|OPAL: Occlusion Pattern Aware Loss for Unsupervised Light Field Disparity Estimation|2023|PyTorch|https://github.com/pengHTYX/OPAL|
|Robust Depth Estimation for Light Field via Spinning Parallelogram Operator|||https://github.com/shuozh/Spinning-Parallelogram-Operator|
|SubFocal: Learning Sub-Pixel Disparity Distribution for Light Field Depth Estimation|2023|TensorFlow|https://github.com/chaowentao/SubFocal|
|Unsupervised disparity estimation from light field using plug-and-play weighted warping loss|||https://www.fujii.nuee.nagoya-u.ac.jp/Research/LFDepth/|
|Variational light field analysis for disparity estimation and super-resolution|||https://github.com/GilbertRC/Light-Field-Structure-Tensor-Depth-Estimation|

### Denoising
| Title | Year | Framework | Link |
|-------|------|-----------|------|
|Light Field Denoising by Sparse 5D Transform Domain Collaborative Filtering|||https://github.com/V-Sense/LFBM5D|
|Pipeline for Noise Generation and Denoising of Light Fields (wavelet, BM3D, LFBM5D, DnCNN, LFDnPatch)|2023|C++|https://github.com/mmspg/Light-Field-Denoising|
|Robust Dense Light Field Reconstruction from Sparse Noisy Sampling|2021||https://github.com/sunshineHDU/NoisyLFRecon|

### Novel view synthesis
| Title | Year | Framework | Link |
|-------|------|-----------|------|
|DistgASR: Disentangling Mechanism for Light Field Angular Super-Resolution|2022|PyTorch|https://github.com/YingqianWang/DistgASR|
|Learning to Synthesize a 4D RGBD Light Field from a Single Image|||https://github.com/pratulsrinivasan/Local_Light_Field_Synthesis|
|Local Light Field Fusion|||https://github.com/Fyusion/LLFF|
|Multi-Angular Epipolar Geometry Based Light Field Angular Reconstruction Network|||https://github.com/ldyorchid/Multi_Angular_Epipolar_Geometry_Based_Light_Field_Angular_Reconstruction_Network|
|Real-Time Light Field Video Focusing and GPU Accelerated Streaming|||https://github.com/dormon/3DApps/blob/master/src/lightfieldPlayer.cpp|
|Lightweight All-Focused Light Field Rendering|||https://www.fit.vutbr.cz/~ichlubna/lf|
|Efficient Random-Access GPU Video Decoding for Light-Field Rendering|||https://github.com/ichlubna/lfEncoding|

### Super-resolution
| Title | Year | Framework | Link |
|-------|------|-----------|------|
|DistgSSR: Disentangling Mechanism for Light Field Statial Super-Resolution|||https://github.com/YingqianWang/DistgSSR|
|DistgEPIT: Enhanced Disparity Learning for Light Field Image Super-Resolution (NTIRE 2023 solution)|2023|PyTorch|https://github.com/OpenMeow/NTIRE23_LFSR_DistgEPIT|
|DPT: Detail-Preserving Transformer for Light Field Image Super-Resolution|2022|PyTorch|https://github.com/BITszwang/DPT|
|EPIT: Learning Non-Local Spatial-Angular Correlation for Light Field Image Super-Resolution|2023|PyTorch|https://github.com/ZhengyuLiang24/EPIT|
|Graph-Based Light Field Super-Resolution|||https://github.com/rossimattia/light-field-super-resolution|
|LF-DET: Exploiting Spatial and Angular Correlations With Deep Efficient Transformers for Light Field Image Super-Resolution|2023|PyTorch|https://github.com/Congrx/LF-DET|
|LF-DGT: Multi-level Disparity-Guided Transformers for Light Field Spatial Super-Resolution|2025|PyTorch|https://github.com/YigengLiao/LF-DGT|
|LF-DMnet: Real-World Light Field Image Super-Resolution via Degradation Modulation|2024|PyTorch|https://github.com/YingqianWang/LF-DMnet|
|LFMamba: Light Field Image Super-Resolution with State Space Model|2024|PyTorch|https://github.com/stanley-313/LFMamba|
|LFMT: Exploring Non-Local Spatial-Angular Correlations with a Hybrid Mamba-Transformer Framework for Light Field Super-Resolution|2025|PyTorch|https://github.com/hsliu01/LFMT|
|LFSRDiff: Light Field Image Super-Resolution via Diffusion Models|2023|PyTorch|https://github.com/chaowentao/LFSRDiff|
|LFT: Light Field Image Super-Resolution with Transformers|2022|PyTorch|https://github.com/ZhengyuLiang24/LFT|
|LFTransMamba: NTIRE 2025 Light Field Super-Resolution Challenge Solution|2025|PyTorch|https://github.com/OpenMeow/LFTransMamba|
|Light Field Spatial Super-resolution via Deep Combinatorial Geometry Embedding and Structural Consistency Regularization|||https://github.com/jingjin25/LFSSR-ATO|
|Light Field Super-Resolution By Jointly Exploiting Internal and External Similarities|||https://github.com/Joechann0831/LFSR-FusNet|
|Residual Networks for Light Field Image Super-Resolution|||https://github.com/wxywhu/demo-resLF|
|Spatial-Angular Interaction for Light Field Image Super-Resolution|||https://github.com/YingqianWang/LF-InterNet|
|Light Field Spatial Super-resolution Using Deep Efficient Spatial-Angular Separable Convolution|||https://github.com/jingjin25/LFSSR-SAS-PyTorch|

### Other tasks
| Title | Year | Framework | Link |
|-------|------|-----------|------|
|DRBNet: Learning to Deblur using Light Field Generated and Real Defocus Images|2022|PyTorch|https://github.com/lingyanruan/DRBNet|
|Light Field Blind Motion Deblurring|2017|TensorFlow|https://github.com/pratulsrinivasan/Light_Field_Blind_Motion_Deblurring|
|Light Field Salient Object Detection: A Review and Benchmark|2021||https://github.com/kerenfu/LFSOD-Survey|
|OAFuser: Towards Omni-Aperture Fusion for Light Field Semantic Segmentation|2023|PyTorch|https://github.com/FeiBryantkit/OAFuser|
|Style Transfer for Light Field Photography|2020||https://github.com/davidmhart/LightFieldStyleTransfer|
|VCD-Net: Real-time volumetric reconstruction of biological dynamics with light-field microscopy|2021|TensorFlow|https://github.com/feilab-hust/VCD-Net|

### Light field and neural rendering
| Title | Year | Framework | Link |
|-------|------|-----------|------|
|Light Field Networks: Neural Scene Representations with Single-Evaluation Rendering|2021|PyTorch|https://github.com/vsitzmann/light-field-networks|
|Light Field Neural Rendering|2022|JAX|https://github.com/google-research/google-research/tree/master/light_field_neural_rendering|
|MobileR2L: Real-Time Neural Light Fields on Mobile Devices|2023|PyTorch|https://github.com/snap-research/MobileR2L|
|NeuLF: Efficient Novel View Synthesis with Neural 4D Light Field|2022|PyTorch|https://github.com/oppo-us-research/NeuLF|
|R2L: Distilling Neural Radiance Field to Neural Light Field for Efficient Novel View Synthesis|2022|PyTorch|https://github.com/snap-research/R2L|

### Other 
- [BasicLFSR: PyTorch benchmark toolbox for light field super-resolution](https://github.com/ZhengyuLiang24/BasicLFSR)
- [CocoLib](https://sourceforge.net/projects/cocolib/)
- [LiFF: Light field features in scale and depth](https://dgd.vision/Tools/LiFF/)
- [Light Field Toolbox for MATLAB](https://github.com/doda42/LFToolbox)
- [LFIT: Light-Field Imaging Toolkit](https://github.com/ElsevierSoftwareX/SOFTX-D-15-00046)
- [Modified Baseline for Light Field Stitching](https://github.com/GilbertRC/Modified-Baseline-for-Light-Field-Stitching)
- [plenpy: Python library for light field and hyperspectral processing](https://iiit-public.gitlab.io/plenpy/user-doc.html)
- [PlenoptiCam](https://github.com/hahnec/plenopticam)
- [Plenoptic Toolbox 2.0](https://github.com/freerafiki/PlenopticToolbox2.0)

## Compression and coding
- [JPEG Pleno Light Field](https://jpeg.org/jpegpleno/lightfield.html) — ISO/IEC 21794 light field coding standard
- [MPEG Immersive Video (MIV)](https://mpeg-miv.org/) — multiview and light field compression standard for immersive video
- [SADN: Spatial-Angular Decorrelated Network for learned light field compression](https://github.com/VincentChandelier/SADN) (2022)

## Hardware, cameras and displays
- [Raytrix](https://raytrix.de/home-2/) — industrial 3D light field cameras
- [Lytro Archive](http://lightfield-forum.com/lytro/lytro-archive/) — software, firmware and resources for discontinued Lytro cameras
- [K|Lens One](https://petapixel.com/2021/11/22/klens-unveils-worlds-first-light-field-lens-that-works-on-any-camera/) — light field lens for standard cameras
- [Looking Glass Factory](https://lookingglassfactory.com/) — glasses-free light field displays
- [Leia / Immersity AI](https://immersity.ai/) — light field displays and 2D-to-3D conversion

## Demos
- [Light Field Renderer](https://github.com/linusmossberg/light-field-renderer)
- [Light Field image viewer](https://github.com/tatsy/LightField)
- [WebGL2 Light field renderer](https://github.com/hypothete/lightfield-webgl2)

## Workshops and challenges
- [NTIRE 2023 Light Field Image Super-Resolution Challenge](https://arxiv.org/abs/2304.10415) — first NTIRE light field challenge, report (CVPR 2023 workshop)
- [NTIRE 2024 Light Field Image Super-Resolution Challenge](https://codalab.lisn.upsaclay.fr/competitions/17265) — challenge page
- [NTIRE 2025 Light Field Image Super-Resolution Challenge](https://openaccess.thecvf.com/content/CVPR2025W/NTIRE/papers/Wang_NTIRE_2025_Challenge_on_Light_Field_Image_Super-Resolution_Methods_and_CVPRW_2025_paper.pdf) — challenge report
- [LFNAT @ CVPR 2023](https://openaccess.thecvf.com/CVPR2023_workshops/LFNAT) — workshop on light fields for computer vision

## Research groups
- [Yingqian Wang (NUDT)](https://yingqianwang.github.io/) — light field super-resolution and disparity estimation, NTIRE LF challenge organizer
- [Fujii Lab, Nagoya University](https://www.fujii.nuee.nagoya-u.ac.jp/publications-e.html) — light field acquisition, coded aperture, neural representations
- [V-SENSE, Trinity College Dublin](https://v-sense.scss.tcd.ie/) — light field imaging for AR/VR and creative technologies
- [KAIST Visual Computing Lab](https://vclab.kaist.ac.kr/) — light field displays and radiance field rendering

## Other resources
- [LightField Forum - Light Field and Computational Imaging News](http://lightfield-forum.com/en/)
- [LF-Image-SR](https://github.com/YingqianWang/LF-Image-SR) — paper list on light field image super-resolution
- [awesome-light-fields](https://github.com/JoanCharmant/awesome-light-fields) — curated light field resources on capture, rendering and processing
- [awesome-light-field-processing](https://github.com/bchao1/awesome-light-field-processing) — light field synthesis and reconstruction papers
- [lightfield-analysis resources](https://github.com/lightfield-analysis/resources) — datasets and tools accompanying the HCI benchmark
