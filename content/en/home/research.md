---
# An instance of the Experience widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: research

active: true

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 40

title: Research Summary
subtitle:

# Date format for experience
#   Refer to https://wowchemy.com/docs/customization/#date-format
date_format: Jan 2006

# Experiences.
#   Add/remove as many `experience` items below as you like.
#   Required fields are `title`, `company`, and `date_start`.
#   Leave `date_end` empty if it's your current employer.
#   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.


design:
  columns: 1
  
  
  
research_step_names:

  step1: GPS-Independent UAV Localization
  step2: Planet-Scale Digital Twins
  step3: Physics-Based Multimodal Simulation

    
    
    
research_step_papers:
  step1:

    - title: "UAV-GeoLoc: A Large-vocabulary Dataset and Geometry-Transformed Method for UAV Geo-Localization"
      authors_text: "Rouwan Wu, jiacheng Deng, Mingyu Mou, Xingyi He, Maojun Zhang, Yu Liu, **Shen Yan**"
      media_icon:
        type: image
        src: "img/research/teaser_RAL.png"
      journal: "IEEE Robotics and Automation Letters"
      intro: "World-UAV -- a diverse and realistic dataset for UAV-to-satellite geo-localization, UAVPlace -- a transformation-invariant retrieval method that significantly improves performance under extreme viewpoint variations."
      cite_text: |
        

      links:
          - name: Paper
            url: "https://ieeexplore.ieee.org/document/11077664"
        
          - name: Project Page
            url: "https://ringowrw.github.io/GeoLoc-UAV/"
        
          - name: Code
            url: "https://github.com/RingoWRW/GeoLoc-UAV"

    - title: "LoD-Loc v2: Aerial Visual Localization over Low Level-of-Detail City Models using Explicit Silhouette Alignment"
      authors_text: "Juelin Zhu, Shuaibang Peng, Long Wang, Hanlin Tan, Yu Liu, Maojun  Zhang, **Shen  Yan**"
      media_icon:
        type: image
        src: "img/research/teaser_ICCV.png"
      journal: "ICCV 2025"
      intro: "We propose a novel method for aerial visual localization over low Level-of-Detail (LoD) city models. Previous wireframe-alignment-based method LoD-Loc [97] has shown promising localization results leveraging LoD models. However, LoD-Loc mainly relies on high-LoD (LoD3 or LoD2) city models, but the majority of available models and those many countries plan to construct nationwide are low-LoD (LoD1). Consequently, enabling localization on low-LoD city models could unlock drones' potential for global urban localization. To address these issues, we introduce LoD-Loc v2, which employs a coarse-to-fine strategy using explicit silhouette alignment to achieve accurate localization over low-LoD city models in the air. Specifically, given a query image, LoD-Loc v2 first applies a building segmentation network to shape building silhouettes. Then, in the coarse pose selection stage, we construct a pose cost volume by uniformly sampling pose hypotheses around a prior pose to represent the pose probability distribution. Each cost of the volume measures the degree of alignment between the projected and predicted silhouettes. We select the pose with maximum value as the coarse pose. In the fine pose estimation stage, a particle filtering method incorporating a multi-beam tracking approach is used to efficiently explore the hypothesis space and obtain the final pose estimation. To further facilitate research in this field, we release two datasets with LoD1 city models covering 10.7 km, along with real RGB queries and ground-truth pose annotations. Experimental results show that LoD-Loc v2 improves estimation accuracy with high-LoD models and enables localization with low-LoD models for the first time. Moreover, it outperforms state-of-the-art baselines by large margins, even surpassing texture-model-based methods, and broadens the convergence basin to accommodate larger prior errors. The code and dataset will be made available upon publication."
      cite_text: |
        @misc{zhu2025lodlocv2aerialvisual,
              title={LoD-Loc v2: Aerial Visual Localization over Low Level-of-Detail City Models using Explicit Silhouette Alignment}, 
              author={Juelin Zhu and Shuaibang Peng and Long Wang and Hanlin Tan and Yu Liu and Maojun Zhang and Shen Yan},
              year={2025},
              eprint={2507.00659},
              archivePrefix={arXiv},
              primaryClass={cs.CV},
              url={https://arxiv.org/abs/2507.00659}, 
        }

      links:
          - name: Paper
            url: "https://arxiv.org/abs/2507.00659"
        
          - name: Project Page
            url: "https://github.com/VictorZoo/LoD-Loc-v2"
        
          - name: Code
            url: "https://github.com/VictorZoo/LoD-Loc-v2" 
  
    - title: "LoD-Loc: Aerial Visual Localization using LoD 3D Map with Neural Wireframe Alignment"
      authors_text: "Juelin Zhu, Shen Yan, Long Wang, Shengyue Zhang, Yu Liu, **Maojun Zhang**"
      media_icon:
        type: image
        src: "img/research/teaser_NuerIPS.png"
      journal: "NeurIPS 2024"
      intro: "We propose a new method named LoD-Loc for visual localization in the air. Unlike existing localization algorithms, LoD-Loc does not rely on complex 3D representations and can estimate the pose of an Unmanned Aerial Vehicle (UAV) using a Level-of-Detail (LoD) 3D map. LoD-Loc mainly achieves this goal by aligning the wireframe derived from the LoD projected model with that predicted by the neural network. Specifically, given a coarse pose provided by the UAV sensor, LoD-Loc hierarchically builds a cost volume for uniformly sampled pose hypotheses to describe pose probability distribution and select a pose with maximum probability. Each cost within this volume measures the degree of line alignment between projected and predicted wireframes. LoD-Loc also devises a 6-DoF pose optimization algorithm to refine the previous result with a differentiable Gaussian-Newton method. As no public dataset exists for the studied problem, we collect two datasets with map levels of LoD3.0 and LoD2.0, along with real RGB queries and ground-truth pose annotations. We benchmark our method and demonstrate that LoD-Loc achieves excellent performance, even surpassing current state-of-the-art methods that use textured 3D models for localization."
      cite_text: |
        @inproceedings{
          zhu2024lodloc,
          title={LoD-Loc: Aerial Visual Localization using LoD 3D Map with Neural Wireframe Alignment},
          author={Juelin Zhu and Shen Yan and Long Wang and zhang shengYue and Yu Liu and Maojun Zhang},
          booktitle={The Thirty-eighth Annual Conference on Neural Information Processing Systems},
          year={2024},
          url={https://openreview.net/forum?id=PqlKliEXyJ}
          }

      links:
          - name: Paper
            url: "https://arxiv.org/abs/2410.12269"
        
          - name: Project Page
            url: "https://github.com/VictorZoo/LoD-Loc"
        
          - name: Code
            url: "https://github.com/VictorZoo/LoD-Loc"

    - title: "UAVD4L:A Large-Scale Dataset for UAV6-DoF Localization"
      authors_text: "Rouwan Wu, Xiaoya Cheng, Juelin Zhu, Yuxiang Liu, **Maojun Zhang**, Shen Yan"
      media_icon:
        type: image
        src: "img/research/teaser_3DV.png"
      journal: "IEEE 3DV"
      intro: "The first large-scale dataset designed specifically for 6-DoF localization of UAVs in GPS-denied environments."
      cite_text: |
        

      links:
          - name: Paper
            url: "https://arxiv.org/pdf/2401.05971"
        
          - name: Project Page
            url: "https://seekanywhere.github.io/"
        
          - name: Code
            url: "https://github.com/RingoWRW/UAVD4L"

    
  step2:
  
    - title: "Prompting Depth Anything for 4K Resolution Accurate Metric Depth Estimation"
      authors_text: "Yuanhong Yu, Xingyi He, Chen Zhao, Junhao Yu, Jiaqi Yang, Ruizhen Hu Yujun Shen Xing Zhu, Xiaowei Zhou, **Sida Peng**"
      media_icon:
        type: image
        src: "img/research/s2-p1.png"
      journal: "CVPR 2025"
      links:
          - name: Paper
            url: "https://arxiv.org/pdf/2504.07955.pdf"
        
          - name: Project Page
            url: "https://zju3dv.github.io/boxdreamer"
        
          - name: Code
            url: "https://github.com/zju3dv/BoxDreamer"
    
  
    - title: "ETCH: Generalizing Body Fitting to Clothed Humans via Equivariant Tightness"
      authors_text: "Boqian Li, Haiwen Feng, Zeyu Cai, Michael J. Black, **Yuliang Xiu**"
      media_icon:
        type: image
        src: "img/research/s2-p2.png"
      journal: "CVPR 2025"
      links:
          - name: Paper
            url: "https://arxiv.org/pdf/2504.07955.pdf"
        
          - name: Project Page
            url: "https://zju3dv.github.io/boxdreamer"
        
          - name: Code
            url: "https://github.com/zju3dv/BoxDreamer"
    
  step3:
  
    - title: "BoxDreamer: Dreaming Box Corners for Generalizable Object Pose Estimation"
      authors_text: "Yuanhong Yu, Xingyi He, Chen Zhao, Junhao Yu, Jiaqi Yang, Ruizhen Hu Yujun Shen Xing Zhu, Xiaowei Zhou, **Sida Peng**"
      media_icon:
        type: image
        src: "img/research/s3-p1.png"
      journal: "CVPR 2025"
      links:
          - name: Paper
            url: "https://arxiv.org/pdf/2504.07955.pdf"
        
          - name: Project Page
            url: "https://zju3dv.github.io/boxdreamer"
        
          - name: Code
            url: "https://github.com/zju3dv/BoxDreamer"
    
  
    - title: "ETCH: Generalizing Body Fitting to Clothed Humans via Equivariant Tightness"
      authors_text: "Boqian Li, Haiwen Feng, Zeyu Cai, Michael J. Black, **Yuliang Xiu**"
      media_icon:
        type: image
        src: "img/research/s3-p2.png"
      journal: "CVPR 2025"
      links:
          - name: Paper
            url: "https://arxiv.org/pdf/2504.07955.pdf"
        
          - name: Project Page
            url: "https://zju3dv.github.io/boxdreamer"
        
          - name: Code
            url: "https://github.com/zju3dv/BoxDreamer"
    

  
---

Our lab pioneers **3D geospatial intelligence** with a focus on:

**·  GPS-Independent UAV Localization** – Enabling drones to geolocate and navigate using various map representations (e.g., textured model, white model, DOM+DSM and DOM+DEM) in GPS-denied environments.

**·  Planet-Scale Digital Twins** – Generating accurate, photorealistic, semantic, and real-time 3D reconstructions of Earth's surface for intelligently measuring, analysis and decision-making.

**·  Physics-Based Multimodal Simulation** – Developing immersive virtual environments for UAV perception, path planning, and localization training via sensor simulation (RGB, thermal, LiDAR, et.al).

![](img/research/r2.png)
