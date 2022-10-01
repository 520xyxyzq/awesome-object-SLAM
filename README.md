# Awesome Object SLAM
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of Object SLAM papers and resources

This repo is mainitained by [Ziqi Lu](https://github.com/520xyxyzq) and [Akash Sharma](https://github.com/akashsharma02).

You are very welcome to contribute to this repo. Please feel free to [submit](https://github.com/520xyxyzq/awesome-object-SLAM/pulls) a PR or contact the maintainers.

## Table of Contents

## Papers

[TODO] Is it better to list them in the order of category->year->paper? But still not sure what's the best way to categorize them... (object representation? sensors?) Or maybe there is a smarter way to label papers with different categories (like a paper can be RGB + using Quadrics + ...)? 

[TODO] I think we need a more explicit decision boundary for what can be considered as object SLAM. Object SLAM, loosely speaking, is _the process of building a 3D object-level environment map from local object-centric observations_. But there are some grey areas like multi-object tracking (3D) or object-centric multi-view stereo. Also does semantic mapping count, or we have to jointly optimize camera and object states? I personally don't want this list to be super long. It's going to be hard to maintain...

[NOTE] Format for now: All-caps title, after which we add PDF/Code/Video/ProjPage. In each year, papers are sorted in alphabetic order. For non-opensource papers (like ICRA), I was using non-offical links (like ArXiv).

### 2022

- SO-SLAM: Semantic Object SLAM with Scale Proportional and Symmetrical Texture Constraints. [\[PDF\]](https://arxiv.org/pdf/2109.04884.pdf) [\[Code\]](https://github.com/XunshanMan/SoSLAM)
- Symmetry and Uncertainty-Aware Object SLAM for 6DoF Object Pose Estimation. [\[PDF\]](https://openaccess.thecvf.com/content/CVPR2022/papers/Merrill_Symmetry_and_Uncertainty-Aware_Object_SLAM_for_6DoF_Object_Pose_Estimation_CVPR_2022_paper.pdf) [\[Code\]](https://github.com/rpng/suo_slam)

### 2021

- Compositional and Scalable Object SLAM. [\[PDF\]](https://akashsharma02.github.io/assets/pdf/Sharma21icra.pdf) [\[Code\]](https://github.com/rpl-cmu/object-slam)
- Consensus-Informed Optimization Over Mixtures for Ambiguity-Aware Object SLAM. [\[PDF\]](https://arxiv.org/pdf/2107.09265.pdf) [\[Video\]](https://www.youtube.com/watch?v=506VSt0tq4o&ab_channel=MITMarineRoboticsGroup)
- DSP-SLAM: Object Oriented SLAM with Deep Shape Priors. [\[PDF\]](https://arxiv.org/abs/2108.09481) [\[Code\]](https://github.com/JingwenWang95/DSP-SLAM) [\[Video\]](https://youtu.be/of4ANH24LP4) [\[Project Page\]](https://jingwenwang95.github.io/dsp-slam/)

### 2020

- EAO-SLAM: Monocular Semi-Dense Object SLAM Based on Ensemble Data Association. [\[PDF\]](https://arxiv.org/pdf/2004.12730.pdf) [\[Code\]](https://github.com/yanmin-wu/EAO-SLAM) [\[Video\]](https://www.youtube.com/watch?v=pvwdQoV1KBI&ab_channel=YanminWu) [\[Project Page\]](https://yanmin-wu.github.io/project/eaoslam/)
- Kimera: an Open-Source Library for Real-Time Metric-Semantic Localization and Mapping. [\[PDF\]](https://arxiv.org/pdf/1910.02490.pdf) [\[Code\]](https://github.com/MIT-SPARK/Kimera) [\[Video\]](https://www.youtube.com/watch?v=-5XxXRABXJs&ab_channel=MITSPARKLab)
- NodeSLAM: Neural Object Descriptors for Multi-View Shape Reconstruction. [\[PDF\]](https://arxiv.org/pdf/2004.04485.pdf) [\[Video\]](https://www.youtube.com/watch?v=zPzMtXU-0JE&ab_channel=DysonRoboticsLaboratoryatImperialCollege) [\[Project Page\]](https://edgarsucar.github.io/NodeSLAM/)

### 2019
- CubeSLAM: Monocular 3D Object SLAM. [\[PDF\]](https://arxiv.org/pdf/1806.00557.pdf) [\[Code\]](https://github.com/shichaoy/cube_slam) [\[Video\]](https://www.youtube.com/watch?v=QnVlexXi9_c&ab_channel=ShichaoYang)
- QuadricSLAM: Dual Quadrics from Object Detections as Landmarks in Object-Oriented SLAM. [\[PDF\]](https://natanaso.github.io/rcw-icra18/assets/ref/ICRA-MRP18_paper_14.pdf) [\[Code\]](https://github.com/qcr/quadricslam) [\[Video\]](https://www.youtube.com/watch?v=n-j0DFDFSKU&ab_channel=LachlanNicholson)
- Robust Object-based SLAM for High-Speed Autonomous Navigation. [\[PDF\]](https://groups.csail.mit.edu/rrg/papers/OkLiu19icra.pdf)

[TODO] Before a certain year?
### 2013
- SLAM++: Simultaneous Localisation and Mapping at the Level of Objects. [\[PDF\]](https://www.doc.ic.ac.uk/~ajd/Publications/salas-moreno_etal_cvpr2013.pdf) [\[Video\]](https://www.youtube.com/watch?v=tmrAh1CqCRo&ab_channel=imperialrobotvision)

## Resources



