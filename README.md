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
- [Evaluation Benchmarks and Metrics](#evaluation-benchmarks-and-metrics)
- [Video Generation](#video-generation)
- [Controllable Video Generation](#controllable-video-generation)
- [Long Video / Film Generation](#long-video--film-generation)
- [Video Generation with Physical Prior / 3D](#video-generation-with-physical-prior--3d)
- [Video Editing](#video-editing)
- [Long-form Video Generation and Completion](#long-form-video-generation-and-completion)
- [Human or Subject Motion](#human-or-subject-motion)
- [AI Safety for Video Generation](#AI-Safety-for-Video-Generation)
- [Video Enhancement and Restoration](#video-enhancement-and-restoration)
- [Audio Synthesis for Video](#audio-synthesis-for-video)
- [Human Feedback for Video Generation](#human-feedback-for-video-generation)
- [Policy Learning with Video Generation](#policy-learning-with-video-generation)
- [3D / NeRF](#3d--nerf)
- [World Model](#world-model)
- [Video Understanding](#video-understanding)
- [Healthcare and Biology](#healthcare-and-biology)

### Open-source Toolboxes and Foundation Models 

+ [Open-Sora-Plan](https://github.com/PKU-YuanGroup/Open-Sora-Plan)  
  [![Star](https://img.shields.io/github/stars/PKU-YuanGroup/Open-Sora-Plan.svg?style=social&label=Star)](https://github.com/PKU-YuanGroup/Open-Sora-Plan)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://github.com/PKU-YuanGroup/Open-Sora-Plan/blob/main/docs/Report-v1.0.0.md)

+ [Open-Sora](https://github.com/hpcaitech/Open-Sora)  
  [![Star](https://img.shields.io/github/stars/hpcaitech/Open-Sora.svg?style=social&label=Star)](https://github.com/hpcaitech/Open-Sora)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://github.com/hpcaitech/Open-Sora/blob/main/docs/zh_CN/README.md)

+ [Stable Video Diffusion](https://github.com/Stability-AI/generative-models)  
  [![Star](https://img.shields.io/github/stars/Stability-AI/generative-models.svg?style=social&label=Star)](https://github.com/Stability-AI/generative-models)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://stability.ai/news/stable-video-diffusion-open-ai-video-model) 

+ [Show-1](https://github.com/showlab/Show-1)  
  [![Star](https://img.shields.io/github/stars/showlab/Show-1.svg?style=social&label=Star)](https://github.com/showlab/Show-1)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://showlab.github.io/Show-1/) 

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

### Evaluation Benchmarks and Metrics

+ [ChronoMagic-Bench: A Benchmark for Metamorphic Evaluation of Text-to-Time-lapse Video Generation](https://arxiv.org/abs/2406.18522) (Jun., 2024)  
  [![Star](https://img.shields.io/github/stars/PKU-YuanGroup/ChronoMagic-Bench.svg?style=social&label=Star)](https://github.com/PKU-YuanGroup/ChronoMagic-Bench)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.18522)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://pku-yuangroup.github.io/ChronoMagic-Bench/)

+ [PEEKABOO: Interactive Video Generation via Masked-Diffusion](https://arxiv.org/abs/2312.07509) (CVPR, 2024)  
  [![Star](https://img.shields.io/github/stars/microsoft/Peekaboo.svg?style=social&label=Star)](https://github.com/microsoft/Peekaboo)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.07509)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://jinga-lala.github.io/projects/Peekaboo/)

+ [T2VScore: Towards A Better Metric for Text-to-Video Generation](https://arxiv.org/abs/2401.07781) (Jan., 2024)      
  [![Star](https://img.shields.io/github/stars/showlab/T2VScore.svg?style=social&label=Star)](https://github.com/showlab/T2VScore)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.07781)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://showlab.github.io/T2VScore/) 

+ [VBench: Comprehensive Benchmark Suite for Video Generative Models](https://arxiv.org/abs/2311.17982) (Nov., 2023)      
  [![Star](https://img.shields.io/github/stars/Vchitect/VBench.svg?style=social&label=Star)](https://github.com/Vchitect/VBench?tab=readme-ov-file)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.17982)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://vchitect.github.io/VBench-project/) 

+ [FETV: A Benchmark for Fine-Grained Evaluation of Open-Domain Text-to-Video Generation](https://arxiv.org/abs/2311.01813) (Nov., 2023)      
  [![Star](https://img.shields.io/github/stars/llyx97/FETV.svg?style=social&label=Star)](https://github.com/llyx97/FETV)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.01813)

+ [EvalCrafter: Benchmarking and Evaluating Large Video Generation Models](https://arxiv.org/abs/2310.11440) (Oct., 2023)      
  [![Star](https://img.shields.io/github/stars/EvalCrafter/EvalCrafter.svg?style=social&label=Star)](https://github.com/EvalCrafter/EvalCrafter)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.11440)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://evalcrafter.github.io/) 
  [![Dataset](https://img.shields.io/badge/Dataset-e97451)](https://huggingface.co/datasets/RaphaelLiu/EvalCrafter_T2V_Dataset) 

+ [Evaluation of Text-to-Video Generation Models: A Dynamics Perspective](https://arxiv.org/pdf/2407.01094) (Jul., 2024)      
  [![Star](https://img.shields.io/github/stars/MingXiangL/DEVIL.svg?style=social&label=Star)](https://github.com/MingXiangL/DEVIL)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2407.01094)

+ [VidProM: A Million-scale Real Prompt-Gallery Dataset for Text-to-Video Diffusion Models](https://arxiv.org/abs/2403.06098) (May., 2024)      
  [![Star](https://img.shields.io/github/stars/WangWenhao0716/VidProM.svg?style=social&label=Star)](https://github.com/WangWenhao0716/VidProM)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.06098)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://github.com/WangWenhao0716/VidProM) 
  [![Dataset](https://img.shields.io/badge/Dataset-e97451)](https://vidprom.github.io/) 
  
+ [Panda-70M: Captioning 70M Videos with Multiple Cross-Modality Teachers](https://arxiv.org/abs/2402.19479) (CVPR, 2024)      
  [![Star](https://img.shields.io/github/stars/snap-research/Panda-70M.svg?style=social&label=Star)](https://github.com/snap-research/Panda-70M)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.19479)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://github.com/snap-research/Panda-70M) 
  [![Dataset](https://img.shields.io/badge/Dataset-e97451)](https://snap-research.github.io/Panda-70M/) 

### Video Generation 

+ [VEnhancer: Generative Space-Time Enhancement for Video Generation](https://arxiv.org/abs/2407.07667) (Jul., 2024)      
  [![Star](https://img.shields.io/github/stars/Vchitect/VEnhancer.svg?style=social&label=Star)](https://github.com/Vchitect/VEnhancer)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.07667)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://vchitect.github.io/VEnhancer-project/)

+ [Live2Diff: Live Stream Translation via Uni-directional Attention in Video Diffusion Models](https://arxiv.org/abs/2407.08701) (Jul., 2024)      
  [![Star](https://img.shields.io/github/stars/open-mmlab/Live2Diff.svg?style=social&label=Star)](https://github.com/open-mmlab/Live2Diff)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.08701)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://live2diff.github.io/)

+ [Video Diffusion Alignment via Reward Gradient](https://arxiv.org/abs/2407.08737) (Jul., 2024)      
  [![Star](https://img.shields.io/github/stars/mihirp1998/VADER.svg?style=social&label=Star)](https://github.com/mihirp1998/VADER)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.08737)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://vader-vid.github.io/)

+ [ExVideo: Extending Video Diffusion Models via Parameter-Efficient Post-Tuning](https://arxiv.org/abs/2406.14130) (Jun., 2024)      
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.14130)

+ [MimicMotion: High-Quality Human Motion Video Generation with Confidence-aware Pose Guidance](https://arxiv.org/abs/2406.19680) (Jul., 2024)      
  [![Star](https://img.shields.io/github/stars/Tencent/MimicMotion.svg?style=social&label=Star)](https://github.com/Tencent/MimicMotion)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.19680)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://tencent.github.io/MimicMotion/)

+ [Identifying and Solving Conditional Image Leakage in Image-to-Video Diffusion Model](https://arxiv.org/abs/2406.15735) (Jun., 2024)   
  [![Star](https://img.shields.io/github/stars/thu-ml/cond-image-leakage.svg?style=social&label=Star)](https://github.com/thu-ml/cond-image-leakage/tree/main?tab=readme-ov-file)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.15735)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://cond-image-leak.github.io/)

+ [Video-Infinity: Distributed Long Video Generation](https://arxiv.org/abs/2406.16260) (Jun., 2024)      
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.16260)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://video-infinity.tanzhenxiong.com/)

+ [MotionBooth: Motion-Aware Customized Text-to-Video Generation](https://arxiv.org/abs/2406.17758) (Jun., 2024)      
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.17758)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://jianzongwu.github.io/projects/motionbooth/)

+ [Text-Animator: Controllable Visual Text Video Generation](https://arxiv.org/abs/2406.17777) (Jun., 2024)      
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.17777)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://laulampaul.github.io/text-animator.html)

+ [UniAnimate: Taming Unified Video Diffusion Models for Consistent Human Image Animation](https://arxiv.org/abs/2406.01188) (Jun., 2024)      
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.01188)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://unianimate.github.io/)

+ [T2V-Turbo: Breaking the Quality Bottleneck of Video Consistency Model with Mixed Reward Feedback](https://arxiv.org/abs/2405.18750) (May, 2024)      
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.18750)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://t2v-turbo.github.io/)

+ [Collaborative Video Diffusion: Consistent Multi-video Generation with Camera Control](https://arxiv.org/abs/2405.17414) (May, 2024)      
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.17414)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://collaborativevideodiffusion.github.io/)

+ [Human4DiT: Free-view Human Video Generation with 4D Diffusion Transformer](https://arxiv.org/abs/2405.17405) (May, 2024)      
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.17405)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://human4dit.github.io/)

+ [FIFO-Diffusion: Generating Infinite Videos from Text without Training](https://arxiv.org/abs/2405.11473) (May, 2024)      
  [![Star](https://img.shields.io/github/stars/jjihwan/FIFO-Diffusion_public.svg?style=social&label=Star)](https://github.com/jjihwan/FIFO-Diffusion_public)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.11473)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://jjihwan.github.io/projects/FIFO-Diffusion)

+ [Vidu: a Highly Consistent, Dynamic and Skilled Text-to-Video Generator with Diffusion Models](https://arxiv.org/abs/2405.04233) (May, 2024)      
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.04233)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://www.shengshu-ai.com/vidu)

+ [Lumina-T2X: Transforming Text into Any Modality, Resolution, and Duration via Flow-based Large Diffusion Transformers](https://arxiv.org/abs/2405.05945) (May, 2024)      
  [![Star](https://img.shields.io/github/stars/Alpha-VLLM/Lumina-T2X.svg?style=social&label=Star)](https://github.com/Alpha-VLLM/Lumina-T2X)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.05945)

+ [StoryDiffusion: Consistent Self-Attention for Long-Range Image and Video Generation](https://arxiv.org/abs/2405.01434) (May, 2024)      
  [![Star](https://img.shields.io/github/stars/HVision-NKU/StoryDiffusion.svg?style=social&label=Star)](https://github.com/HVision-NKU/StoryDiffusion)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.01434)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://storydiffusion.github.io/)

+ [TI2V-Zero: Zero-Shot Image Conditioning for Text-to-Video Diffusion Models](https://arxiv.org/abs/2404.16306) (CVPR 2024)      
  [![Star](https://img.shields.io/github/stars/merlresearch/TI2V-Zero.svg?style=social&label=Star)](https://github.com/merlresearch/TI2V-Zero)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.16306)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://merl.com/research/highlights/TI2V-Zero)

+ [ID-Animator: Zero-Shot Identity-Preserving Human Video Generation](https://arxiv.org/abs/2404.15275) (Apr., 2024)  
  [![Star](https://img.shields.io/github/stars/ID-Animator/ID-Animator.svg?style=social&label=Star)](https://github.com/ID-Animator/ID-Animator) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.15275)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://id-animator.github.io/)

+ [AnimateZoo: Zero-shot Video Generation of Cross-Species Animation via Subject Alignment](https://arxiv.org/abs/2404.04946) (Apr., 2024)  
  [![Star](https://img.shields.io/github/stars/JustinXu0/AnimateZoo.svg?style=social&label=Star)](https://github.com/JustinXu0/AnimateZoo) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.04946)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://justinxu0.github.io/AnimateZoo/)

+ [MagicTime: Time-lapse Video Generation Models as Metamorphic Simulators](https://arxiv.org/abs/2404.05014) (Apr., 2024)      
  [![Star](https://img.shields.io/github/stars/PKU-YuanGroup/MagicTime.svg?style=social&label=Star)](https://github.com/PKU-YuanGroup/MagicTime)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.05014)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://pku-yuangroup.github.io/MagicTime/) 
  [![Dataset](https://img.shields.io/badge/Dataset-e97451)](https://drive.google.com/drive/folders/1WsomdkmSp3ql3ImcNsmzFuSQ9Qukuyr8?usp=sharing) 

+ [TRIP: Temporal Residual Learning with Image Noise Prior for Image-to-Video Diffusion Models](https://arxiv.org/abs/2403.17005) (CVPR 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.17005)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://trip-i2v.github.io/TRIP/)

+ [StreamingT2V: Consistent, Dynamic, and Extendable Long Video Generation from Text](https://arxiv.org/abs/2403.14773) (Mar., 2024)  
  [![Star](https://img.shields.io/github/stars/Picsart-AI-Research/StreamingT2V.svg?style=social&label=Star)](https://github.com/Picsart-AI-Research/StreamingT2V)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.14773)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://streamingt2v.github.io/)

+ [Intention-driven Ego-to-Exo Video Generation](https://arxiv.org/abs/2403.09194) (Mar., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.09194)

+ [VideoElevator: Elevating Video Generation Quality with Versatile Text-to-Image Diffusion Models](https://arxiv.org/abs/2403.05438) (Mar., 2024)  
  [![Star](https://img.shields.io/github/stars/YBYBZhang/VideoElevator.svg?style=social&label=Star)](https://github.com/YBYBZhang/VideoElevator)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.05438)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://videoelevator.github.io/)

+ [Snap Video: Scaled Spatiotemporal Transformers for Text-to-Video Synthesis](https://arxiv.org/abs/2402.14797) (Feb., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.14797)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://snap-research.github.io/snapvideo/)

+ [One-Shot Motion Customization of Text-to-Video Diffusion Models](https://arxiv.org/abs/2402.14780) (Feb., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.14780)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://anonymous-314.github.io/)

+ [Magic-Me: Identity-Specific Video Customized Diffusion](https://arxiv.org/abs/2402.09368) (Feb., 2024)  
  [![Star](https://img.shields.io/github/stars/Zhen-Dong/Magic-Me.svg?style=social&label=Star)](https://github.com/Zhen-Dong/Magic-Me)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.09368)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://magic-me-webpage.github.io/)

+ [ConsistI2V: Enhancing Visual Consistency for Image-to-Video Generation](https://arxiv.org/abs/2402.04324) (Feb., 2024)  
  [![Star](https://img.shields.io/github/stars/TIGER-AI-Lab/ConsistI2V.svg?style=social&label=Star)](https://github.com/TIGER-AI-Lab/ConsistI2V)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.04324)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://tiger-ai-lab.github.io/ConsistI2V/)

+ [Direct-a-Video: Customized Video Generation with User-Directed Camera Movement and Object Motion](https://arxiv.org/abs/2402.03162) (Feb., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.03162)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://direct-a-video.github.io/)

+ [Video-LaVIT: Unified Video-Language Pre-training with Decoupled Visual-Motional Tokenization](https://arxiv.org/abs/2402.03161) (Feb., 2024)  
  [![Star](https://img.shields.io/github/stars/jy0205/LaVIT.svg?style=social&label=Star)](https://github.com/jy0205/LaVIT)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.03161)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://video-lavit.github.io/)

+ [Boximator: Generating Rich and Controllable Motions for Video Synthesis](https://arxiv.org/abs/2402.01566) (Feb., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.01566)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://boximator.github.io/)

+ [Lumiere: A Space-Time Diffusion Model for Video Generation](https://arxiv.org/abs/2401.12945) (Jan., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.12945)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://lumiere-video.github.io/)

+ [ActAnywhere: Subject-Aware Video Background Generation](https://arxiv.org/abs/2401.10822) (Jan., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.10822)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://actanywhere.github.io/)

+ [WorldDreamer: Towards General World Models for Video Generation via Predicting Masked Tokens](https://arxiv.org/abs/2401.09985) (Jan., 2024)  
  [![Star](https://img.shields.io/github/stars/JeffWang987/WorldDreamer.svg?style=social&label=Star)](https://github.com/JeffWang987/WorldDreamer)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.09985)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://world-dreamer.github.io/)

+ [CustomVideo: Customizing Text-to-Video Generation with Multiple Subjects](https://arxiv.org/abs/2401.09962) (Jan., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.09962)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://kyfafyd.wang/projects/customvideo/)

+ [UniVG: Towards UNIfied-modal Video Generation](https://arxiv.org/abs/2401.09084) (Jan., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.09084)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://univg-baidu.github.io/)

+ [VideoCrafter2: Overcoming Data Limitations for High-Quality Video Diffusion Models](https://arxiv.org/abs/2401.09047) (Jan., 2024)  
  [![Star](https://img.shields.io/github/stars/AILab-CVC/VideoCrafter.svg?style=social&label=Star)](https://github.com/AILab-CVC/VideoCrafter)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.09047)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://ailab-cvc.github.io/videocrafter2/)

+ [360DVD: Controllable Panorama Video Generation with 360-Degree Video Diffusion Model](https://arxiv.org/abs/2401.06578) (Jan., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.06578)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://akaneqwq.github.io/360DVD/)

+ [RAVEN: Rethinking Adversarial Video Generation with Efficient Tri-plane Networks](https://arxiv.org/abs/2401.06035) (Jan., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.06035)

+ [Latte: Latent Diffusion Transformer for Video Generation](https://arxiv.org/abs/2401.03048) (Jan., 2024)  
  [![Star](https://img.shields.io/github/stars/Vchitect/Latte.svg?style=social&label=Star)](https://github.com/Vchitect/Latte)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.03048)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://maxin-cn.github.io/latte_project/)

+ [MagicVideo-V2: Multi-Stage High-Aesthetic Video Generation](https://arxiv.org/abs/2401.04468) (Jan., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.04468)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://magicvideov2.github.io/)

+ [VideoDrafter: Content-Consistent Multi-Scene Video Generation with LLM](https://arxiv.org/abs/2401.01256) (Jan., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.01256)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://videodrafter.github.io/)

+ [FlashVideo: A Framework for Swift Inference in Text-to-Video Generation](https://arxiv.org/abs/2401.00869) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.00869)

+ [I2V-Adapter: A General Image-to-Video Adapter for Video Diffusion Models](https://arxiv.org/abs/2312.16693) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.16693)

+ [A Recipe for Scaling up Text-to-Video Generation with Text-free Videos](https://arxiv.org/abs/2312.15770) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.15770)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://tf-t2v.github.io/)

+ [PIA: Your Personalized Image Animator via Plug-and-Play Modules in Text-to-Image Models](https://arxiv.org/abs/2312.13964) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/open-mmlab/PIA.svg?style=social&label=Star)](https://github.com/open-mmlab/PIA)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.13964)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://pi-animator.github.io/)

+ [VideoPoet: A Large Language Model for Zero-Shot Video Generation](https://arxiv.org/abs/2312.14125) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.14125)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://sites.research.google/videopoet/)

+ [InstructVideo: Instructing Video Diffusion Models with Human Feedback](https://arxiv.org/abs/2312.12490) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/damo-vilab/i2vgen-xl.svg?style=social&label=Star)](https://github.com/damo-vilab/i2vgen-xl/blob/main/doc/InstructVideo.md)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.12490)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://instructvideo.github.io/)

+ [VideoLCM: Video Latent Consistency Model](https://arxiv.org/abs/2312.09109) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.09109)

+ [PEEKABOO: Interactive Video Generation via Masked-Diffusion](https://arxiv.org/abs/2312.07509) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/microsoft/Peekaboo.svg?style=social&label=Star)](https://github.com/microsoft/Peekaboo)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.07509)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://jinga-lala.github.io/projects/Peekaboo/)

+ [FreeInit: Bridging Initialization Gap in Video Diffusion Models](https://arxiv.org/abs/2312.07537) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/TianxingWu/FreeInit.svg?style=social&label=Star)](https://github.com/TianxingWu/FreeInit)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.07537)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://tianxingwu.github.io/pages/FreeInit/)

+ [Photorealistic Video Generation with Diffusion Models](https://arxiv.org/abs/2312.06662) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.06662)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://walt-video-diffusion.github.io/)

+ [Upscale-A-Video: Temporal-Consistent Diffusion Model for Real-World Video Super-Resolution](https://arxiv.org/abs/2312.06640) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/sczhou/Upscale-A-Video.svg?style=social&label=Star)](https://github.com/sczhou/Upscale-A-Video)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.06640)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://shangchenzhou.com/projects/upscale-a-video/)

+ [DreaMoving: A Human Video Generation Framework based on Diffusion Models](https://arxiv.org/abs/2312.05107) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/dreamoving/dreamoving-project.svg?style=social&label=Star)](https://github.com/dreamoving/dreamoving-project)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.05107)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://dreamoving.github.io/dreamoving/)

+ [MotionCrafter: One-Shot Motion Customization of Diffusion Models](https://arxiv.org/abs/2312.05288) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/zyxElsa/MotionCrafter.svg?style=social&label=Star)](https://github.com/zyxElsa/MotionCrafter)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.05288)

+ [AnimateZero: Video Diffusion Models are Zero-Shot Image Animators](https://arxiv.org/abs/2312.03793) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/vvictoryuki/AnimateZero.svg?style=social&label=Star)](https://github.com/vvictoryuki/AnimateZero)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.03793)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://vvictoryuki.github.io/animatezero.github.io/)

+ [AVID: Any-Length Video Inpainting with Diffusion Model](https://arxiv.org/abs/2312.03816) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/zhang-zx/AVID.svg?style=social&label=Star)](https://github.com/zhang-zx/AVID)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.03816)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://zhang-zx.github.io/AVID/)

+ [MTVG : Multi-text Video Generation with Text-to-Video Models](https://arxiv.org/abs/2312.04086) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.04086)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://kuai-lab.github.io/mtvg-page)

+ [DreamVideo: Composing Your Dream Videos with Customized Subject and Motion](https://arxiv.org/abs/2312.04433) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/damo-vilab/i2vgen-xl.svg?style=social&label=Star)](https://github.com/damo-vilab/i2vgen-xl)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.04433)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://dreamvideo-t2v.github.io/)

+ [Hierarchical Spatio-temporal Decoupling for Text-to-Video Generation](https://arxiv.org/abs/2312.04483) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/damo-vilab/i2vgen-xl.svg?style=social&label=Star)](https://github.com/damo-vilab/i2vgen-xl)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.04483)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://higen-t2v.github.io/)

+ [GenTron: Delving Deep into Diffusion Transformers for Image and Video Generation](https://arxiv.org/abs/2312.04557) (CVPR 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.04557)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://www.shoufachen.com/gentron_website/)

+ [GenDeF: Learning Generative Deformation Field for Video Generation](https://arxiv.org/abs/2312.04561) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/aim-uofa/GenDeF.svg?style=social&label=Star)](https://github.com/aim-uofa/GenDeF)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.04561)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://aim-uofa.github.io/GenDeF/)

+ [F3-Pruning: A Training-Free and Generalized Pruning Strategy towards Faster and Finer Text-to-Video Synthesis](https://arxiv.org/abs/2312.03459) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.03459)

+ [DreamVideo: High-Fidelity Image-to-Video Generation with Image Retention and Text Guidance](https://arxiv.org/abs/2312.03018) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/anonymous0769/DreamVideo.svg?style=social&label=Star)](https://github.com/anonymous0769/DreamVideo)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.03018)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://anonymous0769.github.io/DreamVideo/)

+ [LivePhoto: Real Image Animation with Text-guided Motion Control](https://arxiv.org/abs/2312.02928) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/XavierCHEN34/LivePhoto.svg?style=social&label=Star)](https://github.com/XavierCHEN34/LivePhoto)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.02928)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://xavierchen34.github.io/LivePhoto-Page/)

+ [Fine-grained Controllable Video Generation via Object Appearance and Context](https://arxiv.org/abs/2312.02919) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.02919)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://hhsinping.github.io/factor/)

+ [VideoBooth: Diffusion-based Video Generation with Image Prompts](https://arxiv.org/abs/2312.00777) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/Vchitect/VideoBooth.svg?style=social&label=Star)](https://github.com/Vchitect/VideoBooth)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.00777)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://vchitect.github.io/VideoBooth-project/)

+ [StyleCrafter: Enhancing Stylized Text-to-Video Generation with Style Adapter](https://arxiv.org/abs/2312.00330) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/GongyeLiu/StyleCrafter.svg?style=social&label=Star)](https://github.com/GongyeLiu/StyleCrafter)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.00330)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://gongyeliu.github.io/StyleCrafter.github.io/)

+ [MicroCinema: A Divide-and-Conquer Approach for Text-to-Video Generation](https://arxiv.org/abs/2311.18829) (Nov., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.18829)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://wangyanhui666.github.io/MicroCinema.github.io/)

+ [ART•V: Auto-Regressive Text-to-Video Generation with Diffusion Models](https://arxiv.org/abs/2311.18834) (Nov., 2023)  
  [![Star](https://img.shields.io/github/stars/WarranWeng/ART.V.svg?style=social&label=Star)](https://github.com/WarranWeng/ART.V)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.18834)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://warranweng.github.io/art.v/)

+ [Smooth Video Synthesis with Noise Constraints on Diffusion Models for One-shot Video Tuning](https://arxiv.org/abs/2311.17536) (Nov., 2023)  
  [![Star](https://img.shields.io/github/stars/SPengLiang/SmoothVideo.svg?style=social&label=Star)](https://github.com/SPengLiang/SmoothVideo)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.17536)

+ [VideoAssembler: Identity-Consistent Video Generation with Reference Entities using Diffusion Model](https://arxiv.org/abs/2311.17338) (Nov., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.17338)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://videoassembler.github.io/videoassembler/)

+ [MotionZero:Exploiting Motion Priors for Zero-shot Text-to-Video Generation](https://arxiv.org/abs/2311.16635) (Nov., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.16635)

+ [MagicAnimate: Temporally Consistent Human Image Animation using Diffusion Model](https://arxiv.org/abs/2311.16498) (Nov., 2023)  
  [![Star](https://img.shields.io/github/stars/magic-research/magic-animate.svg?style=social&label=Star)](https://github.com/magic-research/magic-animate)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.16498)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://showlab.github.io/magicanimate)

+ [FlowZero: Zero-Shot Text-to-Video Synthesis with LLM-Driven Dynamic Scene Syntax](https://arxiv.org/abs/2311.15813) (Nov., 2023)  
  [![Star](https://img.shields.io/github/stars/aniki-ly/FlowZero.svg?style=social&label=Star)](https://github.com/aniki-ly/FlowZero)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.15813)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://flowzero-video.github.io/)

+ [Sketch Video Synthesis](https://arxiv.org/abs/2311.15306) (Nov., 2023)  
  [![Star](https://img.shields.io/github/stars/yudianzheng/SketchVideo.svg?style=social&label=Star)](https://github.com/yudianzheng/SketchVideo)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.15306)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://sketchvideo.github.io/)

+ [Stable Video Diffusion: Scaling Latent Video Diffusion Models to Large Datasets](https://arxiv.org/abs/2311.15127) (Nov., 2023)  
  [![Star](https://img.shields.io/github/stars/Stability-AI/generative-models.svg?style=social&label=Star)](https://github.com/Stability-AI/generative-models)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.15127)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://stability.ai/news/stable-video-diffusion-open-ai-video-model)

+ [Decouple Content and Motion for Conditional Image-to-Video Generation](https://arxiv.org/abs/2311.14294) (Nov., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.14294)

+ [FusionFrames: Efficient Architectural Aspects for Text-to-Video Generation Pipeline](https://arxiv.org/abs/2311.13073) (Nov., 2023)  
  [![Star](https://img.shields.io/github/stars/ai-forever/KandinskyVideo.svg?style=social&label=Star)](https://github.com/ai-forever/KandinskyVideo)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.13073)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://ai-forever.github.io/kandinsky-video/)

+ [Fine-Grained Open Domain Image Animation with Motion Guidance](https://arxiv.org/abs/2311.12886) (Nov., 2023)
  [![Star](https://img.shields.io/github/stars/alibaba/animate-anything.svg?style=social&label=Star)](https://github.com/alibaba/animate-anything)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.12886)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://animationai.github.io/AnimateAnything/)

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
  [![Star](https://img.shields.io/github/stars/Doubiiu/DynamiCrafter.svg?style=social&label=Star)](https://github.com/Doubiiu/DynamiCrafter)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.12190)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://doubiiu.github.io/projects/DynamiCrafter/)
  
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

+ [Learn the Force We Can: Enabling Sparse Motion Control in Multi-Object Video Generation](https://arxiv.org/abs/2306.03988) (Jun., 2023)                                       
  [![Star](https://img.shields.io/github/stars/araachie/yoda.svg?style=social&label=Star)](https://github.com/araachie/yoda) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2306.03988)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://araachie.github.io/yoda/) 

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

+ [Efficient Video Prediction via Sparsely Conditioned Flow Matching](https://arxiv.org/abs/2211.14575) (Nov., 2022)   
  [![Star](https://img.shields.io/github/stars/araachie/river.svg?style=social&label=Star)](https://github.com/araachie/river) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2211.14575) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://araachie.github.io/river/)

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

### Controllable Video Generation

+ [VD3D: Taming Large Video Diffusion Transformers for 3D Camera Control](https://arxiv.org/abs/2407.12781) (Jul., 2024)      
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.12781)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://snap-research.github.io/vd3d/)

+ [Still-Moving: Customized Video Generation without Customized Video Data](https://arxiv.org/abs/2407.08674) (Jul., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.08674)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://still-moving.github.io/)

+ [LivePortrait: Efficient Portrait Animation with Stitching and Retargeting Control](https://arxiv.org/abs/2407.03168) (Jul., 2024)  
  [![Star](https://img.shields.io/github/stars/KwaiVGI/LivePortrait.svg?style=social&label=Star)](https://github.com/KwaiVGI/LivePortrait)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.03168)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://github.com/KwaiVGI/LivePortrait)

+ [Image Conductor: Precision Control for Interactive Video Synthesis](https://arxiv.org/pdf/2406.15339) (Jun., 2024)  
  [![Star](https://img.shields.io/github/stars/liyaowei-stu/ImageConductor.svg?style=social&label=Star)](https://github.com/liyaowei-stu/ImageConductor)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2406.15339)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://liyaowei-stu.github.io/project/ImageConductor/)

+ [MimicMotion: High-Quality Human Motion Video Generation with Confidence-aware Pose Guidance](https://arxiv.org/abs/2406.19680) (Jun., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.19680)

+ [FreeTraj: Tuning-Free Trajectory Control in Video Diffusion Models](https://arxiv.org/abs/2406.16863) (Jun., 2024)  
  [![Star](https://img.shields.io/github/stars/arthur-qiu/FreeTraj.svg?style=social&label=Star)](https://github.com/arthur-qiu/FreeTraj)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.16863)
  [![Website](https://img.shields.io/badge/Website-9cf)](http://haonanqiu.com/projects/FreeTraj.html)

+ [MOFA-Video: Controllable Image Animation via Generative Motion Field Adaptions in Frozen Image-to-Video Diffusion Model](https://arxiv.org/abs/2405.20222) (Jun., 2024)      
  [![Star](https://img.shields.io/github/stars/MyNiuuu/MOFA-Video.svg?style=social&label=Star)](https://github.com/MyNiuuu/MOFA-Video)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.20222)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://myniuuu.github.io/MOFA_Video/)

+ [Champ: Controllable and Consistent Human Image Animation with 3D Parametric Guidance](https://arxiv.org/abs/2403.14781) (Mar., 2024)  
  [![Star](https://img.shields.io/github/stars/fudan-generative-vision/champ.svg?style=social&label=Star)](https://github.com/fudan-generative-vision/champ)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.14781)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://fudan-generative-vision.github.io/champ/)

+ [TrailBlazer: Trajectory Control for Diffusion-Based Video Generation](https://arxiv.org/abs/2401.00896) (Jan., 2024)  
  [![Star](https://img.shields.io/github/stars/hohonu-vicml/Trailblazer.svg?style=social&label=Star)](https://github.com/hohonu-vicml/Trailblazer)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.00896)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://hohonu-vicml.github.io/Trailblazer.Page/)

+ [Motion-Zero: Zero-Shot Moving Object Control Framework for Diffusion-Based Video Generation](https://arxiv.org/abs/2401.10150) (Jan., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.10150)

+ [Moonshot: Towards Controllable Video Generation and Editing with Multimodal Conditions](https://arxiv.org/abs/2401.01827) (Jan., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.01827)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://showlab.github.io/Moonshot/)

+ [MotionCtrl: A Unified and Flexible Motion Controller for Video Generation](https://arxiv.org/abs/2312.03641) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/TencentARC/MotionCtrl.svg?style=social&label=Star)](https://github.com/TencentARC/MotionCtrl)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.03641)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://wzhouxiff.github.io/projects/MotionCtrl/)

+ [Animate Anyone: Consistent and Controllable Image-to-Video Synthesis for Character Animation](https://arxiv.org/abs/2311.17117) (Nov., 2023)  
  [![Star](https://img.shields.io/github/stars/HumanAIGC/AnimateAnyone.svg?style=social&label=Star)](https://github.com/HumanAIGC/AnimateAnyone)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.17117)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://humanaigc.github.io/animate-anyone/)

+ [SparseCtrl: Adding Sparse Controls to Text-to-Video Diffusion Models](https://arxiv.org/abs/2311.16933) (Nov., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.16933)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://guoyww.github.io/projects/SparseCtrl/)

+ [Control-A-Video: Controllable Text-to-Video Generation with Diffusion Models](https://arxiv.org/abs/2305.13840) (May, 2023)  
  [![Star](https://img.shields.io/github/stars/Weifeng-Chen/control-a-video.svg?style=social&label=Star)](https://github.com/Weifeng-Chen/control-a-video)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.13840)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://controlavideo.github.io/) 

+ [Motion-Conditioned Diffusion Model for Controllable Video Synthesis](https://arxiv.org/abs/2304.14404) (Apr., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.14404) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://tsaishien-chen.github.io/MCDiff/)

+ [ControlVideo: Training-free Controllable Text-to-Video Generation](https://arxiv.org/abs/2305.13077) (May, 2023)  
  [![Star](https://img.shields.io/github/stars/YBYBZhang/ControlVideo.svg?style=social&label=Star)](https://github.com/YBYBZhang/ControlVideo)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.13077) 
  
+ [DragNUWA: Fine-grained Control in Video Generation by Integrating Text, Image, and Trajectory](https://arxiv.org/abs/2308.08089) (Aug., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.08089)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://www.microsoft.com/en-us/research/project/dragnuwa/) 

+ [DragAnything: Motion Control for Anything using Entity Representation](https://arxiv.org/abs/2403.07420) (Mar., 2024)  
  [![Star](https://img.shields.io/github/stars/showlab/DragAnything.svg?style=social&label=Star)](https://github.com/showlab/DragAnything)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.07420)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://weijiawu.github.io/draganything_page/)

+ [CameraCtrl: Enabling Camera Control for Video Diffusion Models](https://arxiv.org/abs/2404.02101) (Apr., 2024)  
  [![Star](https://img.shields.io/github/stars/hehao13/CameraCtrl.svg?style=social&label=Star)](https://github.com/hehao13/CameraCtrl) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.02101)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://hehao13.github.io/projects-CameraCtrl/)

+ [Training-free Camera Control for Video Generation](https://arxiv.org/pdf/2406.10126) (Jun., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2406.10126)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://lifedecoder.github.io/CamTrol/)

+ [Customizing Motion in Text-to-Video Diffusion Models](https://arxiv.org/abs/2312.04966) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.04966)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://joaanna.github.io/customizing_motion/)

+ [MotionClone: Training-Free Motion Cloning for Controllable Video Generation](https://arxiv.org/abs/2406.05338) (Jun., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.05338)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://bujiazi.github.io/motionclone.github.io/)

### Long Video / Film Generation

+ [AesopAgent: Agent-driven Evolutionary System on Story-to-Video Production](https://arxiv.org/abs/2403.07952) (Jul, 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.07952)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://aesopai.github.io/)

+ [TheaterGen: Character Management with LLM for Consistent Multi-turn Image Generation](https://arxiv.org/abs/2404.18919) (Jul, 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.18919)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://howe140.github.io/theatergen.io/)
  [![Star](https://img.shields.io/github/stars/donahowe/Theatergen.svg?style=social&label=Star)](https://github.com/donahowe/Theatergen)

+ [AutoStudio: Crafting Consistent Subjects in Multi-turn Interactive Image Generation](https://github.com/donahowe/AutoStudio) (Jul, 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.01388)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://github.com/donahowe/AutoStudio)
  [![Star](https://img.shields.io/github/stars/donahowe/AutoStudio.svg?style=social&label=Star)](https://github.com/donahowe/AutoStudio)

+ [DreamStory: Open-Domain Story Visualization by LLM-Guided Multi-Subject Consistent Diffusion](https://arxiv.org/abs/2407.12899) (Jul, 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.12899)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://dream-xyz.github.io/dreamstory)

+ [VideoDirectorGPT: Consistent Multi-scene Video Generation via LLM-Guided Planning](https://arxiv.org/abs/2309.15091) (Jul, 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.15091)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://videodirectorgpt.github.io/)
  [![Star](https://img.shields.io/github/stars/HL-hanlin/VideoDirectorGPT.svg?style=social&label=Star)](https://github.com/HL-hanlin/VideoDirectorGPT)

### Video Generation with Physical Prior / 3D

+ [IDOL: Unified Dual-Modal Latent Diffusion for Human-Centric Joint Video-Depth Generation](https://arxiv.org/abs/2407.10937) (Jul, 2024)  
  [![Star](https://img.shields.io/github/stars/yhZhai/idol.svg?style=social&label=Star)](https://github.com/yhZhai/idol)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.16823)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://arxiv.org/abs/2407.10937)
  
+ [PhysDreamer: Physics-Based Interaction with 3D Objects via Video Generation](https://arxiv.org/abs/2404.13026) (ECCV 2024)  
  [![Star](https://img.shields.io/github/stars/a1600012888/PhysDreamer.svg?style=social&label=Star)](https://github.com/a1600012888/PhysDreamer)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.13026)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://physdreamer.github.io/)

### Video Editing 

+ [Unified Editing of Panorama, 3D Scenes, and Videos Through Disentangled Self-Attention Injection](https://arxiv.org/abs/2405.16823) (May, 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.16823)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://unifyediting.github.io/)

+ [I2VEdit: First-Frame-Guided Video Editing via Image-to-Video Diffusion Models](https://arxiv.org/abs/2405.16537) (May, 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.16537)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://i2vedit.github.io/)

+ [Looking Backward: Streaming Video-to-Video Translation with Feature Banks](https://arxiv.org/abs/2405.15757) (May, 2024)  
  [![Star](https://img.shields.io/github/stars/Jeff-LiangF/streamv2v.svg?style=social&label=Star)](https://github.com/Jeff-LiangF/streamv2v)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.15757)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://jeff-liangf.github.io/projects/streamv2v/)

+ [ReVideo: Remake a Video with Motion and Content Control](https://arxiv.org/abs/2405.13865) (May, 2024)  
  [![Star](https://img.shields.io/github/stars/MC-E/ReVideo.svg?style=social&label=Star)](https://github.com/MC-E/ReVideo)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.13865)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://mc-e.github.io/project/ReVideo/)

+ [Slicedit: Zero-Shot Video Editing With Text-to-Image Diffusion Models Using Spatio-Temporal Slices](https://arxiv.org/abs/2405.12211) (May, 2024)  
  [![Star](https://img.shields.io/github/stars/fallenshock/Slicedit.svg?style=social&label=Star)](https://github.com/fallenshock/Slicedit)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.12211)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://matankleiner.github.io/slicedit/)

+ [ViViD: Video Virtual Try-on using Diffusion Models](https://arxiv.org/abs/2405.11794) (May, 2024)  
  [![Star](https://img.shields.io/github/stars/BecauseImBatman0/ViViD.svg?style=social&label=Star)](https://github.com/BecauseImBatman0/ViViD)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.11794)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://becauseimbatman0.github.io/ViViD)

+ [Edit-Your-Motion: Space-Time Diffusion Decoupling Learning for Video Motion Editing](https://arxiv.org/abs/2405.04496) (May, 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.04496)

+ [GenVideo: One-shot target-image and shape aware video editing using T2I diffusion models](https://arxiv.org/abs/2404.12541) (Apr., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.12541)

+ [EVA: Zero-shot Accurate Attributes and Multi-Object Video Editing](https://arxiv.org/abs/2403.16111) (Mar., 2024)  
  [![Star](https://img.shields.io/github/stars/knightyxp/EVA_Video_Edit.svg?style=social&label=Star)](https://github.com/knightyxp/EVA_Video_Edit)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.16111)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://knightyxp.github.io/EVA/)

+ [Spectral Motion Alignment for Video Motion Transfer using Diffusion Models](https://arxiv.org/abs/2403.15249) (Mar., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.15249)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://geonyeong-park.github.io/spectral-motion-alignment/)

+ [AnyV2V: A Tuning-Free Framework For Any Video-to-Video Editing Tasks](https://arxiv.org/abs/2403.14468) (Mar., 2024)  
  [![Star](https://img.shields.io/github/stars/TIGER-AI-Lab/AnyV2V.svg?style=social&label=Star)](https://github.com/TIGER-AI-Lab/AnyV2V)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.14468)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://tiger-ai-lab.github.io/AnyV2V/)

+ [CoCoCo: Improving Text-Guided Video Inpainting for Better Consistency, Controllability and Compatibility](https://arxiv.org/abs/2403.12035) (Mar., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.12035)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://cococozibojia.github.io/)
  [![Star](https://img.shields.io/github/stars/zibojia/COCOCO.svg?style=social&label=Star)](https://github.com/zibojia/COCOCO)

+ [DreamMotion: Space-Time Self-Similarity Score Distillation for Zero-Shot Video Editing](https://arxiv.org/abs/2403.12002) (Mar., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.12002)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://hyeonho99.github.io/dreammotion/)

+ [Video Editing via Factorized Diffusion Distillation](https://arxiv.org/abs/2403.09334) (Mar., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.09334)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://fdd-video-edit.github.io/)

+ [FastVideoEdit: Leveraging Consistency Models for Efficient Text-to-Video Editing](https://arxiv.org/abs/2403.06269) (Mar., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.06269)

+ [UniEdit: A Unified Tuning-Free Framework for Video Motion and Appearance Editing](https://arxiv.org/abs/2402.13185) (Feb., 2024)  
  [![Star](https://img.shields.io/github/stars/JianhongBai/UniEdit.svg?style=social&label=Star)](https://github.com/JianhongBai/UniEdit)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2402.13185)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://jianhongbai.github.io/UniEdit/)
  
+ [Object-Centric Diffusion for Efficient Video Editing](https://arxiv.org/abs/2401.05735) (Jan., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.05735)

+ [VASE: Object-Centric Shape and Appearance Manipulation of Real Videos](https://arxiv.org/abs/2401.02473) (Jan., 2024)  
  [![Star](https://img.shields.io/github/stars/helia95/VASE.svg?style=social&label=Star)](https://github.com/helia95/VASE)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.02473)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://helia95.github.io/vase-website/)

+ [FlowVid: Taming Imperfect Optical Flows for Consistent Video-to-Video Synthesis](https://arxiv.org/abs/2312.17681) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/Jeff-LiangF/FlowVid.svg?style=social&label=Star)](https://github.com/Jeff-LiangF/FlowVid)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.17681)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://jeff-liangf.github.io/projects/flowvid/)

+ [Fairy: Fast Parallelized Instruction-Guided Video-to-Video Synthesis](https://arxiv.org/abs/2312.13834) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.13834)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://fairy-video2video.github.io/)

+ [RealCraft: Attention Control as A Solution for Zero-shot Long Video Editing](https://arxiv.org/abs/2312.12635) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.12635)

+ [MaskINT: Video Editing via Interpolative Non-autoregressive Masked Transformers](https://arxiv.org/abs/2312.12468) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.12468)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://maskint.github.io/)

+ [VidToMe: Video Token Merging for Zero-Shot Video Editing](https://arxiv.org/abs/2312.10656) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/lixirui142/VidToMe.svg?style=social&label=Star)](https://github.com/lixirui142/VidToMe)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.10656)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://vidtome-diffusion.github.io/)

+ [A Video is Worth 256 Bases: Spatial-Temporal Expectation-Maximization Inversion for Zero-Shot Video Editing](https://arxiv.org/abs/2312.05856) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/STEM-Inv/stem-inv.svg?style=social&label=Star)](https://github.com/STEM-Inv/stem-inv)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.05856)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://stem-inv.github.io/page/)

+ [Neutral Editing Framework for Diffusion-based Video Editing](https://arxiv.org/abs/2312.06708) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.06708)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://neuedit.github.io/)
  
+ [DiffusionAtlas: High-Fidelity Consistent Diffusion Video Editing](https://arxiv.org/abs/2312.03772) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.03772)

+ [RAVE: Randomized Noise Shuffling for Fast and Consistent Video Editing with Diffusion Models](https://arxiv.org/abs/2312.04524) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/rehg-lab/RAVE.svg?style=social&label=Star)](https://github.com/rehg-lab/RAVE)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.04524)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://rave-video.github.io/)

+ [SAVE: Protagonist Diversification with Structure Agnostic Video Editing](https://arxiv.org/abs/2312.02503) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.02503)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://ldynx.github.io/SAVE/)

+ [MagicStick: Controllable Video Editing via Control Handle Transformations](https://arxiv.org/abs/2312.03047) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/mayuelala/MagicStick.svg?style=social&label=Star)](https://github.com/mayuelala/MagicStick)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.03047)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://magic-stick-edit.github.io/)

+ [VideoSwap: Customized Video Subject Swapping with Interactive Semantic Point Correspondence](https://arxiv.org/abs/2312.02087) (CVPR 2024)  
  [![Star](https://img.shields.io/github/stars/showlab/VideoSwap.svg?style=social&label=Star)](https://github.com/showlab/VideoSwap)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.02087)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://videoswap.github.io/)

+ [DragVideo: Interactive Drag-style Video Editing](https://arxiv.org/abs/2312.02216) (Dec., 2023)  
  [![Star](https://img.shields.io/github/stars/RickySkywalker/DragVideo-Official.svg?style=social&label=Star)](https://github.com/RickySkywalker/DragVideo-Official)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.02216)

+ [Drag-A-Video: Non-rigid Video Editing with Point-based Interaction](https://arxiv.org/abs/2312.02936) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.02936)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://drag-a-video.github.io/)

+ [BIVDiff: A Training-Free Framework for General-Purpose Video Synthesis via Bridging Image and Video Diffusion Models](https://arxiv.org/abs/2312.02813) (Dec., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.02813)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://bivdiff.github.io/)

+ [VMC: Video Motion Customization using Temporal Attention Adaption for Text-to-Video Diffusion Models](https://arxiv.org/abs/2312.00845) (CVPR 2024)  
  [![Star](https://img.shields.io/github/stars/HyeonHo99/Video-Motion-Customization.svg?style=social&label=Star)](https://github.com/HyeonHo99/Video-Motion-Customization)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.00845)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://video-motion-customization.github.io)

+ [FLATTEN: optical FLow-guided ATTENtion for consistent text-to-video editing](https://arxiv.org/abs/2310.05922) (ICLR 2024)  
  [![Star](https://img.shields.io/github/stars/yrcong/flatten.svg?style=social&label=Star)](https://github.com/yrcong/flatten)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.05922)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://flatten-video-editing.github.io)

+ [MotionEditor: Editing Video Motion via Content-Aware Diffusion](https://arxiv.org/abs/2311.18830) (Nov., 2023)  
  [![Star](https://img.shields.io/github/stars/Francis-Rings/MotionEditor.svg?style=social&label=Star)](https://github.com/Francis-Rings/MotionEditor)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.18830)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://francis-rings.github.io/MotionEditor/)

+ [Motion-Conditioned Image Animation for Video Editing](https://arxiv.org/abs/2311.18827) (Nov., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.18827) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://facebookresearch.github.io/MoCA/)

+ [Space-Time Diffusion Features for Zero-Shot Text-Driven Motion Transfer](https://arxiv.org/abs/2311.17009) (CVPR 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.17009) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://diffusion-motion-transfer.github.io/)

+ [Cut-and-Paste: Subject-Driven Video Editing with Attention Control](https://arxiv.org/abs/2311.11697) (Nov., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.11697)

+ [LatentWarp: Consistent Diffusion Latents for Zero-Shot Video-to-Video Translation](https://arxiv.org/abs/2311.00353) (Nov., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.00353) 
  
+ [Fuse Your Latents: Video Editing with Multi-source Latent Diffusion Models](https://arxiv.org/abs/2310.16400) (Oct., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.16400) 

+ [DynVideo-E: Harnessing Dynamic NeRF for Large-Scale Motion- and View-Change Human-Centric Video Editing](https://arxiv.org/abs/2310.10624) (Oct., 2023)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.10624) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://showlab.github.io/DynVideo-E/)

+ [Ground-A-Video: Zero-shot Grounded Video Editing using Text-to-image Diffusion Models](https://arxiv.org/abs/2310.01107) (ICLR 2024)  
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

+ [CoDeF: Content Deformation Fields for Temporally Consistent Video Processing](https://arxiv.org/abs/2308.07926) (CVPR 2024)  
  [![Star](https://img.shields.io/github/stars/qiuyu96/CoDeF.svg?style=social&label=Star)](https://github.com/qiuyu96/CoDeF)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.07926)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://qiuyu96.github.io/CoDeF/) 

+ [TokenFlow: Consistent Diffusion Features for Consistent Video Editing](https://arxiv.org/abs/2307.10373) (ICLR 2024)   
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

+ [Streetscapes: Large-scale Consistent Street View Generation Using Autoregressive Video Diffusion](https://arxiv.org/pdf/2407.13759) (Jul., 2024)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2407.13759) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://boyangdeng.com/streetscapes/)
  
  
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

+ [A Comprehensive Survey on Human Video Generation: Challenges, Methods, and Insights](https://arxiv.org/abs/2407.08428) (Jul., 2024)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.08428) 
  
  
+ [OccFusion: Rendering Occluded Humans with Generative Diffusion Priors](https://arxiv.org/pdf/2406.08801) (Jul., 2024)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2407.00316) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://cs.stanford.edu/~xtiange/projects/occfusion/)

+ [EchoMimic: Lifelike Audio-Driven Portrait Animations through Editable Landmark Conditions](https://arxiv.org/abs/2407.08136) (Jul., 2024)   
  [![Star](https://img.shields.io/github/stars/BadToBest/EchoMimic?style=social)](https://github.com/BadToBest/EchoMimic) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2407.08136) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://badtobest.github.io/echomimic.html)
  
+ [Hallo: Hierarchical Audio-Driven Visual Synthesis for Portrait Image Animation](https://arxiv.org/pdf/2406.08801) (Jun., 2024)   
  [![Star](https://img.shields.io/github/stars/fudan-generative-vision/hallo?style=social)](https://github.com/fudan-generative-vision/hallo) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2406.08801) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://fudan-generative-vision.github.io/hallo/#/)

+ [DiffSHEG: A Diffusion-Based Approach for Real-Time Speech-driven Holistic 3D Expression and Gesture Generation](https://arxiv.org/abs/2401.04747) (CVPR 2024)   
  [![Star](https://img.shields.io/github/stars/JeremyCJM/DiffSHEG.svg?style=social&label=Star)](https://github.com/JeremyCJM/DiffSHEG) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.04747) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://jeremycjm.github.io/proj/DiffSHEG/)

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

### AI Safety for Video Generation
+ [What Matters in Detecting AI-Generated Videos like Sora?](https://arxiv.org/abs/2406.19568) (Jun., 2024)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.19568) 
  [![Website](https://img.shields.io/badge/Website-9cf)](https://justin-crchang.github.io/3DCNNDetection.github.io/)


### Video Enhancement and Restoration

+ [Disentangled Motion Modeling for Video Frame Interpolation](https://arxiv.org/abs/2406.17256) (Jun, 2024)   
  [![Star](https://img.shields.io/github/stars/JHLew/MoMo.svg?style=social&label=Star)](https://github.com/JHLew/MoMo)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.17256)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://github.com/JHLew/MoMo)

+ [DiffIR2VR-Zero: Zero-Shot Video Restoration with Diffusion-based Image Restoration Models](https://arxiv.org/abs/2407.01519) (Jul., 2024)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.01519)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://jimmycv07.github.io/DiffIR2VR_web/)

+ [LDMVFI: Video Frame Interpolation with Latent Diffusion Models](https://arxiv.org/abs/2303.09508) (Mar., 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.09508)

+ [CaDM: Codec-aware Diffusion Modeling for Neural-enhanced Video Streaming](https://arxiv.org/abs/2211.08428) (Nov., 2022)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2211.08428)

### Audio Synthesis for Video

+ [Masked Generative Video-to-Audio Transformers with Enhanced Synchronicity](https://arxiv.org/abs/2407.10387) (Jul., 2024)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.10387)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://maskvat.github.io/)

+ [Video-to-Audio Generation with Hidden Alignment](https://arxiv.org/abs/2407.07464) (Jul., 2024)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.07464)
  [![Star](https://img.shields.io/github/stars/ariesssxu/vta-ldm.svg?style=social&label=Star)](https://github.com/ariesssxu/vta-ldm)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://sites.google.com/view/vta-ldm)
      
+ [Read, Watch and Scream! Sound Generation from Text and Video](https://arxiv.org/abs/2407.05551) (Jul., 2024)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.05551)
  [![Star](https://img.shields.io/github/stars/naver-ai/rewas.svg?style=social&label=Star)](https://github.com/naver-ai/rewas)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://naver-ai.github.io/rewas/)

+ [FoleyCrafter: Bring Silent Videos to Life with Lifelike and Synchronized Sounds](https://arxiv.org/abs/2407.01494) (July, 2024)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.01494)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://foleycrafter.github.io/)

+ [Network Bending of Diffusion Models for Audio-Visual Generation](https://arxiv.org/abs/2406.19589) (CVPR, 2024)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.19589)
  [![Star](https://img.shields.io/github/stars/dzluke/DAFX2024.svg?style=social&label=Star)](https://github.com/dzluke/DAFX2024)

### Human Feedback for Video Generation

+ [VIDEOSCORE: Building Automatic Metrics to Simulate Fine-grained Human Feedback for Video Generation](https://arxiv.org/pdf/2406.15252) (July, 2024)   
  [![Star](https://img.shields.io/github/stars/TIGER-AI-Lab/VideoScore.svg?style=social&label=Star)](https://github.com/TIGER-AI-Lab/VideoScore/)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.15252)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://tiger-ai-lab.github.io/VideoScore/)

### Policy Learning with Video Generation

+ [Any-point Trajectory Modeling for Policy Learning](https://arxiv.org/abs/2401.00025) (July, 2024)   
  [![Star](https://img.shields.io/github/stars/Large-Trajectory-Model/ATM.svg?style=social&label=Star)](https://github.com/Large-Trajectory-Model/ATM)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2401.00025)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://xingyu-lin.github.io/atm/)

+ [This&That: Language-Gesture Controlled Video Generation for Robot Planning](https://arxiv.org/abs/2407.05530) (Jun, 2024)   
  [![Star](https://img.shields.io/github/stars/cfeng16/this-and-that.svg?style=social&label=Star)](https://github.com/cfeng16/this-and-that)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.05530)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://cfeng16.github.io/this-and-that/)

+ [Dreamitate: Real-World Visuomotor Policy Learning via Video Generation](https://arxiv.org/abs/2406.16862) (Jun, 2024)   
  [![Star](https://img.shields.io/github/stars/cvlab-columbia/dreamitate.svg?style=social&label=Star)](https://github.com/cvlab-columbia/dreamitate)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.16862)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://dreamitate.cs.columbia.edu/)

### 3D / NeRF

+ [Shape of Motion: 4D Reconstruction from a Single Video](https://arxiv.org/abs/2407.13764) (Jul., 2024)   
  [![Star](https://img.shields.io/github/stars/vye16/shape-of-motion.svg?style=social&label=Star)](https://github.com/vye16/shape-of-motion/)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.13764)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://shape-of-motion.github.io/)

+ [WonderWorld: Interactive 3D Scene Generation from a Single Image](https://arxiv.org/abs/2406.09394) (Jun., 2024)  
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.09394)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://wonderworld-2024.github.io/)

+ [WonderJourney: Going from Anywhere to Everywhere](https://arxiv.org/pdf/2312.03884) (CVPR 2024)  
  [![Star](https://img.shields.io/github/stars/KovenYu/WonderJourney.svg?style=social&label=Star)](https://github.com/KovenYu/WonderJourney)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2312.03884)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://kovenyu.com/wonderjourney/)

+ [MultiDiff: Consistent Novel View Synthesis from a Single Image](https://sirwyver.github.io/MultiDiff/static/assets/MultiDiff.pdf) (CVPR, 2024)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://sirwyver.github.io/MultiDiff/static/assets/MultiDiff.pdf)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://sirwyver.github.io/MultiDiff/)

+ [Vivid-ZOO: Multi-View Video Generation with Diffusion Model](https://arxiv.org/pdf/2406.08659v1) (Jun, 2024)   
  [![Star](https://img.shields.io/github/stars/Lakonik/SSDNeRF.svg?style=social&label=Star)](https://github.com/hi-zhengcheng/vividzoo)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2406.08659v1)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://hi-zhengcheng.github.io/vividzoo/)

+ [Director3D: Real-world Camera Trajectory and 3D Scene Generation from Text](https://arxiv.org/pdf/2406.17601) (June, 2024)   
  [![Star](https://img.shields.io/github/stars/imlixinyang/director3d.svg?style=social&label=Star)](https://github.com/imlixinyang/director3d)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2406.17601)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://imlixinyang.github.io/director3d-page/)
  
+ [YouDream: Generating Anatomically Controllable Consistent Text-to-3D Animals](https://arxiv.org/abs/2406.16273v1) (June, 2024)   
  [![Star](https://img.shields.io/github/stars/YouDream3D/YouDream.svg?style=social&label=Star)](https://github.com/YouDream3D/YouDream/)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.16273v1)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://youdream3d.github.io/)

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


### World Model

+ [Digital Life Project: Autonomous 3D Characters with Social Intelligence](https://arxiv.org/abs/2312.04547) (CVPR 2024)  
  [![Star](https://img.shields.io/github/stars/caizhongang/Digital_Life_Project.svg?style=social&label=Star)](https://github.com/caizhongang/Digital_Life_Project) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2312.04547)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://digital-life-project.com/)

+ [3D-VLA: A 3D Vision-Language-Action Generative World Model](https://arxiv.org/abs/2403.09631) (ICML 2024)  
  [![Star](https://img.shields.io/github/stars/UMass-Foundation-Model/3D-VLA.svg?style=social&label=Star)](https://github.com/UMass-Foundation-Model/3D-VLA) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2403.09631)
  [![Website](https://img.shields.io/badge/Website-9cf)](https://vis-www.cs.umass.edu/3dvla/)



### Video Understanding

+ [Exploring Diffusion Models for Unsupervised Video Anomaly Detection](https://arxiv.org/abs/2304.05841) (Apr., 2023)   
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.05841)

+ [PDPP:Projected Diffusion for Procedure Planning in Instructional Videos](https://arxiv.org/abs/2303.14676) (CVPR 2023)   
  [![Star](https://img.shields.io/github/stars/MCG-NJU/PDPP.svg?style=social&label=Star)](https://github.com/MCG-NJU/PDPP) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.14676)

+ [DiffTAD: Temporal Action Detection with Proposal Denoising Diffusion](https://arxiv.org/abs/2303.14863) (Mar., 2023)     
  [![Star](https://img.shields.io/github/stars/sauradip/DiffusionTAD.svg?style=social&label=Star)](https://github.com/sauradip/DiffusionTAD) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2303.14863)

+ [Diffusion Action Segmentation](https://arxiv.org/abs/2303.17959) (ICCV 2023)   
  [![Star](https://img.shields.io/github/stars/Finspire13/DiffAct.svg?style=social&label=Star)](https://github.com/Finspire13/DiffAct) 
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]([https://arxiv.org/abs/2303.09867](https://arxiv.org/abs/2303.17959))
  [![Website](https://img.shields.io/badge/Website-9cf)](https://daochang.site/DiffAct-Project-Page/)

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

