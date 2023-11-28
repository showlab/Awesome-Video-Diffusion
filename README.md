# Awesome Video Diffusion [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) <!-- omit in toc -->
A curated list of recent diffusion models for video generation, editing, restoration, understanding, nerf, etc.

<p align="center">
<img src="https://makeavideo.studio/assets/overview.webp" width="240px"/>
<img src="https://makeavideo.studio/assets/A_teddy_bear_painting_a_portrait.webp" width="240px"/>    
</p>

<p align="center">
<img src="https://tuneavideo.github.io/assets/teaser.gif" width="480px"/>  
</p>

<p align="center">
<img src="https://github.com/ChenyangQiQi/FateZero/blob/main/docs/gif_results/17_car_posche_01_concat_result.gif?raw=true" width="240px"/>
<img src="https://github.com/ChenyangQiQi/FateZero/blob/main/docs/gif_results/3_sunflower_vangogh_conat_result.gif?raw=true" width="240px"/>    
</p>

<p align="center">
(Source: <a href="https://makeavideo.studio/">Make-A-Video</a>, <a href="https://tuneavideo.github.io/">Tune-A-Video</a>, and <a href="https://fate-zero-edit.github.io/">Fate/Zero</a>.)
</p>


## Table of Contents <!-- omit in toc -->
- [Open-source Toolboxes and Foundation Models](#open-source-toolboxes-and-foundation-models)
- [Video Generation](#video-generation)
- [Video Editing](#video-editing)
- [Long-form Video Generation and Completion](#long-form-video-generation-and-completion)
- [Human or Subject Motion](#human-or-subject-motion)
- [Video Enhancement and Restoration](#video-enhancement-and-restoration)
- [3D / NeRF](#3d--nerf)
- [Video Understanding](#video-understanding)
- [Healthcare and Biology](#healthcare-and-biology)

### Open-source Toolboxes and Foundation Models 

+ [Stable Video Diffusion](https://github.com/Stability-AI/generative-models)  
  [![Star](https://img.shields.io/github/stars/Stability-AI/generative-models.svg?style=social&label=Star)](https://github.com/Stability-AI/generative-models)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://stability.ai/news/stable-video-diffusion-open-ai-video-model) 

+ [Hotshot-XL (text-to-GIF)](https://huggingface.co/cerspense/zeroscope_v2_576w)  
  [![Star](https://img.shields.io/github/stars/hotshotco/Hotshot-XL.svg?style=social&label=Star)](https://github.com/hotshotco/Hotshot-XL)

+ [zeroscope_v2](https://huggingface.co/cerspense/zeroscope_v2_576w)  
  [![Website](https://img.shields.io/badge/576w-9cf)](https://huggingface.co/cerspense/zeroscope_v2_576w) 
  [![Website](https://img.shields.io/badge/XL-9cf)](https://huggingface.co/cerspense/zeroscope_v2_XL) 

+ [I2VGen-XL (image-to-video / video-to-video)](https://modelscope.cn/models/damo/Image-to-Video/summary)  
  [![Website](https://img.shields.io/badge/Website(I2V)-9cf)](https://modelscope.cn/models/damo/Image-to-Video/summary) 
  [![Website](https://img.shields.io/badge/Website(V2V)-9cf)](https://modelscope.cn/models/damo/Video-to-Video/summary) 

+ [text-to-video-synthesis-colab](https://github.com/camenduru/text-to-video-synthesis-colab)  
  [![Star](https://img.shields.io/github/stars/camenduru/text-to-video-synthesis-colab.svg?style=social&label=Star)](https://github.com/camenduru/text-to-video-synthesis-colab)

+ [VideoCrafter: A Toolkit for Text-to-Video Generation and Editing](https://github.com/VideoCrafter/VideoCrafter)  
  [![Star](https://img.shields.io/github/stars/VideoCrafter/VideoCrafter.svg?style=social&label=Star)](https://github.com/VideoCrafter/VideoCrafter)

+ [ModelScope (Text-to-video synthesis)](https://modelscope.cn/models/damo/text-to-video-synthesis/summary)  
  [![Star](https://img.shields.io/github/stars/modelscope/modelscope.svg?style=social&label=Star)](https://github.com/modelscope/modelscope)

+ [Diffusers (Text-to-video synthesis)](https://huggingface.co/docs/diffusers/main/en/api/pipelines/text_to_video#texttovideo-synthesis)  
  [![Star](https://img.shields.io/github/stars/huggingface/diffusers.svg?style=social&label=Star)](https://github.com/huggingface/diffusers)

### Video Generation 

+ [FusionFrames: Efficient Architectural Aspects for Text-to-Video Generation Pipeline](https://arxiv.org/abs/2311.13073) (Nov., 2023)  
  [![Star](https://img.shields.io/github/stars/ai-forever/KandinskyVideo.svg?style=social&label=Star)](https://github.com/ai-forever/KandinskyVideo)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.13073)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://ai-forever.github.io/kandinsky-video/)

+ [Fine-Grained Open Domain Image Animation with Motion Guidance](https://arxiv.org/abs/2311.12886) (Nov., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.12886)

+ [GPT4Motion: Scripting Physical Motions in Text-to-Video Generation via Blender-Oriented GPT Planning](https://arxiv.org/abs/2311.12631) (Nov., 2023)  
  [![Star](https://img.shields.io/github/stars/jiaxilv/GPT4Motion.svg?style=social&label=Star)](https://github.com/jiaxilv/GPT4Motion)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.12631)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://gpt4motion.github.io/)

+ [MagicDance: Realistic Human Dance Video Generation with Motions & Facial Expressions Transfer](https://arxiv.org/abs/2311.12052) (Nov., 2023)  
  [![Star](https://img.shields.io/github/stars/Boese0601/MagicDance.svg?style=social&label=Star)](https://github.com/Boese0601/MagicDance)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.12052)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://boese0601.github.io/magicdance/)

+ [MoVideo: Motion-Aware Video Generation with Diffusion Models](https://arxiv.org/abs/2311.11325) (Nov., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.11325)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://jingyunliang.github.io/MoVideo/)

+ [Make Pixels Dance: High-Dynamic Video Generation](https://arxiv.org/abs/2311.10982) (Nov., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.10982)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://makepixelsdance.github.io/)

+ [Emu Video: Factorizing Text-to-Video Generation by Explicit Image Conditioning](https://arxiv.org/abs/2311.10709) (Nov., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.10709)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://emu-video.metademolab.com/)
  
+ [Optimal Noise pursuit for Augmenting Text-to-Video Generation](https://arxiv.org/abs/2311.00949) (Nov., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.00949)

+ [VideoDreamer: Customized Multi-Subject Text-to-Video Generation with Disen-Mix Finetuning](https://arxiv.org/abs/2311.00990) (Nov., 2023)  
  [![Star](https://img.shields.io/github/stars/videodreamer23/videodreamer23.github.io.svg?style=social&label=Star)](https://github.com/videodreamer23/videodreamer23.github.io)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.00990)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://videodreamer23.github.io/)

+ [SEINE: Short-to-Long Video Diffusion Model for Generative Transition and Prediction](https://arxiv.org/abs/2310.20700) (Oct., 2023)  
  [![Star](https://img.shields.io/github/stars/Vchitect/SEINE.svg?style=social&label=Star)](https://github.com/Vchitect/SEINE)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.20700)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://vchitect.github.io/SEINE-project/)

+ [FreeNoise: Tuning-Free Longer Video Diffusion Via Noise Rescheduling](https://arxiv.org/abs/2310.15169) (Oct., 2023)  
  [![Star](https://img.shields.io/github/stars/arthur-qiu/LongerCrafter.svg?style=social&label=Star)](https://github.com/arthur-qiu/LongerCrafter)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.15169)
  [![Website](https://img.shields.io/badge/Website-9cf)](http://haonanqiu.com/projects/FreeNoise.html)

+ [DynamiCrafter: Animating Open-domain Images with Video Diffusion Priors](https://arxiv.org/abs/2310.12190) (Oct., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.12190)
  
+ [LAMP: Learn A Motion Pattern for Few-Shot-Based Video Generation](https://arxiv.org/abs/2310.10769) (Oct., 2023)  
  [![Star](https://img.shields.io/github/stars/RQ-Wu/LAMP.svg?style=social&label=Star)](https://github.com/RQ-Wu/LAMP)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.10769)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://rq-wu.github.io/projects/LAMP/) 

+ [Show-1: Marrying Pixel and Latent Diffusion Models for Text-to-Video Generation](https://arxiv.org/abs/2309.15818) (Sep., 2023)  
  [![Star](https://img.shields.io/github/stars/showlab/Show-1.svg?style=social&label=Star)](https://github.com/showlab/Show-1)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.15818)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://showlab.github.io/Show-1/) 

+ [MotionDirector: Motion Customization of Text-to-Video Diffusion Models](https://arxiv.org/abs/2310.08465) (Sep., 2023)  
  [![Star](https://img.shields.io/github/stars/showlab/MotionDirector.svg?style=social&label=Star)](https://github.com/showlab/MotionDirector)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.08465)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://showlab.github.io/MotionDirector/)

+ [LAVIE: High-Quality Video Generation with Cascaded Latent Diffusion Models](https://arxiv.org/abs/2309.15103) (Sep., 2023)  
  [![Star](https://img.shields.io/github/stars/Vchitect/LaVie.svg?style=social&label=Star)](https://github.com/Vchitect/LaVie)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.15103)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://vchitect.github.io/LaVie-project/) 

+ [Diverse and Aligned Audio-to-Video Generation via Text-to-Video Model Adaptation](https://arxiv.org/abs/2309.16429) (Sep., 2023)  
  [![Star](https://img.shields.io/github/stars/guyyariv/TempoTokens.svg?style=social&label=Star)](https://github.com/guyyariv/TempoTokens)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.16429)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://pages.cs.huji.ac.il/adiyoss-lab/TempoTokens/) 

+ [Free-Bloom: Zero-Shot Text-to-Video Generator with LLM Director and LDM Animator](https://arxiv.org/abs/2309.14494) (Sep., 2023)  
  [![Star](https://img.shields.io/github/stars/SooLab/Free-Bloom.svg?style=social&label=Star)](https://github.com/SooLab/Free-Bloom)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.14494)

+ [Hierarchical Masked 3D Diffusion Model for Video Outpainting](https://arxiv.org/abs/2309.02119) (Sep., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.02119)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://fanfanda.github.io/M3DDM/) 

+ [Reuse and Diffuse: Iterative Denoising for Text-to-Video Generation](https://arxiv.org/abs/2309.03549) (Sep., 2023)  
  [![Star](https://img.shields.io/github/stars/anonymous0x233/ReuseAndDiffuse.svg?style=social&label=Star)](https://github.com/anonymous0x233/ReuseAndDiffuse)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.03549)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://anonymous0x233.github.io/ReuseAndDiffuse/) 

+ [VideoGen: A Reference-Guided Latent Diffusion Approach for High Definition Text-to-Video Generation](https://arxiv.org/abs/2309.00398) (Sep., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.00398)

+ [MagicAvatar: Multimodal Avatar Generation and Animation](https://arxiv.org/abs/2308.14748) (Aug., 2023)  
  [![Star](https://img.shields.io/github/stars/magic-research/magic-avatar.svg?style=social&label=Star)](https://github.com/magic-research/magic-avatar)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.14748)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://magic-avatar.github.io/) 

+ [Empowering Dynamics-aware Text-to-Video Diffusion with Large Language Models](https://arxiv.org/abs/2308.13812) (Aug., 2023)  
  [![Star](https://img.shields.io/github/stars/scofield7419/Dysen.svg?style=social&label=Star)](https://github.com/scofield7419/Dysen)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.13812)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://haofei.vip/Dysen-VDM/) 

+ [SimDA: Simple Diffusion Adapter for Efficient Video Generation](https://arxiv.org/abs/2308.09710) (Aug., 2023)  
  [![Star](https://img.shields.io/github/stars/ChenHsing/SimDA.svg?style=social&label=Star)](https://github.com/ChenHsing/SimDA)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.09710)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://chenhsing.github.io/SimDA/) 

+ [ModelScope Text-to-Video Technical Report](https://arxiv.org/abs/2308.06571) (Aug., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.06571)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://modelscope.cn/models/damo/text-to-video-synthesis/summary) 

+ [Dual-Stream Diffusion Net for Text-to-Video Generation](https://arxiv.org/abs/2308.08316) (Aug., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.08316)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://anonymous.4open.science/r/Private-C3E8) 

+ [DragNUWA: Fine-grained Control in Video Generation by Integrating Text, Image, and Trajectory](https://arxiv.org/abs/2308.08089) (Aug., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.08089)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://www.microsoft.com/en-us/research/project/dragnuwa/) 

+ [InternVid: A Large-scale Video-Text Dataset for Multimodal Understanding and Generation](https://arxiv.org/abs/2307.06942) (Jul., 2023)  
  [![Star](https://img.shields.io/github/stars/OpenGVLab/InternVideo.svg?style=social&label=Star)](https://github.com/OpenGVLab/InternVideo/tree/main/Data/InternVid)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.06942)

+ [Animate-A-Story: Storytelling with Retrieval-Augmented Video Generation](https://arxiv.org/abs/2307.06940) (Jul., 2023)  
  [![Star](https://img.shields.io/github/stars/VideoCrafter/Animate-A-Story.svg?style=social&label=Star)](https://github.com/VideoCrafter/Animate-A-Story)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.06940)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://videocrafter.github.io/Animate-A-Story/) 

+ [AnimateDiff: Animate Your Personalized Text-to-Image Diffusion Models without Specific Tuning](https://arxiv.org/abs/2307.04725) (Jul., 2023)  
  [![Star](https://img.shields.io/github/stars/guoyww/animatediff.svg?style=social&label=Star)](https://github.com/guoyww/animatediff/)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.04725)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://animatediff.github.io/) 

+ [DisCo: Disentangled Control for Referring Human Dance Generation in Real World](https://arxiv.org/abs/2307.000400) (Jul., 2023)  
  [![Star](https://img.shields.io/github/stars/Wangt-CN/DisCo.svg?style=social&label=Star)](https://github.com/Wangt-CN/DisCo)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.00040)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://disco-dance.github.io/) 

+ [VideoComposer: Compositional Video Synthesis with Motion Controllability](https://arxiv.org/abs/2306.02018) (Jun., 2023)  
  [![Star](https://img.shields.io/github/stars/damo-vilab/videocomposer.svg?style=social&label=Star)](https://github.com/damo-vilab/videocomposer)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2306.02018)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://videocomposer.github.io/) 

+ [Probabilistic Adaptation of Text-to-Video Models](https://arxiv.org/abs/2306.01872) (Jun., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2306.01872)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://video-adapter.github.io/video-adapter/) 

+ [Make-Your-Video: Customized Video Generation Using Textual and Structural Guidance](https://arxiv.org/abs/2306.00943) (Jun., 2023)  
  [![Star](https://img.shields.io/github/stars/VideoCrafter/Make-Your-Video.svg?style=social&label=Star)](https://github.com/VideoCrafter/Make-Your-Video)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2306.00943)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://doubiiu.github.io/projects/Make-Your-Video/) 

+ [Gen-L-Video: Multi-Text to Long Video Generation via Temporal Co-Denoising](https://arxiv.org/abs/2305.18264) (May, 2023)  
  [![Star](https://img.shields.io/github/stars/G-U-N/Gen-L-Video.svg?style=social&label=Star)](https://github.com/G-U-N/Gen-L-Video)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.18264)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://g-u-n.github.io/projects/gen-long-video/index.html) 

+ [Control-A-Video: Controllable Text-to-Video Generation with Diffusion Models](https://arxiv.org/abs/2305.13840) (May, 2023)  
  [![Star](https://img.shields.io/github/stars/Weifeng-Chen/control-a-video.svg?style=social&label=Star)](https://github.com/Weifeng-Chen/control-a-video)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.13840)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://controlavideo.github.io/) 

+ [ControlVideo: Training-free Controllable Text-to-Video Generation](https://arxiv.org/abs/2305.13077) (May, 2023)  
  [![Star](https://img.shields.io/github/stars/YBYBZhang/ControlVideo.svg?style=social&label=Star)](https://github.com/YBYBZhang/ControlVideo)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.13077) 

+ [Cinematic Mindscapes: High-quality Video Reconstruction from Brain Activity](https://arxiv.org/abs/2305.11675) (May, 2023)  
  [![Star](https://img.shields.io/github/stars/jqin4749/MindVideo.svg?style=social&label=Star)](https://github.com/jqin4749/MindVideo)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.11675) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://mind-video.com/)

+ [Any-to-Any Generation via Composable Diffusion](https://arxiv.org/abs/2305.11846) (May, 2023)  
  [![Star](https://img.shields.io/github/stars/microsoft/i-Code.svg?style=social&label=Star)](https://github.com/microsoft/i-Code/tree/main/i-Code-V3)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.11846) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://codi-gen.github.io/)

+ [VideoFactory: Swap Attention in Spatiotemporal Diffusions for Text-to-Video Generation](https://arxiv.org/abs/2305.10874) (May, 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.10874) 

+ [Preserve Your Own Correlation: A Noise Prior for Video Diffusion Models](https://arxiv.org/abs/2305.10474) (May, 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.10474) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://research.nvidia.com/labs/dir/pyoco/)

+ [Motion-Conditioned Diffusion Model for Controllable Video Synthesis](https://arxiv.org/abs/2304.14404) (Apr., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.14404) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://tsaishien-chen.github.io/MCDiff/)

+ [LaMD: Latent Motion Diffusion for Video Generation](https://arxiv.org/abs/2304.11603) (Apr., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.11603) 

+ [Align your Latents: High-Resolution Video Synthesis with Latent Diffusion Models](https://arxiv.org/abs/2304.08818) (CVPR 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.08818) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://research.nvidia.com/labs/toronto-ai/VideoLDM/)

+ [Text2Performer: Text-Driven Human Video Generation](https://arxiv.org/abs/2304.08483) (Apr., 2023)  
  [![Star](https://img.shields.io/github/stars/yumingj/Text2Performer.svg?style=social&label=Star)](https://github.com/yumingj/Text2Performer)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.08483) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://yumingj.github.io/projects/Text2Performer)
  
+ [Generative Disco: Text-to-Video Generation for Music Visualization](https://arxiv.org/abs/2304.08551) (Apr., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.08551) 

+ [Latent-Shift: Latent Diffusion with Temporal Shift](https://arxiv.org/abs/2304.08477) (Apr., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.08477) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://latent-shift.github.io/) 
  
+ [DreamPose: Fashion Image-to-Video Synthesis via Stable Diffusion](https://arxiv.org/abs/2304.06025) (Apr., 2023)  
  [![Star](https://img.shields.io/github/stars/johannakarras/DreamPose.svg?style=social&label=Star)](https://github.com/johannakarras/DreamPose)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.06025) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://grail.cs.washington.edu/projects/dreampose/)

+ [Follow Your Pose: Pose-Guided Text-to-Video Generation using Pose-Free Videos](https://arxiv.org/abs/2304.01186) (Apr., 2023)  
  [![Star](https://img.shields.io/github/stars/mayuelala/FollowYourPose.svg?style=social&label=Star)](https://github.com/mayuelala/FollowYourPose)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.01186) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://follow-your-pose.github.io/) 

+ [Physics-Driven Diffusion Models for Impact Sound Synthesis from Videos](https://arxiv.org/abs/2303.16897) (CVPR 2023)  
  [![Star](https://img.shields.io/github/stars/sukun1045/video-physics-sound-diffusion.svg?style=social&label=Star)](https://github.com/sukun1045/video-physics-sound-diffusion) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.16897) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://sukun1045.github.io/video-physics-sound-diffusion/) 

+ [Seer: Language Instructed Video Prediction with Latent Diffusion Models](https://arxiv.org/abs/2303.14897) (Mar., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.14897) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://seervideodiffusion.github.io/) 

+ [Text2video-Zero: Text-to-Image Diffusion Models Are Zero-Shot Video Generators](https://arxiv.org/abs/2303.13439) (Mar., 2023)   
  [![Star](https://img.shields.io/github/stars/Picsart-AI-Research/Text2Video-Zero.svg?style=social&label=Star)](https://github.com/Picsart-AI-Research/Text2Video-Zero) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.13439) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://text2video-zero.github.io/) 
  
+ [Conditional Image-to-Video Generation with Latent Flow Diffusion Models](https://arxiv.org/abs/2303.13744) (CVPR 2023)   
  [![Star](https://img.shields.io/github/stars/nihaomiao/CVPR23_LFDM.svg?style=social&label=Star)](https://github.com/nihaomiao/CVPR23_LFDM) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.13744)

+ [Decomposed Diffusion Models for High-Quality Video Generation](https://arxiv.org/abs/2303.08320) (CVPR 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.08320) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://modelscope.cn/models/damo/text-to-video-synthesis/summary) 

+ [Video Probabilistic Diffusion Models in Projected Latent Space](https://arxiv.org/abs/2302.07685) (CVPR 2023)   
  [![Star](https://img.shields.io/github/stars/sihyun-yu/PVDM.svg?style=social&label=Star)](https://github.com/sihyun-yu/PVDM) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2302.07685) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://sihyun.me/PVDM/) 

+ [Learning 3D Photography Videos via Self-supervised Diffusion on Single Images](https://arxiv.org/abs/2302.10781) (Feb., 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2302.10781)

+ [Structure and Content-Guided Video Synthesis With Diffusion Models](https://arxiv.org/abs/2302.03011) (Feb., 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2302.03011) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://research.runwayml.com/gen2) 

+ [Tune-A-Video: One-Shot Tuning of Image Diffusion Models for Text-to-Video Generation](https://arxiv.org/abs/2212.11565) (ICCV 2023)   
  [![Star](https://img.shields.io/github/stars/showlab/Tune-A-Video?style=social)](https://github.com/showlab/Tune-A-Video) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2212.11565) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://tuneavideo.github.io/) 

+ [Mm-Diffusion: Learning Multi-Modal Diffusion Models for Joint Audio and Video Generation](https://arxiv.org/abs/2212.09478) (CVPR 2023)   
  [![Star](https://img.shields.io/github/stars/researchmm/MM-Diffusion.svg?style=social&label=Star)](https://github.com/researchmm/MM-Diffusion) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2212.09478)

+ [Magvit: Masked Generative Video Transformer](https://arxiv.org/abs/2212.05199) (Dec., 2022)    
  [![Star](https://img.shields.io/github/stars/MAGVIT/magvit.svg?style=social&label=Star)](https://github.com/MAGVIT/magvit) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2212.05199) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://magvit.cs.cmu.edu/) 

+ [VIDM: Video Implicit Diffusion Models](https://arxiv.org/abs/2212.00235) (AAAI 2023)   
  [![Star](https://img.shields.io/github/stars/MKFMIKU/VIDM.svg?style=social&label=Star)](https://github.com/MKFMIKU/VIDM) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2212.00235) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://kfmei.page/vidm/) 

+ [Latent Video Diffusion Models for High-Fidelity Video Generation With Arbitrary Lengths](https://arxiv.org/abs/2211.13221) (Nov., 2022)   
  [![Star](https://img.shields.io/github/stars/YingqingHe/LVDM.svg?style=social&label=Star)](https://github.com/YingqingHe/LVDM) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2211.13221) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://yingqinghe.github.io/LVDM/)

+ [SinFusion: Training Diffusion Models on a Single Image or Video](https://arxiv.org/abs/2211.11743) (Nov., 2022)   
  [![Star](https://img.shields.io/github/stars/YingqingHe/LVDM.svg?style=social&label=Star)](https://github.com/yanivnik/sinfusion-code) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2211.11743) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://yanivnik.github.io/sinfusion/)

+ [MagicVideo: Efficient Video Generation With Latent Diffusion Models](https://arxiv.org/abs/2211.11018) (Nov., 2022)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2211.11018) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://magicvideo.github.io/#)

+ [Imagen Video: High Definition Video Generation With Diffusion Models](https://arxiv.org/abs/2210.02303) (Oct., 2022)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2210.02303) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://imagen.research.google/video/)

+ [Make-A-Video: Text-to-Video Generation without Text-Video Data](https://openreview.net/forum?id=nJfylDvgzlq) (ICLR 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://openreview.net/forum?id=nJfylDvgzlq) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://makeavideo.studio)

+ [Diffusion Models for Video Prediction and Infilling](https://arxiv.org/abs/2206.07696) (TMLR 2022)   
  [![Star](https://img.shields.io/github/stars/Tobi-r9/RaMViD.svg?style=social&label=Star)](https://github.com/Tobi-r9/RaMViD) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2206.07696) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://sites.google.com/view/video-diffusion-prediction)

+ [McVd: Masked Conditional Video Diffusion for Prediction, Generation, and Interpolation](https://arxiv.org/abs/2205.09853) (NeurIPS 2022)   
  [![Star](https://img.shields.io/github/stars/Tobi-r9/RaMViD.svg?style=social&label=Star)](https://github.com/voletiv/mcvd-pytorch)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2205.09853) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://mask-cond-video-diffusion.github.io)

+ [Video Diffusion Models](https://arxiv.org/abs/2204.03458) (Apr., 2022)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2204.03458) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://video-diffusion.github.io/)

+ [Diffusion Probabilistic Modeling for Video Generation](https://arxiv.org/abs/2203.09481) (Mar., 2022)   
  [![Star](https://img.shields.io/github/stars/buggyyang/RVD.svg?style=social&label=Star)](https://github.com/buggyyang/RVD) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2203.09481)


### Video Editing 

+ [Cut-and-Paste: Subject-Driven Video Editing with Attention Control](https://arxiv.org/abs/2311.11697) (Nov., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.11697)

+ [LatentWarp: Consistent Diffusion Latents for Zero-Shot Video-to-Video Translation](https://arxiv.org/abs/2311.00353) (Nov., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.00353) 
  
+ [Fuse Your Latents: Video Editing with Multi-source Latent Diffusion Models](https://arxiv.org/abs/2310.16400) (Oct., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.16400) 

+ [DynVideo-E: Harnessing Dynamic NeRF for Large-Scale Motion- and View-Change Human-Centric Video Editing](https://arxiv.org/abs/2310.10624) (Oct., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.10624) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://showlab.github.io/DynVideo-E/)

+ [Ground-A-Video: Zero-shot Grounded Video Editing using Text-to-image Diffusion Models](https://arxiv.org/abs/2310.01107) (Oct., 2023)  
  [![Star](https://img.shields.io/github/stars/Ground-A-Video/Ground-A-Video.svg?style=social&label=Star)](https://github.com/Ground-A-Video/Ground-A-Video) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.01107) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://ground-a-video.github.io/)

+ [CCEdit: Creative and Controllable Video Editing via Diffusion Models](https://arxiv.org/abs/2309.16496) (Sep., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.16496)

+ [MagicProp: Diffusion-based Video Editing via Motion-aware Appearance Propagation](https://arxiv.org/abs/2309.00908) (Sep., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.00908)

+ [MagicEdit: High-Fidelity and Temporally Coherent Video Editing](https://arxiv.org/abs/2308.14749) (Aug., 2023)  
  [![Star](https://img.shields.io/github/stars/magic-research/magic-edit.svg?style=social&label=Star)](https://github.com/magic-research/magic-edit)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.14749)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://magic-edit.github.io/) 

+ [StableVideo: Text-driven Consistency-aware Diffusion Video Editing](https://arxiv.org/abs/2308.09592) (ICCV 2023)  
  [![Star](https://img.shields.io/github/stars/rese1f/StableVideo.svg?style=social&label=Star)](https://github.com/rese1f/StableVideo)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.09592)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://rese1f.github.io/StableVideo/) 

+ [CoDeF: Content Deformation Fields for Temporally Consistent Video Processing](https://arxiv.org/abs/2308.07926) (Aug., 2023)  
  [![Star](https://img.shields.io/github/stars/qiuyu96/CoDeF.svg?style=social&label=Star)](https://github.com/qiuyu96/CoDeF)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.07926)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://qiuyu96.github.io/CoDeF/) 

+ [TokenFlow: Consistent Diffusion Features for Consistent Video Editing](https://arxiv.org/abs/2307.10373) (Jul., 2023)   
  [![Star](https://img.shields.io/github/stars/omerbt/TokenFlow.svg?style=social&label=Star)](https://github.com/omerbt/TokenFlow) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.10373) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://diffusion-tokenflow.github.io/)

+ [INVE: Interactive Neural Video Editing](https://arxiv.org/abs/2307.07663) (Jul., 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.07663) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://gabriel-huang.github.io/inve/)  

+ [VidEdit: Zero-Shot and Spatially Aware Text-Driven Video Editing](https://arxiv.org/abs//2306.08707) (Jun., 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs//2306.08707) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://videdit.github.io/) 

+ [Rerender A Video: Zero-Shot Text-Guided Video-to-Video Translation](https://arxiv.org/abs/2306.07954) (SIGGRAPH Asia 2023)                                       
  [![Star](https://img.shields.io/github/stars/williamyang1991/Rerender_A_Video.svg?style=social&label=Star)](https://github.com/williamyang1991/Rerender_A_Video) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2306.07954)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://www.mmlab-ntu.com/project/rerender/) 

+ [ControlVideo: Adding Conditional Control for One Shot Text-to-Video Editing](https://arxiv.org/abs/2305.17098) (May, 2023)   
  [![Star](https://img.shields.io/github/stars/thu-ml/controlvideo.svg?style=social&label=Star)](https://github.com/thu-ml/controlvideo) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.17098) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://ml.cs.tsinghua.edu.cn/controlvideo/) 

+ [Make-A-Protagonist: Generic Video Editing with An Ensemble of Experts](https://arxiv.org/abs/2305.08850) (May, 2023)   
  [![Star](https://img.shields.io/github/stars/Make-A-Protagonist/Make-A-Protagonist.svg?style=social&label=Star)](https://github.com/Make-A-Protagonist/Make-A-Protagonist) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.08850) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://make-a-protagonist.github.io/) 

+ [Soundini: Sound-Guided Diffusion for Natural Video Editing](https://arxiv.org/abs/2304.06818) (Apr., 2023)   
  [![Star](https://img.shields.io/github/stars/kuai-lab/soundini-official.svg?style=social&label=Star)](https://github.com/kuai-lab/soundini-official) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.06818) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://kuai-lab.github.io/soundini-gallery/) 

+ [Zero-Shot Video Editing Using Off-the-Shelf Image Diffusion Models](https://arxiv.org/abs/2303.17599) (Mar., 2023)   
  [![Star](https://img.shields.io/github/stars/baaivision/vid2vid-zero.svg?style=social&label=Star)](https://github.com/baaivision/vid2vid-zero) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.17599) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://huggingface.co/spaces/BAAI/vid2vid-zero) 

+ [Edit-A-Video: Single Video Editing with Object-Aware Consistency](https://arxiv.org/abs/2303.17599) (Mar., 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.07945) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://edit-a-video.github.io/) 

+ [FateZero: Fusing Attentions for Zero-shot Text-based Video Editing](https://arxiv.org/abs/2303.09535) (Mar., 2023)   
  [![Star](https://img.shields.io/github/stars/ChenyangQiQi/FateZero.svg?style=social&label=Star)](https://github.com/ChenyangQiQi/FateZero) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.09535) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://fate-zero-edit.github.io/)

+ [Pix2video: Video Editing Using Image Diffusion](https://arxiv.org/abs/2303.12688) (Mar., 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.12688) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://duyguceylan.github.io/pix2video.github.io/) 

+ [Video-P2P: Video Editing with Cross-attention Control](https://arxiv.org/abs/2303.04761) (Mar., 2023)   
  [![Star](https://img.shields.io/github/stars/ShaoTengLiu/Video-P2P.svg?style=social&label=Star)](https://github.com/ShaoTengLiu/Video-P2P) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.04761) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://video-p2p.github.io/)

+ [Dreamix: Video Diffusion Models Are General Video Editors](https://arxiv.org/abs/2302.01329) (Feb., 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2302.01329) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://dreamix-video-editing.github.io/) 

+ [Shape-Aware Text-Driven Layered Video Editing](https://arxiv.org/abs/2301.13173) (Jan., 2023)    
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2301.13173) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://text-video-edit.github.io/)   

+ [Speech Driven Video Editing via an Audio-Conditioned Diffusion Model](https://arxiv.org/abs/2301.04474) (Jan., 2023)   
  [![Star](https://img.shields.io/github/stars/DanBigioi/DiffusionVideoEditing.svg?style=social&label=Star)](https://github.com/DanBigioi/DiffusionVideoEditing) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2301.04474) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://danbigioi.github.io/DiffusionVideoEditing/) 

+ [Diffusion Video Autoencoders: Toward Temporally Consistent Face Video Editing via Disentangled Video Encoding](https://arxiv.org/abs/2212.02802) (CVPR 2023)  
  [![Star](https://img.shields.io/github/stars/man805/Diffusion-Video-Autoencoders.svg?style=social&label=Star)](https://github.com/man805/Diffusion-Video-Autoencoders) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2212.02802) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://diff-video-ae.github.io/) 


### Long-form Video Generation and Completion

+ [MCVD: Masked Conditional Video Diffusion for Prediction, Generation, and Interpolation](https://arxiv.org/abs/2205.09853) (NeurIPS 2022)   
  [![Star](https://img.shields.io/github/stars/voletiv/mcvd-pytorch.svg?style=social&label=Star)](https://github.com/voletiv/mcvd-pytorch) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2205.09853) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://mask-cond-video-diffusion.github.io)

+ [NUWA-XL: Diffusion over Diffusion for eXtremely Long Video Generation](https://arxiv.org/abs/2303.12346) (Mar., 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.12346) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://msra-nuwa.azurewebsites.net/#/)

+ [Flexible Diffusion Modeling of Long Videos](https://arxiv.org/abs/2205.11495) (May, 2022)   
  [![Star](https://img.shields.io/github/stars/plai-group/flexible-video-diffusion-modeling.svg?style=social&label=Star)](https://github.com/plai-group/flexible-video-diffusion-modeling) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2205.11495) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://fdmolv.github.io/)


### Human or Subject Motion 

+ [Avatars Grow Legs: Generating Smooth Human Motion from Sparse Tracking Inputs with Diffusion Model](https://arxiv.org/abs/2304.08577) (CVPR 2023)   
  [![Star](https://img.shields.io/github/stars/facebookresearch/AGRoL.svg?style=social&label=Star)](https://github.com/facebookresearch/AGRoL) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.08577) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://dulucas.github.io/agrol/)

+ [InterGen: Diffusion-based Multi-human Motion Generation under Complex Interactions](https://arxiv.org/abs/2304.05684) (Apr., 2023)   
  [![Star](https://img.shields.io/github/stars/tr3e/InterGen.svg?style=social&label=Star)](https://github.com/tr3e/InterGen) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.05684) 

+ [ReMoDiffuse: Retrieval-Augmented Motion Diffusion Model](https://arxiv.org/abs/2304.01116) (Apr., 2023)   
  [![Star](https://img.shields.io/github/stars/mingyuan-zhang/ReMoDiffuse.svg?style=social&label=Star)](https://github.com/mingyuan-zhang/ReMoDiffuse) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.01116) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://mingyuan-zhang.github.io/projects/ReMoDiffuse.html)

+ [Human Motion Diffusion as a Generative Prior](https://arxiv.org/abs/2303.01418) (Mar., 2023)   
  [![Star](https://img.shields.io/github/stars/priorMDM/priorMDM.svg?style=social&label=Star)](https://github.com/priorMDM/priorMDM) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.01418) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://priormdm.github.io/priorMDM-page/)

+ [Can We Use Diffusion Probabilistic Models for 3d Motion Prediction?](https://arxiv.org/abs/2302.14503) (Feb., 2023)    
  [![Star](https://img.shields.io/github/stars/cotton-ahn/diffusion-motion-prediction.svg?style=social&label=Star)](https://github.com/cotton-ahn/diffusion-motion-prediction) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2302.14503) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://sites.google.com/view/diffusion-motion-prediction)

+ [Single Motion Diffusion](https://arxiv.org/abs/2302.05905) (Feb., 2023)   
  [![Star](https://img.shields.io/github/stars/SinMDM/SinMDM.svg?style=social&label=Star)](https://github.com/SinMDM/SinMDM) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2302.05905) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://sinmdm.github.io/SinMDM-page/)

+ [HumanMAC: Masked Motion Completion for Human Motion Prediction](https://arxiv.org/abs/2302.03665) (Feb., 2023)   
  [![Star](https://img.shields.io/github/stars/LinghaoChan/HumanMAC.svg?style=social&label=Star)](https://github.com/LinghaoChan/HumanMAC) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2302.03665) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://lhchen.top/Human-MAC/)

+ [DiffMotion: Speech-Driven Gesture Synthesis Using Denoising Diffusion Model](https://arxiv.org/abs/2301.10047) (Jan., 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2301.10047) 

+ [Modiff: Action-Conditioned 3d Motion Generation With Denoising Diffusion Probabilistic Models](https://arxiv.org/abs/2301.03949) (Jan., 2023)     
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2301.03949) 

+ [Unifying Human Motion Synthesis and Style Transfer With Denoising Diffusion Probabilistic Models](https://arxiv.org/abs/2212.08526) (GRAPP 2023)     
  [![Star](https://img.shields.io/github/stars/mrzzy2021/styledmotionsynthesis.svg?style=social&label=Star)](https://github.com/mrzzy2021/styledmotionsynthesis) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2212.08526) 

+ [Executing Your Commands via Motion Diffusion in Latent Space](https://arxiv.org/abs/2212.04048) (CVPR 2023)   
  [![Star](https://img.shields.io/github/stars/ChenFengYe/motion-latent-diffusion.svg?style=social&label=Star)](https://github.com/ChenFengYe/motion-latent-diffusion) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2212.04048) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://chenxin.tech/mld/)

+ [Pretrained Diffusion Models for Unified Human Motion Synthesis](https://arxiv.org/abs/2212.02837) (Dec., 2022)    
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2212.02837) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://ofa-sys.github.io/MoFusion/)
  
+ [PhysDiff: Physics-Guided Human Motion Diffusion Model](https://arxiv.org/abs/2212.02500) (Dec., 2022)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2212.02500) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://nvlabs.github.io/PhysDiff/)

+ [BeLFusion: Latent Diffusion for Behavior-Driven Human Motion Prediction](https://arxiv.org/abs/2211.14304) (Dec., 2022)     
  [![Star](https://img.shields.io/github/stars/BarqueroGerman/BeLFusion.svg?style=social&label=Star)](https://github.com/BarqueroGerman/BeLFusion) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2211.14304) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://barquerogerman.github.io/BeLFusion/)
  
+ [Listen, Denoise, Action! Audio-Driven Motion Synthesis With Diffusion Models](https://arxiv.org/abs/2211.09707) (Nov. 2022)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2211.09707) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://www.speech.kth.se/research/listen-denoise-action/)
  
+ [Diffusion Motion: Generate Text-Guided 3d Human Motion by Diffusion Model](https://arxiv.org/abs/2210.12315) (ICASSP 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2210.12315) 
  
+ [Human Joint Kinematics Diffusion-Refinement for Stochastic Motion Prediction](https://arxiv.org/abs/2210.05976) (Oct., 2022)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2210.05976) 

+ [Human Motion Diffusion Model](https://arxiv.org/abs/2209.14916) (ICLR 2023)   
  [![Star](https://img.shields.io/github/stars/GuyTevet/motion-diffusion-model.svg?style=social&label=Star)](https://github.com/GuyTevet/motion-diffusion-model) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2209.14916) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://guytevet.github.io/mdm-page/)

+ [FLAME: Free-form Language-based Motion Synthesis & Editing](https://arxiv.org/abs/2209.00349) (AAAI 2023)   
  [![Star](https://img.shields.io/github/stars/kakaobrain/flame.svg?style=social&label=Star)](https://github.com/kakaobrain/flame) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2209.00349) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://kakaobrain.github.io/flame/)

+ [MotionDiffuse: Text-Driven Human Motion Generation with Diffusion Model](https://arxiv.org/abs/2208.15001) (Aug., 2022)   
  [![Star](https://img.shields.io/github/stars/mingyuan-zhang/MotionDiffuse.svg?style=social&label=Star)](https://github.com/mingyuan-zhang/MotionDiffuse) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2208.15001) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://mingyuan-zhang.github.io/projects/MotionDiffuse.html)

+ [Stochastic Trajectory Prediction via Motion Indeterminacy Diffusion](https://arxiv.org/abs/2203.13777) (CVPR 2022)   
  [![Star](https://img.shields.io/github/stars/gutianpei/MID.svg?style=social&label=Star)](https://github.com/gutianpei/MID) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2203.13777) 


### Video Enhancement and Restoration

+ [LDMVFI: Video Frame Interpolation with Latent Diffusion Models](https://arxiv.org/abs/2303.09508) (Mar., 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.09508)

+ [CaDM: Codec-aware Diffusion Modeling for Neural-enhanced Video Streaming](https://arxiv.org/abs/2211.08428) (Nov., 2022)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2211.08428)


### 3D / NeRF

+ [Text2NeRF: Text-Driven 3D Scene Generation with Neural Radiance Fields](https://arxiv.org/abs/2305.11588) (May, 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.11588)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://eckertzhang.github.io/Text2NeRF.github.io/)

+ [RoomDreamer: Text-Driven 3D Indoor Scene Synthesis with Coherent Geometry and Texture](https://arxiv.org/abs/2305.11337) (May, 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.11337)


+ [NeuralField-LDM: Scene Generation with Hierarchical Latent Diffusion Models](https://arxiv.org/abs/2304.09787) (CVPR 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.09787)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://research.nvidia.com/labs/toronto-ai/NFLDM/)

+ [Single-Stage Diffusion NeRF: A Unified Approach to 3D Generation and Reconstruction](https://arxiv.org/abs/2304.06714) (Apr., 2023)  
  [![Star](https://img.shields.io/github/stars/Lakonik/SSDNeRF.svg?style=social&label=Star)](https://github.com/Lakonik/SSDNeRF) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.06714)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://lakonik.github.io/ssdnerf/)

+ [Instruct-NeRF2NeRF: Editing 3D Scenes with Instructions](https://arxiv.org/abs/2303.12789) (Mar., 2023)  
  [![Star](https://img.shields.io/github/stars/ayaanzhaque/instruct-nerf2nerf.svg?style=social&label=Star)](https://github.com/ayaanzhaque/instruct-nerf2nerf) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.12789)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://instruct-nerf2nerf.github.io/)

+ [DiffusioNeRF: Regularizing Neural Radiance Fields with Denoising Diffusion Models](https://arxiv.org/abs/2302.12231) (Feb., 2023)  
  [![Star](https://img.shields.io/github/stars/nianticlabs/diffusionerf.svg?style=social&label=Star)](https://github.com/nianticlabs/diffusionerf) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2302.12231)

+ [NerfDiff: Single-image View Synthesis with NeRF-guided Distillation from 3D-aware Diffusion](https://arxiv.org/abs/2302.10109) (Feb., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2302.10109)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://jiataogu.me/nerfdiff/)

+ [DiffRF: Rendering-guided 3D Radiance Field Diffusion](https://arxiv.org/abs/2212.01206) (CVPR 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2212.01206)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://sirwyver.github.io/DiffRF/)


### Video Understanding

+ [Exploring Diffusion Models for Unsupervised Video Anomaly Detection](https://arxiv.org/abs/2304.05841) (Apr., 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.05841)

+ [PDPP:Projected Diffusion for Procedure Planning in Instructional Videos](https://arxiv.org/abs/2303.14676) (CVPR 2023)   
  [![Star](https://img.shields.io/github/stars/MCG-NJU/PDPP.svg?style=social&label=Star)](https://github.com/MCG-NJU/PDPP) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.14676)

+ [DiffTAD: Temporal Action Detection with Proposal Denoising Diffusion](https://arxiv.org/abs/2303.14863) (Mar., 2023)     
  [![Star](https://img.shields.io/github/stars/sauradip/DiffusionTAD.svg?style=social&label=Star)](https://github.com/sauradip/DiffusionTAD) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.14863)

+ [DiffusionRet: Generative Text-Video Retrieval with Diffusion Model](https://arxiv.org/abs/2303.09867) (ICCV 2023)   
  [![Star](https://img.shields.io/github/stars/jpthu17/DiffusionRet.svg?style=social&label=Star)](https://github.com/jpthu17/DiffusionRet) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.09867)

+ [Refined Semantic Enhancement Towards Frequency Diffusion for Video Captioning](https://arxiv.org/abs/2211.15076) (Nov., 2022)   
  [![Star](https://img.shields.io/github/stars/lzp870/RSFD.svg?style=social&label=Star)](https://github.com/lzp870/RSFD) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2211.15076)

+ [A Generalist Framework for Panoptic Segmentation of Images and Videos](https://arxiv.org/abs/2210.06366) (Oct., 2022)   
  [![Star](https://img.shields.io/github/stars/google-research/pix2seq.svg?style=social&label=Star)](https://github.com/google-research/pix2seq) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2210.06366)


### Healthcare and Biology

+ [Annealed Score-Based Diffusion Model for Mr Motion Artifact Reduction](https://arxiv.org/abs/2301.03027) (Jan., 2023)  
  [![arxiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2301.03027) 

+ [Feature-Conditioned Cascaded Video Diffusion Models for Precise Echocardiogram Synthesis](https://arxiv.org/abs/2303.12644) (Mar., 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.12644)

+ [Neural Cell Video Synthesis via Optical-Flow Diffusion](https://arxiv.org/abs/2212.03250) (Dec., 2022)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2212.03250)

