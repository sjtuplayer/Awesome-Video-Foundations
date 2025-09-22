# Video Generation Foundation Model: A Survey

[![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)
[![Website](https://img.shields.io/badge/Project-Page-green?style=flat-square&logo=gitbook)](https://github.com/worldbench/survey)

---

## 📖 Overview

The rapid advancement of **Artificial Intelligence Generated Content (AIGC)** has revolutionized video generation, enabling systems like **OpenAI's Sora**, **Google's Veo3**, and **Pika Labs' tools** to synthesize temporally coherent and semantically rich videos. These advancements pave the way for building **"world models"** 🌍 that simulate real-world dynamics, with applications spanning entertainment, education, and virtual reality.

This survey provides a **systematic review** of the development of video generation technology, tracing its evolution through **three major paradigms**:

> 🎭 **GAN Era (2014-2020)** → 🌊 **Diffusion Dominance (2021-2025+)** → 🔄 **Autoregressive Future (2024-2025+)**

We conduct an **in-depth analysis** of the foundational principles, key advancements, and comparative strengths/limitations of each methodology, with special attention to **🎬 multimodal video generation** that integrates text, audio, and visual modalities for comprehensive content creation.

### 🎯 Key Contributions

**1️⃣ Comprehensive Coverage**: **Systematic review** of **three dominant paradigms** - 🎭 **GAN-based**, 🌊 **Diffusion-based**, and 🔄 **Autoregressive (AR)-based** methods
   - 📊 **50+ GAN models** spanning spatio-temporal joint modeling to StyleGAN-based generation
   - 🌊 **80+ Diffusion models** from UNet architectures to advanced Transformer-based approaches  
   - 🔄 **50+ AR models** covering pixel-level to latent space autoregressive generation

**2️⃣ Historical Perspective**: **Traces the complete evolution** from early GANs (2014) to current state-of-the-art models (2025)
   - 📈 **Decade-spanning analysis** of technological breakthroughs and paradigm shifts
   - 🔍 **Comparative assessment** of each era's strengths, limitations, and impact on the field

**3️⃣ Future Insights**: **Provides strategic guidance** for future research in video generation and **🌍 world modeling**
   - 🚀 **Emerging opportunities** in real-time generation and interactive content creation
   - ⚖️ **Safety and ethics** considerations for responsible AI development
   - 🔮 **Next-generation architectures** and scaling laws for video foundation models

---

## 🏗️ Architecture Overview

### 📅 **Leading Video Foundation Models Timeline (Dec 2024 - Present)**

<div align="center">
  <img src="assets/imgs/timeline.png" alt="Video Generation Timeline" width="100%">
</div>

> **🚀 Recent Breakthroughs**: This timeline showcases the rapid evolution of video foundation models from December 2024 to the present, highlighting key milestones in:
> - 🎬 **Commercial Deployments**: Sora, Veo3, Runway Gen-3
> - 🔬 **Research Advances**: CogVideoX, HunyuanVideo, Wan
> - 📊 **Performance Leaps**: Resolution scaling, temporal consistency, generation speed
> - 🌐 **Multimodal Integration**: Text-to-video, image-to-video, audio-visual synthesis

### 📊 **Benchmark Evaluation Results for Leading Methods**

<div align="center">
  <img src="assets/imgs/benchmarks.png" alt="Video Generation Benchmarks" width="100%">
</div>

> **📈 Comprehensive Assessment**: This evaluation matrix compares state-of-the-art video generation models across three key dimensions:
> - 🏗️ **Foundation**: Comprehensive video generation evaluation including visual quality, temporal consistency, text alignment, and generation efficiency
> - ⚖️ **Physics**: Physics-constrained evaluation covering motion realism, object dynamics, physical plausibility, and natural scene interactions
> - 🛡️ **Safety**: Generation safety evaluation including content appropriateness, bias detection, harmful content protection, and ethical compliance
>
> **Key Insights**: Diffusion models currently lead in quality, while autoregressive approaches show promise for scalability and controllability.

---


## 📚 Table of Contents

- [GAN-based Models](#-gan-based-models)
  - [Spatio-Temporal Joint GANs](#spatio-temporal-joint-gans)
  - [Temporal GANs](#temporal-gans)
  - [Progressive GANs](#progressive-gans)
  - [StyleGAN-based Generation](#stylegan-based-generation)
- [Diffusion-based Models](#-diffusion-based-models)
  - [UNet with Temporal Modules](#1-unet-with-temporal-modules)
  - [Diffusion Transformers](#2-diffusion-transformers)
  - [Efficient Video Diffusion Models](#3-efficient-video-diffusion-models)
- [Autoregressive Models](#-autoregressive-models)
  - [Pixel-level AR Models](#pixel-level-ar-models)
  - [Latent Space AR Models](#latent-space-ar-models)
  - [Multimodal AR Models](#multimodal-ar-models)
- [Benchmarks & Evaluation](#-benchmarks--evaluation)
- [Applications & Downstream Tasks](#-applications--downstream-tasks)
- [Research Trends & Future Directions](#-research-trends--future-directions)

---

## 🎭 GAN-based Models

> Generative Adversarial Networks (GANs) laid the groundwork for video synthesis, with innovations in spatio-temporal joint modeling, temporal decomposition, and progressive generation strategies.

### Spatio-Temporal Joint GANs
> Models that process both spatial and temporal dimensions simultaneously using unified architectures.

|     Model     | Paper                                                        |   Venue    |                           Website                            |                            GitHub                            |
| :-----------: | :----------------------------------------------------------- | :--------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|   `3D-Conv`   | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>Learning Spatiotemporal Features with 3D Convolutional Networks | Coming Soon |                              -                               |                              -                               |
|     `VGAN`    | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>Generating Videos with Scene Dynamics | Coming Soon |                              -                               |                              -                               |
|   `DVD-GAN`   | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>Adversarial Video Generation on Complex Datasets | Coming Soon |                              -                               |                              -                               |

### Temporal GANs
> Models that decompose video generation into motion and content components for more efficient training.

|     Model     | Paper                                                        |   Venue    |                           Website                            |                            GitHub                            |
| :-----------: | :----------------------------------------------------------- | :--------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|    `MCnet`    | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>Decomposing Motion and Content for Natural Video Sequence Prediction | Coming Soon |                              -                               |                              -                               |
|   `MoCoGAN`   | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>MoCoGAN: Decomposing Motion and Content for Video Generation | Coming Soon |                              -                               |                              -                               |
| `MoCoGAN-HD`  | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>MoCoGAN-HD: A Good Image Generator Is What You Need for High-Resolution Video Synthesis | Coming Soon |                              -                               |                              -                               |
|   `TS-GAN`    | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>Temporal Shift GAN for Large Scale Video Generation | Coming Soon |                              -                               |                              -                               |

### Progressive GANs
> Models that generate content progressively, starting from low resolution and gradually increasing detail.

|     Model     | Paper                                                        |   Venue    |                           Website                            |                            GitHub                            |
| :-----------: | :----------------------------------------------------------- | :--------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| `Progressive` | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>Progressive Growing of GANs for Improved Quality, Stability, and Variation | Coming Soon |                              -                               |                              -                               |
|    `SWGAN`    | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>Sliced Wasserstein Generative Models | Coming Soon |                              -                               |                              -                               |
| `Patch VAE-GAN` | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>Patch-based Video Autoencoder with Adversarial Training | Coming Soon |                              -                               |                              -                               |

### StyleGAN-based Generation
> Models leveraging StyleGAN's progressive architecture and style control for high-quality video generation.

|     Model     | Paper                                                        |   Venue    |                           Website                            |                            GitHub                            |
| :-----------: | :----------------------------------------------------------- | :--------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| `StyleVideoGAN` | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>StyleVideoGAN: A Temporal Generative Model using a Pretrained StyleGAN | Coming Soon |                              -                               |                              -                               |
| `StyleGAN-V`  | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>StyleGAN-V: A Continuous Video Generator with the Price, Image Quality and Perks of StyleGAN2 | Coming Soon |                              -                               |                              -                               |
| `StyleFaceV`  | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>StyleFaceV: Face Video Generation via Decomposing and Recomposing Pretrained StyleGAN2 | Coming Soon |                              -                               |                              -                               |
| `StyleHEAT`   | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>StyleHEAT: One-Shot High-Resolution Editable Talking Face Generation via Pre-trained StyleGAN | Coming Soon |                              -                               |                              -                               |

---

## 🌊 Diffusion-based Models

> Diffusion models have emerged as the dominant paradigm in video generation, offering superior quality and controllability through iterative denoising processes.

### 1. UNet with Temporal Modules
> Models leveraging UNet architectures with temporal modules for video generation.

|           Model            | Paper                                                        |   Venue    |                           Website                            |                            GitHub                            |
| :------------------------: | :----------------------------------------------------------- | :--------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|      ` Make-A-Video`       | [![arXiv](https://img.shields.io/badge/arXiv-2209.14792-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2209.14792)<br>Make-A-Video: Text-to-Video Generation without Text-Video Data | arXiv 2022 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://arxiv.org/abs/2209.14792) |                              -                               |
|       `Imagen Video`       | [![arXiv](https://img.shields.io/badge/arXiv-2210.02303-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2210.02303)<br>Imagen Video: High Definition Video Generation with Diffusion Models | arXiv 2022 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://imagen.research.google/video) |                              -                               |
|       `Magic Video`        | [![arXiv](https://img.shields.io/badge/arXiv-2211.11018-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2211.11018)<br>MagicVideo: Efficient Video Generation With Latent Diffusion Models | arXiv 2022 |                              -                               |                              -                               |
|           `LVDM`           | [![arXiv](https://img.shields.io/badge/arXiv-2211.13221-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2211.13221)<br>Latent Video Diffusion Models for High-Fidelity Long Video Generation | arXiv 2022 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://yingqinghe.github.io/LVDM/) | [![GitHub](https://img.shields.io/github/stars/YingqingHe/LVDM)](https://github.com/YingqingHe/LVDM) |
|       `Latent-Shift`       | [![arXiv](https://img.shields.io/badge/arXiv-2304.08477-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2304.08477)<br>Latent-Shift: Latent Diffusion with Temporal Shift for Efficient Text-to-Video Generation | arXiv 2023 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://latent-shift.github.io) |                              -                               |
| `Align-Your-<br/>Latents ` | [![arXiv](https://img.shields.io/badge/arXiv-2304.08818-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2304.08818)<br>Align your Latents: High-Resolution Video Synthesis with Latent Diffusion Models | CVPR 2023  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://research.nvidia.com/labs/toronto-ai/VideoLDM/) |                              -                               |
|      `Video-Factory`       | [![arXiv](https://img.shields.io/badge/arXiv-2305.10874-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2305.10874)<br>Swap Attention in Spatiotemporal Diffusions for Text-to-Video Generation | arXiv 2023 |                              -                               |                              -                               |
|          `PYOCO`           | [![arXiv](https://img.shields.io/badge/arXiv-2305.10474-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2305.10474)<br>Preserve Your Own Correlation: A Noise Prior for Video Diffusion Models | ICCV 2023  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://research.nvidia.com/labs/dir/pyoco/) |                              -                               |
|       `Animatediff`        | [![arXiv](https://img.shields.io/badge/arXiv-2307.04725-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2307.04725)<br>AnimateDiff: Animate Your Personalized Text-to-Image Diffusion Models without Specific Tuning | ICLR 2024  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://animatediff.github.io/) | [![GitHub](https://img.shields.io/github/stars/guoyww/Animatediff)](https://github.com/guoyww/animatediff/) |
|      `ModelScopeT2V`       | [![arXiv](https://img.shields.io/badge/arXiv-2308.065711-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2308.06571)<br>ModelScope Text-to-Video Technical Report | arXiv 2023 |                              -                               |                              -                               |
|          `SimDA`           | [![arXiv](https://img.shields.io/badge/arXiv-2308.09710-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2308.09710)<br>SimDA: Simple Diffusion Adapter for Efficient Video Generation | CVPR 2024  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://chenhsing.github.io/SimDA/) | [![GitHub](https://img.shields.io/github/stars/ChenHsing/SimDA)](https://github.com/ChenHsing/SimDA) |
|        `Dysen-VDM`         | [![arXiv](https://img.shields.io/badge/arXiv-2308.13812-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2308.13812)<br>Dysen-VDM: Empowering Dynamics-aware Text-to-Video Diffusion with LLMs | CVPR 2024  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://haofei.vip/Dysen-VDM/) | [![GitHub](https://img.shields.io/github/stars/scofield7419/Dysen)](https://github.com/scofield7419/Dysen) |
|     `VideoDirectorGPT`     | [![arXiv](https://img.shields.io/badge/arXiv-2309.15091-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2309.15091)<br>VideoDirectorGPT: Consistent Multi-Scene Video Generation via LLM-Guided Planning | COLM 2024  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://videodirectorgpt.github.io) | [![GitHub](https://img.shields.io/github/stars/HL-hanlin/VideoDirectorGPT)](https://github.com/HL-hanlin/VideoDirectorGPT) |
|          `LAVIE `          | [![arXiv](https://img.shields.io/badge/arXiv-2310.07771-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2310.07771)<br>LaVie: High-Quality Video Generation with Cascaded Latent Diffusion Models | IJCV 2024  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://vchitect.github.io/LaVie-project/) | [![GitHub](https://img.shields.io/github/stars/Vchitect/LaVie)](https://github.com/Vchitect/LaVie) |
|      `DynamiCrafter`       | [![arXiv](https://img.shields.io/badge/arXiv-2310.12190-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2310.12190)<br>DynamiCrafter: Animating Open-domain Images with Video Diffusion Priors | ECCV 2024  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://doubiiu.github.io/projects/DynamiCrafter/) | [![GitHub](https://img.shields.io/github/stars/Doubiiu/Dynamicrafter)](https://github.com/Doubiiu/DynamiCrafter) |
|       `VideoCrafter`       | [![arXiv](https://img.shields.io/badge/arXiv-2310.19512-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2310.19512)<br>VideoCrafter1: Open Diffusion Models for High-Quality Video Generation | arXiv 2023 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://ailab-cvc.github.io/videocrafter2/) | [![GitHub](https://img.shields.io/github/stars/AILab-CVC/VideoCrafter)](https://github.com/AILab-CVC/VideoCrafter) |
|        `Emu-Video`         | [![arXiv](https://img.shields.io/badge/arXiv-2311.10709-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2311.10709)<br>Emu Video: Factorizing Text-to-Video Generation by Explicit Image Conditioning | ECCV 2024  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://luhannan.github.io/CogDrivingPage/) |                              -                               |
|        `PixelDance`        | [![arXiv](https://img.shields.io/badge/arXiv-2311.10982-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2311.10982)<br>Make Pixels Dance: High-Dynamic Video Generation | CVPR 2024  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://makepixelsdance.github.io) |                              -                               |
|           `SVD`            | [![arXiv](https://img.shields.io/badge/arXiv-2311.15127-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2311.15127v1)<br>Stable Video Diffusion: Scaling Latent Video Diffusion Models to Large Datasets | arXiv 2023 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://stability.ai/research/stable-video-diffusion-scaling-latent-video-diffusion-models-to-large-datasets) | [![GitHub](https://img.shields.io/github/stars/Stability-AI/generative-models)](https://github.com/Stability-AI/generative-models?tab=readme-ov-file) |
|       `MicroCinema`        | [![arXiv](https://img.shields.io/badge/arXiv-2311.18829-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2311.18829)<br>MicroCinema: A Divide-and-Conquer Approach for Text-to-Video Generation | CVPR 2024  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://wangyanhui666.github.io/MicroCinema.github.io/) |                              -                               |
|          `Show-1`          | [![arXiv](https://img.shields.io/badge/arXiv-2312.02934-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2312.02934)<br>Show-1: Marrying Pixel and Latent Diffusion Models for Text-to-Video Generation |  IJCV2024  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://showlab.github.io/Show-1/) | [![GitHub](https://img.shields.io/github/stars/showlab/Show-1)](https://github.com/showlab/Show-1) |
|      `MagicVideo v2`       | [![arXiv](https://img.shields.io/badge/arXiv-2401.04468-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2401.04468)<br>MagicVideo-V2: Multi-Stage High-Aesthetic Video Generation | arXiv 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://magicvideov2.github.io) |                              -                               |
|        `FlexiFilm`         | [![arXiv](https://img.shields.io/badge/arXiv-2404.18620-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2404.18620)<br>FlexiFilm: Long Video Generation with Flexible Conditions | arxiv 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://y-ichen.github.io/FlexiFilm-Page/) | [![GitHub](https://img.shields.io/github/stars/Y-ichen/FlexiFilm)](https://github.com/Y-ichen/FlexiFilm) |
|      `VideoCrafter2`       | [![arXiv](https://img.shields.io/badge/arXiv-2409.01595-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2409.01595)<br>VideoCrafter2: Overcoming Data Limitations for High-Quality Video Diffusion Models | arXiv 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://ailab-cvc.github.io/videocrafter2/) | [![GitHub](https://img.shields.io/github/stars/AILab-CVC/VideoCrafter)](https://github.com/AILab-CVC/VideoCrafter) |


### 2. Diffusion Transformers
> Models using transformer-based architectures for video diffusion.

|      Model       | Paper                                                        |   Venue    |                           Website                            |                            GitHub                            |
| :--------------: | :----------------------------------------------------------- | :--------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|      `VDT`       | [![arXiv](https://img.shields.io/badge/arXiv-2305.13311-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2305.13311)<br>VDT: General-purpose Video Diffusion Transformers via Mask Modeling | ICLR 2024  |                              -                               | [![GitHub](https://img.shields.io/github/stars/RERV/VDT)](https://github.com/RERV/VDT) |
|    `GenTron`     | [![arXiv](https://img.shields.io/badge/arXiv-2312.04557-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2312.04557)<br>GenTron: Diffusion Transformers for Image and Video Generation | CVPR 2024  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.shoufachen.com/gentron_website/) |                              -                               |
|    `W.A.L.T`     | [![arXiv](https://img.shields.io/badge/arXiv-2312.06662-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2312.06662)<br>Photorealistic Video Generation with Diffusion Models | arXiv 2023 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://walt-video-diffusion.github.io) |                              -                               |
|     `Latte`      | [![arXiv](https://img.shields.io/badge/arXiv-2401.03048-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2401.03048)<br> Latte: Latent Diffusion Transformer for Video Generation | TMLR 2025  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://maxin-cn.github.io/latte_project/) | [![GitHub](https://img.shields.io/github/stars/Vchitect/Latte)](https://github.com/Vchitect/Latte) |
|   `SnapVideo`    | [![](https://img.shields.io/badge/arXiv-2402.14797-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2402.14797)<br>Snap Video: Scaled Spatiotemporal Transformers for Text-to-Video Synthesis | arXiv 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://snap-research.github.io/snapvideo/) |                              -                               |
|   `CogvideoX`    | [![arXiv](https://img.shields.io/badge/arXiv-2408.06072-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2408.06072)<br>CogVideoX: Text-to-Video Diffusion Models with An Expert Transformer | ICLR 2025  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://yzy-thu.github.io/CogVideoX-demo/) | [![GitHub](https://img.shields.io/github/stars/zai-org/CogVideo)](https://github.com/zai-org/CogVideo) |
|  `PyramidFlow`   | [![arXiv](https://img.shields.io/badge/arXiv-2410.05954-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.05954)<br>Pyramidal Flow Matching for Efficient Video Generative Modeling | ICLR 2025  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://pyramid-flow.github.io/) | [![GitHub](https://img.shields.io/github/stars/jy0205/Pyramid-Flow)](https://github.com/jy0205/Pyramid-Flow) |
|    `MovieGen`    | [![arXiv](https://img.shields.io/badge/arXiv-2410.13720-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.13720)<br>Movie Gen: A Cast of Media Foundation Models | arXIv 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://ai.meta.com/research/movie-gen/) |                              -                               |
| `Open-Sora-Plan` | [![arXiv](https://img.shields.io/badge/arXiv-2412.00131-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.00131)<br>Open-Sora Plan: Open-Source Large Video Generation Model | arXiv 2024 |                              -                               | [![GitHub](https://img.shields.io/github/stars/PKU-YuanGroup/Open-Sora-Plan)](https://github.com/PKU-YuanGroup/Open-Sora-Plan) |
| `Hunyuan Video`  | [![arXiv](https://img.shields.io/badge/arXiv-2412.03603-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.03603)<br>HunyuanVideo: A Systematic Framework For Large Video Generation Model | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aivideo.hunyuan.tencent.com) | [![GitHub](https://img.shields.io/github/stars/Tencent-Hunyuan/HunyuanVideo)](https://github.com/Tencent-Hunyuan/HunyuanVideo?tab=readme-ov-file) |
|   `LTX-Video`    | [![arXiv](https://img.shields.io/badge/arXiv-2501.00103-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2501.00103)<br>LTX-Video: Realtime Video Latent Diffusion | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://ltx.video) | [![GitHub](https://img.shields.io/github/stars/Lightricks/LTX-Video)](https://github.com/Lightricks/LTX-Video) |
|      `Goku`      | [![arXiv](https://img.shields.io/badge/arXiv-2502.04896-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.04896)<br>Goku: Flow Based Video Generative Foundation Models | CVPR 2025  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://saiyan-world.github.io/goku/) | [![GitHub](https://img.shields.io/github/stars/Saiyan-World/goku)](https://github.com/Saiyan-World/goku) |
|  `Lumina-Video`  | [![arXiv](https://img.shields.io/badge/arXiv-2502.06782-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.06782)<br>Lumina-Video: Efficient and Flexible Video Generation with Multi-scale Next-DiT | arXiv 2025 |                              -                               | [![GitHub](https://img.shields.io/github/stars/Alpha-VLLM/Lumina-Video)](https://github.com/Alpha-VLLM/Lumina-Video) |
| `Step-Video T2V` | [![arXiv](https://img.shields.io/badge/arXiv-2502.10248-b31b1b?style=flat-square&logo=arxiv)](htttps://arxiv.org/abs/2502.10248)<br>Step-Video-T2V Technical Report: The Practice, Challenges, and Future of Video Foundation Model | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://yuewen.cn/videos) | [![GitHub](https://img.shields.io/github/stars/stepfun-ai/Step-Video-T2V)](https://github.com/stepfun-ai/Step-Video-T2V) |
|    `FullDiT`     | [![arXiv](https://img.shields.io/badge/arXiv-2503.19907-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.19907)<br>FullDiT: Multi-Task Video Generative Foundation Model with Full Attention | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://fulldit.github.io) |                              -                               |
|      `Wan`       | [![arXiv](https://img.shields.io/badge/arXiv-2503.20314-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.20314)<br>Wan: Open and Advanced Large-Scale Video Generative Models | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://wan.video) | [![GitHub](https://img.shields.io/github/stars/Wan-Video/Wan2.1)](ttps://github.com/Wan-Video/Wan2.1) |


### 3. Efficient Video Diffusion Models
> Models optimized for efficiency in video generation through various acceleration and optimization techniques.

|     Model     | Paper                                                        |    Venue     |                           Website                            |                            GitHub                            |
| :-----------: | :----------------------------------------------------------- | :----------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|    `PVDM`     | [![arXiv](https://img.shields.io/badge/arXiv-2302.07685-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2302.07685)<br>Video Probabilistic Diffusion Models in Projected Latent Space |  CVPR 2023   | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://sihyun.me/PVDM/) | [![GitHub](https://img.shields.io/github/stars/sihyun-yu/PVDM)](https://github.com/sihyun-yu/PVDM) |
| `VideoFusion` | [![arXiv](https://img.shields.io/badge/arXiv-2303.08320-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2303.08320)<br>VideoFusion: Decomposed Diffusion Models for High-Quality Video Generation |  CVPR 2023   |                              -                               |                              -                               |
|  `T2V-Zero`   | [![arXiv](https://img.shields.io/badge/arXiv-2303.13439-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2303.13439)<br>Text2Video-Zero: Text-to-Image Diffusion Models are Zero-Shot Video Generators |  ICCV 2023   | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://text2video-zero.github.io) | [![GitHub](https://img.shields.io/github/stars/Picsart-AI-Research/Text2Video-Zero)](https://github.com/Picsart-AI-Research/Text2Video-Zero) |
|  `DirectT2V`  | [![arXiv](https://img.shields.io/badge/arXiv-2305.14330-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2305.14330)<br>DirecT2V: Large Language Models are Frame-Level Directors for Zero-Shot Text-to-Video Generation |  arXiv 2023  |                              -                               | [![GitHub](https://img.shields.io/github/stars/cvlab-kaist/DirecT2V)](https://github.com/cvlab-kaist/DirecT2V) |
|   `GD-VDM`    | [![arXiv](https://img.shields.io/badge/arXiv-2306.11173-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2306.11173)<br>GD-VDM: Generated Depth for better Diffusion-based Video Generation |  ICCV 2025   |                              -                               | [![GitHub](https://img.shields.io/github/stars/lapid92/GD-VDM)](ttps://github.com/lapid92/GD-VDM/tree/main) |
|  `FreeBloom`  | [![arXiv](https://img.shields.io/badge/arXiv-2309.14494-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2309.14494)<br>Free-Bloom: Zero-Shot Text-to-Video Generator with LLM Director and LDM Animator | NeurIPS 2023 |                              -                               | [![GitHub](https://img.shields.io/github/stars/SooLab/Free-Bloom)](https://github.com/SooLab/Free-Bloom) |
|     `LVD`     | [![arXiv](https://img.shields.io/badge/arXiv-2309.17444-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2309.17444)<br>LLM-grounded Video Diffusion Models |  ICLR 2024   | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://llm-grounded-video-diffusion.github.io) | [![GitHub](https://img.shields.io/github/stars/TonyLianLong/LLM-groundedVideoDiffusion)](https://github.com/TonyLianLong/LLM-groundedVideoDiffusion) |
|     `CMD`     | [![arXiv](https://img.shields.io/badge/arXiv-2403.14148-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2403.14148)<br>Efficient Video Diffusion Models via Content-Frame Motion-Latent Decomposition |  ICLR 2024   | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://sihyun.me/CMD/) | [![GitHub](https://img.shields.io/github/stars/NVlabs/CMD)](https://github.com/NVlabs/CMD) |
|   `Matten`    | [![arXiv](https://img.shields.io/badge/arXiv-2405.03025-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2405.03025)<br/>Matten: Video Generation with Mamba-Attention |  arXiv 2024  |                              -                               |                              -                               |
|     `DiM`     | [![arXiv](https://img.shields.io/badge/arXiv-2405.15881-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2405.15881)<br>Scaling Diffusion Mamba with Bidirectional SSMs for Efficient Image and Video Generation |  arXiv 2024  |                              -                               |                              -                               |
| `Video-RWKV`  | [![arXiv](https://img.shields.io/badge/arXiv-2411.05636-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2411.05636)<br>Video RWKV:Video Action Recognition Based RWKV |  arXiv 2024  |                              -                               |                              -                               |
|  `GridDiff`   | [![arXiv](https://img.shields.io/badge/arXiv-2412.03934-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.03934)<br>Grid Diffusion Models for Text-to-Video Generation |  CVPR 2024   |                              -                               |                              -                               |
|   `LinGen`    | [![arXiv](https://img.shields.io/badge/arXiv-2412.09856-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.09856)<br>LinGen: Towards High-Resolution Minute-Length Text-to-Video Generation with Linear Computational Complexity |  CVPR 2025   | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://lineargen.github.io) | [![GitHub](https://img.shields.io/github/stars/jha-lab/LinGen)](https://github.com/jha-lab/LinGen) |

---

## 🔄 Autoregressive Models

> Autoregressive (AR) models represent the next frontier in video generation, leveraging next-token prediction frameworks for scalable and controllable video synthesis.

### Pixel-level AR Models
> Models that directly operate on raw pixel data using autoregressive prediction.

|     Model     | Paper                                                        |   Venue    |                           Website                            |                            GitHub                            |
| :-----------: | :----------------------------------------------------------- | :--------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| `VPN` | [![arXiv](https://img.shields.io/badge/arXiv-1610.00527-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/1610.00527)<br>Video Pixel Networks | ICML 2017 | - | - |
| `PMARD` | [![arXiv](https://img.shields.io/badge/arXiv-1703.03664-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/1703.03664)<br>Parallel Multiscale Autoregressive Density Estimation | ICML 2017 | - | - |
| `Video Transformer` | [![arXiv](https://img.shields.io/badge/arXiv-1906.02634-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/1906.02634)<br>Scaling Autoregressive Video Models | ICLR 2020 | - | - |

### Latent Space AR Models
> Models that perform autoregressive generation in compressed latent representations for improved efficiency.

|     Model     | Paper                                                        |   Venue    |                           Website                            |                            GitHub                            |
| :-----------: | :----------------------------------------------------------- | :--------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| `VideoGPT` | [![arXiv](https://img.shields.io/badge/arXiv-2104.10157-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2104.10157)<br>VideoGPT: Video Generation using VQ-VAE and Transformers | arXiv 2021 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://wilson1yan.github.io/videogpt/index.html) | [![GitHub](https://img.shields.io/github/stars/wilson1yan/VideoGPT)](https://github.com/wilson1yan/VideoGPT) |
| `TATS` | [![arXiv](https://img.shields.io/badge/arXiv-2204.03638-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2204.03638)<br>Long Video Generation with Time-Agnostic VQGAN and Time Sensitive Transformer | ECCV 2022 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://songweige.github.io/projects/tats) | [![GitHub](https://img.shields.io/github/stars/SongweiGe/TATS)](https://github.com/SongweiGe/TATS) |
| `MAGVIT` | [![arXiv](https://img.shields.io/badge/arXiv-2212.05199-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2212.05199)<br>MAGVIT: Masked Generative Video Transformer | CVPR 2023 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://magvit.cs.cmu.edu/) | [![GitHub](https://img.shields.io/github/stars/google-research/magvit)](https://github.com/google-research/magvit) |
| `MAGVIT-v2` | [![arXiv](https://img.shields.io/badge/arXiv-2310.05737-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2310.05737)<br>Language Model Beats Diffusion — Tokenizer Is Key to Visual Generation | ICLR 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://magvit.cs.cmu.edu/v2/) | - |
| `Open-MAGVIT2` | [![arXiv](https://img.shields.io/badge/arXiv-2409.04410-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2409.04410)<br>Open-MAGVIT2: An Open-Source Project Toward Democratizing Auto-regressive Visual Generation | arXiv 2024 | - | [![GitHub](https://img.shields.io/github/stars/TencentARC/SEED-Voken)](https://github.com/TencentARC/SEED-Voken) |
| `VidTok` | [![arXiv](https://img.shields.io/badge/arXiv-2412.13061-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.13061)<br>VidTok: A Versatile and Open-Source Video Tokenizer | arXiv 2024 | - | [![GitHub](https://img.shields.io/github/stars/microsoft/VidTok)](https://github.com/microsoft/VidTok) |
| `Omnitokenizer` | [![arXiv](https://img.shields.io/badge/arXiv-2406.09399-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2406.09399)<br>Omnitokenizer: A Joint Image-Video Tokenizer for Visual Generation | NeurIPS 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.wangjunke.info/OmniTokenizer/) | [![GitHub](https://img.shields.io/github/stars/FoundationVision/OmniTokenizer)](https://github.com/FoundationVision/OmniTokenizer) |
| `Cosmos` | [![arXiv](https://img.shields.io/badge/arXiv-2501.03575-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2501.03575)<br>Cosmos World Foundation Model Platform for Physical AI | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://research.nvidia.com/labs/dir/cosmos-tokenizer/) | [![GitHub](https://img.shields.io/github/stars/NVIDIA/Cosmos-Tokenizer)](https://github.com/NVIDIA/Cosmos-Tokenizer?tab=readme-ov-file) |
| `LARP` | [![arXiv](https://img.shields.io/badge/arXiv-2410.21264-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.21264)<br>Larp: Tokenizing Videos with a Learned Autoregressive Generative Prior | ICLR 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://hywang66.github.io/larp/) | [![GitHub](https://img.shields.io/github/stars/hywang66/LARP)](https://github.com/hywang66/LARP/) |
| `LVT` | [![arXiv](https://img.shields.io/badge/arXiv-2006.xxxx-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>Latent Video Transformer | arXiv 2020 | - | - |
| `GODIVA` | [![arXiv](https://img.shields.io/badge/arXiv-2104.xxxx-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>GODIVA: Generating Open-DomaIn Videos from nAtural Descriptions | arXiv 2021 | - | - |
| `HARP` | [![arXiv](https://img.shields.io/badge/arXiv-2209.07143-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2209.07143)<br>Harp: Autoregressive Latent Video Prediction with High-Fidelity Image Generator | ICIP 2022 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://sites.google.com/view/harp-videos/home) | - |
| `Nuwa-infinity` | [![arXiv](https://img.shields.io/badge/arXiv-2207.09814-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2207.09814)<br>Nuwa-infinity: Autoregressive over Autoregressive Generation for Infinite Visual Synthesis | NeurIPS 2022 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://nuwa-infinity.microsoft.com/#/NUWAInfinity) | - |
| `CogVideo` | [![arXiv](https://img.shields.io/badge/arXiv-2205.15868-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2205.15868)<br>CogVideo: Large-Scale Pretraining for Text-to-Video Generation via Transformers | arXiv 2022 | - | [![GitHub](https://img.shields.io/github/stars/THUDM/CogVideo)](https://github.com/THUDM/CogVideo) |
| `Transframer` | [![arXiv](https://img.shields.io/badge/arXiv-2203.09494-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2203.09494)<br>Transframer: Arbitrary Frame Prediction with Generative Models | TMLR 2023 | - | - |
| `IRIS` | [![arXiv](https://img.shields.io/badge/arXiv-2209.00588-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2209.00588)<br>Transformers are Sample Efficient World Models | ICLR 2023 | - | [![GitHub](https://img.shields.io/github/stars/eloialonso/iris)](https://github.com/eloialonso/iris) |
| `MOSO` | [![arXiv](https://img.shields.io/badge/arXiv-2303.03684-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2303.03684)<br>MOSO: Decomposing MOtion, Scene and Object for Video Prediction | CVPR 2023 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://iva-mzsun.github.io/MOSO) | [![GitHub](https://img.shields.io/github/stars/iva-mzsun/MOSO)](https://github.com/iva-mzsun/MOSO) |
| `PAR` | [![arXiv](https://img.shields.io/badge/arXiv-2412.15119-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.15119)<br>Parallelized Autoregressive Visual Generation | arXiv 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://epiphqny.github.io/PAR-project/) | [![GitHub](https://img.shields.io/github/stars/Epiphqny/PAR)](https://github.com/Epiphqny/PAR) |
| `VideoPoet` | [![arXiv](https://img.shields.io/badge/arXiv-2312.14125-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2312.14125)<br>VideoPoet: A Large Language Model for Zero-Shot Video Generation | ICML 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://sites.research.google/videopoet/) | - |
| `iVideoGPT` | [![arXiv](https://img.shields.io/badge/arXiv-2405.15223-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2405.15223)<br>iVideoGPT: Interactive VideoGPTs are Scalable World Models | NeurIPS 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://thuml.github.io/iVideoGPT/) | [![GitHub](https://img.shields.io/github/stars/thuml/iVideoGPT)](https://github.com/thuml/iVideoGPT) |
| `LVM` | [![arXiv](https://img.shields.io/badge/arXiv-2312.00785-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2312.00785)<br>Sequential Modeling Enables Scalable Learning for Large Vision Models | CVPR 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://yutongbai.com/lvm.html) | [![GitHub](https://img.shields.io/github/stars/ytongbai/LVM)](https://github.com/ytongbai/LVM) |
| `Loong` | [![arXiv](https://img.shields.io/badge/arXiv-2410.02757-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.02757)<br>Loong: Generating Minute-level Long Videos with Autoregressive Language Models | arXiv 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://epiphqny.github.io/Loong-video/) | - |
| `ARCON` | [![arXiv](https://img.shields.io/badge/arXiv-2412.03758v1-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.03758v1)<br>Advancing Auto-Regressive Continuation for Video Frames | arXiv 2024 | - | - |
| `Phenaki` | [![arXiv](https://img.shields.io/badge/arXiv-2210.02399-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2210.02399)<br>Phenaki: Variable Length Video Generation From Open Domain Textual Description | ICLR 2023  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://phenaki.video/) | - |
| `MaskViT` | [![arXiv](https://img.shields.io/badge/arXiv-2206.11894-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2206.11894)<br>Masked visual pre-training for video prediction | arXiv 2022 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://maskedvit.github.io/) | - |
| `WorldDreamer` | [![arXiv](https://img.shields.io/badge/arXiv-2401.09985-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2401.09985)<br>WorldDreamer: Towards General World Models for Video Generation via Predicting Masked Tokens | arXiv 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://world-dreamer.github.io/) | [![GitHub](https://img.shields.io/github/stars/PJLab-ADG/DriveArena)](https://github.com/PJLab-ADG/DriveArena) |
| `FACTOR` | [![arXiv](https://img.shields.io/badge/arXiv-2312.02919-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2312.02919)<br>Fine-grained controllable video generation via object appearance and context | WACV 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://hhsinping.github.io/factor/) | - |
| `NOVA` | [![arXiv](https://img.shields.io/badge/arXiv-2412.14169-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.14169)<br>AUTOREGRESSIVE VIDEO GENERATION WITHOUT VECTOR QUANTIZATION | ICLR 2025 | - | [![GitHub](https://img.shields.io/github/stars/baaivision/NOVA)](https://github.com/baaivision/NOVA) |

### Multimodal AR Models
> Models that integrate multiple modalities (text, audio, video) within unified autoregressive frameworks.

|     Model     | Paper                                                        |   Venue    |                           Website                            |                            GitHub                            |
| :-----------: | :----------------------------------------------------------- | :--------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| `UniVL` | [![arXiv](https://img.shields.io/badge/arXiv-2002.06353-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2002.06353)<br>UniVL: A Unified Video and Language Pre-Training Model for Multimodal Understanding and Generation | arXiv | - | [![GitHub](https://img.shields.io/github/stars/microsoft/UniVL)](https://github.com/microsoft/UniVL) |
| `Nüwa` | [![arXiv](https://img.shields.io/badge/arXiv-2111.12417-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2111.12417)<br>Nüwa: Visual synthesis pre-training for neural visual world creation | ECCV 2022  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://nuwa-infinity.microsoft.com/#/) | - |
| `MMVID` | [![arXiv](https://img.shields.io/badge/arXiv-2203.02573-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2203.02573)<br>Show Me What and Tell Me How: Video Synthesis via Multimodal Conditioning | CVPR 2022 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://snap-research.github.io/MMVID/) | [![GitHub](https://img.shields.io/github/stars/snap-research/MMVID)](https://github.com/snap-research/MMVID) |
| `MMVG` | [![arXiv](https://img.shields.io/badge/arXiv-2211.12824-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2211.12824)<br>Tell Me What Happened: Unifying Text-guided Video Completion via Multimodal Masked Video Generation | CVPR 2023 | - | - |
| `EMU` | [![arXiv](https://img.shields.io/badge/arXiv-2307.05222-b31b1b?style=flat-square&logo=arxiv)](http://arxiv.org/abs/2307.05222)<br>EMU: GENERATIVE PRETRAINING IN MULTIMODALITY | ICLR 2024 | - | [![GitHub](https://img.shields.io/github/stars/baaivision/Emu)](https://github.com/baaivision/Emu) |
| `JAM` | [![arXiv](https://img.shields.io/badge/arXiv-2309.15564-b31b1b?style=flat-square&logo=arxiv)](http://arxiv.org/abs/2309.15564)<br>JOINTLY TRAINING LARGE AUTOREGRESSIVE MULTIMODAL MODELS | ICLR 2024 | - | [![GitHub](https://img.shields.io/github/stars/kyegomez/MultiModalCrossAttn)](https://github.com/kyegomez/MultiModalCrossAttn) |
| `NExT-GPT` | [![arXiv](https://img.shields.io/badge/arXiv-2309.05519-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2309.05519)<br>NExT-GPT: Any-to-Any Multimodal LLM | ICML 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://next-gpt.github.io/) | [![GitHub](https://img.shields.io/github/stars/NExT-GPT/NExT-GPT)](https://github.com/NExT-GPT/NExT-GPT) |
| `GPT4Video` | [![arXiv](https://img.shields.io/badge/arXiv-2311.16511-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2311.16511)<br>GPT4Video: A Unified Multimodal Large Language Model for Instruction-Followed Understanding and Safety-Aware Generation | MM 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://gpt4video.github.io/) | [![GitHub](https://img.shields.io/github/stars/gpt4video/GPT4Video)](https://github.com/gpt4video/GPT4Video) |
| `CoDi-2` | [![arXiv](https://img.shields.io/badge/arXiv-2311.18775-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2311.18775)<br>CoDi-2: In-Context, Interleaved, and Interactive Any-to-Any Generation | arXiv 2023 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://codi-2.github.io/) | [![GitHub](https://img.shields.io/github/stars/microsoft/i-Code)](https://github.com/microsoft/i‑Code/tree/main/CoDi‑2) |
| `Emu2` | [![arXiv](https://img.shields.io/badge/arXiv-2312.13286-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2312.13286)<br>Generative Multimodal Models are In-Context Learners | CVPR 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://baaivision.github.io/emu2/) | [![GitHub](https://img.shields.io/github/stars/baaivision/Emu)](https://github.com/baaivision/Emu) |
| `Moonshot` | [![arXiv](https://img.shields.io/badge/arXiv-2401.01827-b31b1b?style=flat-square&logo=arxiv)](http://arxiv.org/abs/2401.01827)<br>Moonshot: Towards Controllable Video Generation and Editing with Multimodal Conditions | IJCV 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://showlab.github.io/Moonshot/) | - |
| `Video‑LaVIT` | [![arXiv](https://img.shields.io/badge/arXiv-2402.03161-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2402.03161)<br>Video‑LaVIT: Unified Video‑Language Pre‑training with Decoupled Visual‑Motional Tokenization | ICML 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://video-lavit.github.io/) | [![GitHub](https://img.shields.io/github/stars/jy0205/LaVIT)](https://github.com/jy0205/LaVIT) |
| `LWM` | [![arXiv](https://img.shields.io/badge/arXiv-2402.08268-b31b1b?style=flat-square&logo=arxiv)](http://arxiv.org/abs/2402.08268)<br>World Model on Million‑Length Video and Language with Blockwise RingAttention | ICLR 2025  | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://largeworldmodel.github.io/lwm/) | [![GitHub](https://img.shields.io/github/stars/LargeWorldModel/LWM)](https://github.com/LargeWorldModel/LWM) |
| `X-VILA` | [![arXiv](https://img.shields.io/badge/arXiv-2405.19335-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/pdf/2405.19335)<br>X-VILA: Cross-Modality Alignment for Large Language Model | arXiv 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://video-lavit.github.io/) | [![GitHub](https://img.shields.io/github/stars/jy0205/LaVIT)](https://github.com/jy0205/LaVIT) |
| `SHOW‑O` | [![arXiv](https://img.shields.io/badge/arXiv-2408.12528-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2408.12528)<br>SHOW‑O: ONE SINGLE TRANSFORMER TO UNIFY MULTIMODAL UNDERSTANDING AND GENERATION | ICLR 2025 | - | [![GitHub](https://img.shields.io/github/stars/showlab/Show-o)](https://github.com/showlab/Show-o) |
| `VILA‑U` | [![arXiv](https://img.shields.io/badge/arXiv-2409.04429-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2409.04429)<br>VILA‑U: A Unified Foundation Model Integrating Visual Understanding and Generation | ICLR 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://hanlab.mit.edu/projects/vila-u) | [![GitHub](https://img.shields.io/github/stars/mit-han-lab/vila-u)](https://github.com/mit-han-lab/vila-u) |
| `MIO` | [![arXiv](https://img.shields.io/badge/arXiv-2409.17692-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2409.17692)<br>MIO: A Foundation Model on Multimodal Tokens | arXiv 2024 | - | [![GitHub](https://img.shields.io/github/stars/MIO-Team/MIO)](https://github.com/MIO-Team/MIO) |
| `Emu3` | [![arXiv](https://img.shields.io/badge/arXiv-2409.18869-b31b1b?style=flat-square&logo=arxiv)](http://arxiv.org/abs/2409.18869)<br>Emu3: Next-Token Prediction is All You Need | arXiv 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://emu.baai.ac.cn/about) | [![GitHub](https://img.shields.io/github/stars/baaivision/Emu3)](https://github.com/baaivision/Emu3) |
| `Janus` | [![arXiv](https://img.shields.io/badge/arXiv-2410.13848-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.13848)<br>Janus: Decoupling Visual Encoding for Unified Multimodal Understanding and Generation | CVPR 2025 | - | [![GitHub](https://img.shields.io/github/stars/deepseek-ai/Janus)](https://github.com/deepseek-ai/Janus) |
| `Janusflow` | [![arXiv](https://img.shields.io/badge/arXiv-2411.07975-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2411.07975)<br>Janusflow: Harmonizing autoregression and rectified flow for unified multimodal understanding and generation | CVPR 2025 | - | [![GitHub](https://img.shields.io/github/stars/deepseek-ai/Janus)](https://github.com/deepseek-ai/Janus) |
| `Tokenflow` | [![arXiv](https://img.shields.io/badge/arXiv-2412.03069-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.03069)<br>Tokenflow: Unified image tokenizer for multimodal understanding and generation | CVPR 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://bytevisionlab.github.io/TokenFlow/) | [![GitHub](https://img.shields.io/github/stars/ByteVisionLab/TokenFlow)](https://github.com/ByteVisionLab/TokenFlow) |
| `GEM` | [![arXiv](https://img.shields.io/badge/arXiv-2412.11198-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.11198)<br>A Generalizable Ego-Vision Multimodal World Model for Fine-Grained Ego-Motion, Object Dynamics, and Scene Composition Control | CVPR 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://vita-epfl.github.io/GEM.github.io/) | [![GitHub](https://img.shields.io/github/stars/vita-epfl/GEM)](https://github.com/vita-epfl/GEM) |
| `MetaMorph` | [![arXiv](https://img.shields.io/badge/arXiv-2412.14164-b31b1b?style=flat-square&logo=arxiv)](http://arxiv.org/abs/2412.14164)<br>MetaMorph: Multimodal Understanding and Generation via Instruction Tuning | arXiv | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://tsb0601.github.io/metamorph/) | [![GitHub](https://img.shields.io/github/stars/facebookresearch/metamorph)](https://github.com/facebookresearch/metamorph/) |
| `Unitok` | [![arXiv](https://img.shields.io/badge/arXiv-2502.20321-b31b1b?style=flat-square&logo=arxiv)](http://arxiv.org/abs/2502.20321)<br>Unitok: A unified tokenizer for visual generation and understanding | arXiv | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://foundationvision.github.io/UniTok/) | [![GitHub](https://img.shields.io/github/stars/FoundationVision/UniTok)](https://github.com/FoundationVision/UniTok) |
| `WISE` | [![arXiv](https://img.shields.io/badge/arXiv-2503.07265-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.07265)<br>WISE: A World Knowledge-Informed Semantic Evaluation for Text-to-Image Generation | arXiv | - | [![GitHub](https://img.shields.io/github/stars/PKU-YuanGroup/WISE)](https://github.com/PKU-YuanGroup/WISE) |
| `MetaQueries` | [![arXiv](https://img.shields.io/badge/arXiv-2504.06256-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.06256)<br>Transfer between Modalities with MetaQueries | arXiv | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://xichenpan.com/metaquery/) | [![GitHub](https://img.shields.io/github/stars/facebookresearch/metaquery)](https://github.com/facebookresearch/metaquery) |
| `Unitoken` | [![arXiv](https://img.shields.io/badge/arXiv-2504.04423-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.04423)<br>Unitoken: Harmonizing multimodal understanding and generation through unified visual encoding | CVPRW 2025 | - | [![GitHub](https://img.shields.io/github/stars/SxJyJay/UniToken)](https://github.com/SxJyJay/UniToken) |
| `BAGEL` | [![arXiv](https://img.shields.io/badge/arXiv-2505.14683-b31b1b?style=flat-square&logo=arxiv)](http://arxiv.org/abs/2505.14683)<br>Emerging Properties in Unified Multimodal Pretraining | arXiv| - |-|
| `Mogao` | [![arXiv](https://img.shields.io/badge/arXiv-2505.05472-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.05472)<br>Mogao: An Omni Foundation Model for Interleaved Multi-Modal Generation | arXiv | - | - |
| `BLIP3-o` | [![arXiv](https://img.shields.io/badge/arXiv-2505.09568-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.09568)<br>BLIP3-o: A Family of Fully Open Unified Multimodal Models-Architecture, Training and Dataset | arXiv | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://jiuhaichen.github.io/BLIP3o-NEXT.github.io/) | [![GitHub](https://img.shields.io/github/stars/JiuhaiChen/BLIP3o)](https://github.com/JiuhaiChen/BLIP3o) |
| `Muddit` | [![arXiv](https://img.shields.io/badge/arXiv-2505.23606-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.23606)<br>Muddit: Liberating Generation Beyond Text-to-Image with a Unified Discrete Diffusion Model | arXiv | - | [![GitHub](https://img.shields.io/github/stars/M-E-AGI-Lab/Muddit)](https://github.com/M-E-AGI-Lab/Muddit) |
| `UniWorld` | [![arXiv](https://img.shields.io/badge/arXiv-2506.03147-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2506.03147)<br>UniWorld: High-Resolution Semantic Encoders for Unified Visual Understanding and Generation | arXiv | - | [![GitHub](https://img.shields.io/github/stars/PKU-YuanGroup/UniWorld-V1)](https://github.com/PKU-YuanGroup/UniWorld-V1) |
| `Show-o2` | [![arXiv](https://img.shields.io/badge/arXiv-2506.15564-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2506.15564)<br>Show-o2: Improved Native Unified Multimodal Models | NeurIPS 2025 | - | [![GitHub](https://img.shields.io/github/stars/showlab/Show-o)](https://github.com/showlab/Show-o) |
| `Qwen-Image` | [![arXiv](https://img.shields.io/badge/arXiv-2508.02324-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2508.02324)<br>Qwen-Image Technical Report | arXiv | - | [![GitHub](https://img.shields.io/github/stars/QwenLM/Qwen-Image)](https://github.com/QwenLM/Qwen-Image) |
| `RecA` | [![arXiv](https://img.shields.io/badge/arXiv-2509.07295-b31b1b?style=flat-square&logo=arxiv)](https://www.arxiv.org/abs/2509.07295)<br>Reconstruction Alignment Improves Unified Multimodal Models | arXiv | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://reconstruction-alignment.github.io/) | [![GitHub](https://img.shields.io/github/stars/HorizonWind2004/reconstruction-alignment)](https://github.com/HorizonWind2004/reconstruction-alignment) |

---

## 📊 Benchmarks & Evaluation

> Comprehensive evaluation frameworks for assessing video generation quality, temporal consistency, and semantic alignment.

### Quality & Fidelity Benchmarks
|   Benchmark   | Paper                                                        |   Venue    |                           Website                            |                            GitHub                            |
| :-----------: | :----------------------------------------------------------- | :--------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|   `VBench`    | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>VBench: Comprehensive Benchmark Suite for Video Generative Models | Coming Soon |                              -                               |                              -                               |
| `T2V-CompBench` | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>T2V-CompBench: A Comprehensive Benchmark for Compositional Text-to-video Generation | Coming Soon |                              -                               |                              -                               |
| `VBench-2.0`  | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>VBench-2.0: Evaluating Video Generation with Human-Centric Metrics | Coming Soon |                              -                               |                              -                               |

### Specialized Evaluation
|   Benchmark   | Paper                                                        |   Venue    |                           Website                            |                            GitHub                            |
| :-----------: | :----------------------------------------------------------- | :--------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| `MovieBench`  | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>MovieBench: Long Video Generation Benchmark | Coming Soon |                              -                               |                              -                               |
| `ChronoMagic-Bench` | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>ChronoMagic-Bench: A Benchmark for Metamorphic Evaluation of Text-to-Time-lapse Video Generation | Coming Soon |                              -                               |                              -                               |
| `T2VSafetyBench` | [![arXiv](https://img.shields.io/badge/arXiv-Coming_Soon-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/)<br>T2VSafetyBench: Evaluating the Safety of Text-to-Video Generation | Coming Soon |                              -                               |                              -                               |

---

## 🎯 Applications & Downstream Tasks

> Real-world applications and specialized tasks enabled by video generation models.

### Content Creation & Entertainment
- **Film & Animation**: Automated scene generation, character animation, visual effects
- **Gaming**: Procedural content generation, dynamic environments, NPC behavior
- **Social Media**: Short-form video creation, content augmentation, viral content generation

### Education & Training
- **Educational Content**: Interactive learning materials, historical recreations, scientific visualizations
- **Professional Training**: Simulation-based training, safety scenarios, skill development
- **Language Learning**: Immersive language environments, cultural context videos

### Scientific & Industrial Applications
- **Autonomous Driving**: Simulation environments, edge case generation, safety testing
- **Robotics**: Behavior prediction, environment simulation, training data generation
- **Medical**: Surgical training, patient education, therapy applications
- **Climate & Weather**: Environmental modeling, disaster simulation, climate visualization

### Virtual & Augmented Reality
- **Metaverse**: Virtual world creation, avatar animation, social interactions
- **AR Applications**: Real-time content overlay, interactive experiences, spatial computing
- **Digital Twins**: Industrial simulation, urban planning, architectural visualization

---

## 📈 Timeline & Evolution

```mermaid
timeline
    title Video Generation Evolution
    
    2014-2017 : Early GANs
              : VGAN
              : 3D-Conv
              : Basic temporal modeling
    
    2018-2020 : Advanced GANs
              : MoCoGAN
              : DVD-GAN
              : StyleGAN-based methods
              : Progressive generation
    
    2021-2022 : Diffusion Era Begins
              : DDPM for video
              : Make-A-Video
              : Imagen Video
              : LVDM
    
    2023      : Diffusion Dominance
              : Stable Video Diffusion
              : AnimateDiff
              : LaVie
              : Text-to-video breakthroughs
    
    2024-2025 : Multimodal & AR
              : Sora
              : CogVideoX
              : Autoregressive models
              : World model paradigms
```

---


## 🔬 Research Trends & Future Directions

### 🚧 Current Challenges
- **⏱️ Temporal Consistency**: Maintaining coherent motion and object persistence across frames
- **⚡ Computational Efficiency**: Reducing inference time and memory requirements
- **🎛️ Controllability**: Fine-grained control over generation process and content
- **📹 Long-form Generation**: Scaling to minute-length or longer videos
- **🔗 Multimodal Integration**: Seamless fusion of text, audio, and visual modalities

### 📈 Emerging Trends
- **🌍 World Models**: Building comprehensive environmental representations
- **🔄 Autoregressive Scaling**: Leveraging LLM-style scaling laws for video
- **⚡ Real-time Generation**: Achieving interactive generation speeds
- **👤 Personalization**: User-specific content generation and style adaptation
- **🛡️ Safety & Ethics**: Ensuring responsible AI development and deployment

### 🔮 Future Opportunities
- **🎮 Interactive Video Generation**: Real-time user interaction and modification
- **🧠 Cross-modal Understanding**: Deep integration of vision, language, and audio
- **🔗 Causal Reasoning**: Understanding and modeling cause-effect relationships
- **⚖️ Physical Simulation**: Accurate physics-based video generation
- **🤝 Collaborative Creation**: Human-AI collaborative content creation workflows

---

## 🤝 Contributing

We welcome contributions to this survey! Please feel free to:

- **Add new papers**: Submit PRs with new video generation models
- **Update information**: Correct errors or add missing details
- **Suggest improvements**: Propose better categorization or organization
- **Report issues**: Flag broken links or outdated information

### Contribution Guidelines
1. Follow the existing format for consistency
2. Include paper title, authors, venue, and links
3. Provide brief, accurate descriptions
4. Ensure all links are functional
5. Maintain chronological order within categories

---

## 📚 Citation

If you find this survey useful for your research, please consider citing:

```bibtex
@article{hu2025video,
  title={Video Generation Foundation Model: A Survey},
  author={Hu, Teng and Jiangning Zhang, Huang, Hongrui, Ran Yi, Zihan Su, Jieyu Weng, Zhucun Xue, Lizhuang Ma},
  journal={Arxiv},
  year={2025}
}
```

---



## 🔗 Resources & Links

### Related Surveys & Resources
- [Awesome Diffusion Models](https://github.com/heejkoo/Awesome-Diffusion-Models)
- [Awesome Video Generation](https://github.com/yzhang2016/video-generation-survey)
- [Awesome Multimodal ML](https://github.com/pliang279/awesome-multimodal-ml)
- [Papers With Code - Video Generation](https://paperswithcode.com/task/video-generation)

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

We thank the video generation research community for their groundbreaking work and the open-source contributors who make this field accessible to everyone. Special thanks to all the authors whose papers are included in this survey.

---

<div align="center">
  <img src="https://img.shields.io/github/stars/worldbench/survey?style=social" alt="GitHub stars">
  <img src="https://img.shields.io/github/forks/worldbench/survey?style=social" alt="GitHub forks">
  <img src="https://img.shields.io/github/watchers/worldbench/survey?style=social" alt="GitHub watchers">
</div>

<div align="center">
  <strong>⭐ Star this repository if you find it helpful! ⭐</strong>
</div>