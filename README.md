# Awesome Object SLAM [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of Object SLAM papers and resources, inspired by [awesome-implicit-representations](https://github.com/vsitzmann/awesome-implicit-representations).

## Disclaimer

This list *does not aim to be exhaustive*. In this list, we consider papers that **jointly** optimize robot (camera) and object states, where object states typically include object poses and object shape parameters.

For more general SLAM papers, please refer to [awesome-visual-SLAM](https://github.com/tzutalin/awesome-visual-slam) and [Awesome-SLAM](https://github.com/SilenceOverflow/Awesome-SLAM).

This repo is mainitained by [Ziqi Lu](https://github.com/520xyxyzq) and [Akash Sharma](https://github.com/akashsharma02). You are very welcome to contribute to this repo. If you spot anything wrong or missing, please feel free to [submit a pull request](https://github.com/520xyxyzq/awesome-object-SLAM/pulls) or contact the maintainers.

## Table of Contents

- [What is Object SLAM](#what-is-object-slam?)
- [Papers](#papers)
  - [Parametric Object Representation](#parametric-object-representation-cubesquadrics6dof-poseetc)
  - [Field Object Representation](#field-object-representation-neural-fieldsdense-gridsetc)
  - [Inference Methods for Object SLAM](#inference-methods-for-object-slam)
  - [Reviews](#reviews)
- [Resources](#resources)
  - [Datasets](#datasets)


## What is Object SLAM?

Object SLAM, loosely speaking tackles the problem of Simultaneous Localisation and Mapping (SLAM) by building a _3D object-level global environment map from local observations_. To build such a map of the environment, object detection, pose estimation and instance segmentation networks are typically used as virtual sensors in a sensor fusion framework. Representing the 3D map with objects is interesting as it is easy to ascribe semantics to the landmarks to perform higher-level tasks such as object manipulation, motion and task planning, etc. It compresses the map by focusing compute and memory for meaningful regions, and map abstraction is also useful for other tasks such as distributed map building.


## Papers

### Parametric Object Representation (Cubes/Quadrics/6DoF Pose/etc.)

- #### 2023

  - An Object SLAM Framework for Association, Mapping, and High-Level Tasks. [\[PDF\]](https://arxiv.org/pdf/2305.07299.pdf)
  - BundleSDF: Neural 6-DoF Tracking and 3D Reconstruction of Unknown Objects. [\[PDF\]](https://arxiv.org/abs/2303.14158) [\[Code\]](https://github.com/NVlabs/BundleSDF) [\[Video\]](https://www.youtube.com/watch?v=5PymzKbKv8w)
  - Object-based SLAM utilizing unambiguous pose parameters considering general symmetry types. [\[PDF\]](https://arxiv.org/pdf/2303.07872.pdf) [\[Video\]](https://www.youtube.com/watch?v=aVc4x3hsVo4)
  - ObVi-SLAM: Long-Term Object-Visual SLAM. [\[PDF\]](https://arxiv.org/pdf/2309.15268.pdf) [\[Code\]](https://github.com/ut-amrl/ObVi-SLAM) [\[Video\]](https://youtu.be/quJOgnEdaZ0)
  - UniQuadric: A SLAM Backend for Unknown Rigid Object 3D Tracking and Light-Weight Modeling. [\[PDF\]](https://arxiv.org/pdf/2309.17036.pdf)

- #### 2022

  - LayoutSLAM: Object Layout based Simultaneous Localization and Mapping for Reducing Object Map Distortion. [\[PDF\]](https://ieeexplore.ieee.org/abstract/document/9981492)
  - OA-SLAM: Leveraging Objects for Camera Relocalization in Visual SLAM. [\[PDF\]](https://arxiv.org/pdf/2209.08338.pdf) [\[Code\]](https://gitlab.inria.fr/tangram/oa-slam) [\[Video1\]](https://www.youtube.com/watch?v=L1HEL4kLJ3g) [\[Video2\]](https://www.youtube.com/watch?v=50zXF7Z7FLo)
  - SO-SLAM: Semantic Object SLAM with Scale Proportional and Symmetrical Texture Constraints. [\[PDF\]](https://arxiv.org/pdf/2109.04884.pdf) [\[Code\]](https://github.com/XunshanMan/SoSLAM)
  - SQ-SLAM: Monocular Semantic SLAM Based on Superquadric Object Representation. [\[PDF\]](https://arxiv.org/pdf/2209.10817.pdf) [\[Code\]](https://github.com/XiaoHan-Git/SQ-SLAM)
  - Symmetry and Uncertainty-Aware Object SLAM for 6DoF Object Pose Estimation. [\[PDF\]](https://openaccess.thecvf.com/content/CVPR2022/papers/Merrill_Symmetry_and_Uncertainty-Aware_Object_SLAM_for_6DoF_Object_Pose_Estimation_CVPR_2022_paper.pdf) [\[Code\]](https://github.com/rpng/suo_slam)


- #### 2021

  - Accurate and Robust Object-oriented SLAM with 3D Quadric Landmark Construction in Outdoor Environment. [\[PDF\]](https://arxiv.org/pdf/2110.08977.pdf) [\[Video\]](https://www.youtube.com/watch?v=t1KQ8FhO0wo&ab_channel=SLAMer)
  - A Multi-Hypothesis Approach to Pose Ambiguity in Object-Based SLAM. [\[PDF\]](https://arxiv.org/pdf/2108.01225.pdf) [\[Video\]](https://www.youtube.com/watch?v=O3wzdGToh-8&ab_channel=MITMarineRoboticsGroup)
  - BundleTrack: 6D Pose Tracking for Novel Objects without Instance or Category-Level 3D Models. [\[PDF\]](https://arxiv.org/pdf/2108.00516.pdf) [\[Code\]](https://github.com/wenbowen123/BundleTrack) [\[Video\]](https://www.youtube.com/watch?v=0UorLR0ADd4)
  - DynaSLAM II: Tightly-Coupled Multi-Object Tracking and SLAM. [\[PDF\]](https://arxiv.org/pdf/2010.07820.pdf)
  - Object-Augmented RGB-D SLAM for Wide-Disparity Relocalisation. [\[PDF\]](https://arxiv.org/pdf/2108.02522) [\[Code\]](https://github.com/YuhangMing/Object-Guided-Relocalisation) [\[Video\]](https://www.youtube.com/watch?v=H3i9Q4JvX2o)

- #### 2020

  - Dynamic SLAM: The Need for Speed. [\[PDF\]](https://arxiv.org/pdf/2002.08584.pdf)
  - EAO-SLAM: Monocular Semi-Dense Object SLAM Based on Ensemble Data Association. [\[PDF\]](https://arxiv.org/pdf/2004.12730.pdf) [\[Code\]](https://github.com/yanmin-wu/EAO-SLAM) [\[Project Page\]](https://yanmin-wu.github.io/project/eaoslam/)
  - OrcVIO: Object Residual Constrained Visual-Inertial Odometry.  [\[PDF\]](https://arxiv.org/pdf/2007.15107.pdf) [\[Code\]](https://github.com/shanmo/OrcVIO-Stereo-Mapping) [\[Project Page\]](https://moshan.cf/orcvio_githubpage/)
  - VDO-SLAM: A Visual Dynamic Object-Aware SLAM System. [\[PDF\]](https://arxiv.org/pdf/2005.11052.pdf) [\[Code\]](https://github.com/halajun/VDO_SLAM) [\[Video\]](https://drive.google.com/file/d/1PbL4KiJ3sUhxyJSQPZmRP6mgi9dIC0iu/view)

- #### 2019

  - CubeSLAM: Monocular 3D Object SLAM. [\[PDF\]](https://arxiv.org/pdf/1806.00557.pdf) [\[Code\]](https://github.com/shichaoy/cube_slam) [\[Video\]](https://www.youtube.com/watch?v=QnVlexXi9_c&ab_channel=ShichaoYang)
  - Monocular Object and Plane SLAM in Structured Environments. [\[PDF\]](https://arxiv.org/pdf/1809.03415.pdf) [\[Video\]](https://www.youtube.com/watch?v=jzBMsKCm0uk&ab_channel=ShichaoYang)
  - QuadricSLAM: Dual Quadrics from Object Detections as Landmarks in Object-Oriented SLAM. [\[PDF\]](https://natanaso.github.io/rcw-icra18/assets/ref/ICRA-MRP18_paper_14.pdf) [\[Code\]](https://github.com/qcr/quadricslam) [\[Video\]](https://www.youtube.com/watch?v=n-j0DFDFSKU&ab_channel=LachlanNicholson)
  - Real-Time Monocular Object-Model Aware Sparse SLAM. [\[PDF\]](https://ieeexplore.ieee.org/document/8793728) [\[Video\]](https://www.youtube.com/watch?v=UMWXd4sHONw&ab_channel=MehdiHosseinzadeh)
  - Robust Object-based SLAM for High-Speed Autonomous Navigation. [\[PDF\]](https://groups.csail.mit.edu/rrg/papers/OkLiu19icra.pdf)

- #### 2018

  - Structure Aware SLAM using Quadrics and Planes. [\[PDF\]](https://arxiv.org/pdf/1804.09111.pdf) [\[Video\]](https://www.youtube.com/watch?v=dR-rB9keF8M&ab_channel=MehdiHosseinzadeh)

- #### 2016

  - Real-Time Monocular Object SLAM. [\[PDF\]](https://arxiv.org/pdf/1504.02398.pdf) [\[Video\]](https://www.youtube.com/watch?v=wjCK4OTRRO0&ab_channel=dorian3d)

- #### 2013

  - SLAM++: Simultaneous Localisation and Mapping at the Level of Objects. [\[PDF\]](https://www.doc.ic.ac.uk/~ajd/Publications/salas-moreno_etal_cvpr2013.pdf) [\[Video\]](https://www.youtube.com/watch?v=tmrAh1CqCRo&ab_channel=imperialrobotvision)

- #### 2011

  - Semantic Structure From Motion with Object and Point Interactions. [\[PDF\]](https://cvgl.stanford.edu/papers/bao_CORP2011.pdf)
  - Towards Semantic SLAM using a Monocular Camera. [\[PDF\]](http://doriangalvez.com/papers/CiveraIROS11.pdf) [\[Video1\]](https://www.youtube.com/watch?v=_rF2eOOEzEw&ab_channel=dorian3d) [\[Video2\]](https://www.youtube.com/watch?v=1a-GvSQETJ8&ab_channel=dorian3d)


- #### 2008

  - Object-based Visual SLAM: How Object Identity Informs Geometry. [\[PDF\]](https://dellaert.github.io/files/Selvatici08wvc.pdf)

### Field Object Representation (Neural Fields/Dense Grids/etc.)

- #### 2023

  - NeuSE: Neural SE(3)-Equivariant Embedding for Consistent Spatial Understanding with Objects. [\[PDF\]](https://arxiv.org/abs/2303.07308) [\[Project Page\]](https://neuse-slam.github.io/neuse/)
  - RO-MAP: Real-Time Multi-Object Mapping with Neural Radiance Fields. [\[PDF\]](https://arxiv.org/pdf/2304.05735.pdf) [\[Code\]](https://github.com/XiaoHan-Git/RO-MAP) [\[Video\]](https://www.youtube.com/watch?v=sFrLXPw40wU)
  - vMAP: Vectorised Object Mapping for Neural Field SLAM. [\[PDF\]](https://arxiv.org/pdf/2302.01838.pdf) [\[Code\]](https://github.com/kxhit/vMAP) [\[Project Page\]](https://kxhit.github.io/vMAP) [\[Video\]](https://kxhit.github.io/media/vMAP/vmap_raw.mp4)

- #### 2022

  - Learning to Complete Object Shapes for Object-level Mapping in Dynamic Scenes. [\[PDF\]](https://arxiv.org/pdf/2208.05067.pdf) [\[Project Page\]](https://mlr.in.tum.de/research/projects/cosom)

- #### 2021

  - Compositional and Scalable Object SLAM. [\[PDF\]](https://akashsharma02.github.io/assets/pdf/Sharma21icra.pdf) [\[Code\]](https://github.com/rpl-cmu/object-slam)
  - DSP-SLAM: Object Oriented SLAM with Deep Shape Priors. [\[PDF\]](https://arxiv.org/abs/2108.09481) [\[Code\]](https://github.com/JingwenWang95/DSP-SLAM) [\[Project Page\]](https://jingwenwang95.github.io/dsp-slam/)

- #### 2020

  - NodeSLAM: Neural Object Descriptors for Multi-View Shape Reconstruction. [\[PDF\]](https://arxiv.org/pdf/2004.04485.pdf) [\[Project Page\]](https://edgarsucar.github.io/NodeSLAM/)

- #### 2019

  - Deep-SLAM++: Object-Level RGBD SLAM Based on Class-Specific Deep Shape Priors. [\[PDF\]](https://arxiv.org/pdf/1907.09691.pdf)
  - MID-Fusion: Octree-based Object-Level Multi-Instance Dynamic SLAM. [\[PDF\]](https://arxiv.org/pdf/1812.07976.pdf) [\[Video\]](https://www.youtube.com/watch?v=gturboNl9gg)

- #### 2018

  - Fusion++: Volumetric Object-Level SLAM. [\[PDF\]](https://arxiv.org/pdf/1808.08378.pdf) [\[Video\]](https://www.youtube.com/watch?v=2luKNC03x4k)
  - MaskFusion: Real-Time Recognition, Tracking and Reconstruction of Multiple Moving Objects. [\[PDF\]](https://arxiv.org/pdf/1804.09194.pdf) [\[Code\]](https://github.com/martinruenz/maskfusion) [\[Project Page\]](http://visual.cs.ucl.ac.uk/pubs/maskfusion/index.html)

- #### 2017

  - Co-Fusion: : Real-time Segmentation, Tracking and Fusion of Multiple Objects. [\[PDF\]](http://visual.cs.ucl.ac.uk/pubs/cofusion/icra2017_co-fusion_web.pdf) [\[Code\]](https://github.com/martinruenz/co-fusion) [\[Project Page\]](http://visual.cs.ucl.ac.uk/pubs/cofusion/index.html)

### Inference Methods for Object SLAM

- #### 2022

  - Discrete-Continuous Smoothing and Mapping. [\[PDF\]](https://arxiv.org/abs/2204.11936) [\[Code\]](https://github.com/MarineRoboticsGroup/dcsam) [\[Video\]](https://www.youtube.com/watch?v=mUHOZRq2Cik&ab_channel=MITMarineRoboticsGroup)

- #### 2021

  - Consensus-Informed Optimization Over Mixtures for Ambiguity-Aware Object SLAM. [\[PDF\]](https://arxiv.org/pdf/2107.09265.pdf) [\[Video\]](https://www.youtube.com/watch?v=506VSt0tq4o&ab_channel=MITMarineRoboticsGroup)

- #### 2020

  - Probabilistic Data Association via Mixture Models for Robust Semantic SLAM. [\[PDF\]](https://arxiv.org/pdf/1909.11213.pdf) [\[Video\]](https://www.youtube.com/watch?v=Eq_w8zOXCF4&ab_channel=MITMarineRoboticsGroup)

- #### 2019

  - EM-Fusion: Dynamic Object-Level SLAM with Probabilistic Data Association. [\[PDF\]](http://openaccess.thecvf.com/content_ICCV_2019/html/Strecke_EM-Fusion_Dynamic_Object-Level_SLAM_With_Probabilistic_Data_Association_ICCV_2019_paper.html) [\[Code\]](https://github.com/EmbodiedVision/emfusion) [\[Project Page\]](https://emfusion.is.tue.mpg.de/)
  - Multimodal Semantic SLAM with Probabilistic Data Association. [\[PDF\]](https://dspace.mit.edu/bitstream/handle/1721.1/137995/doherty_icra2019_revised.pdf?sequence=2&isAllowed=y) [\[Video\]](https://www.youtube.com/watch?v=9hEonD8KDrs&ab_channel=MITMarineRoboticsGroup)

- #### 2018

  - A Unifying View of Geometry, Semantics, and Data Association in SLAM. [\[PDF\]](https://existentialrobotics.org/ref/Atanasov_SemanticSLAM_IJCAI18.pdf) [\[Video\]](https://existentialrobotics.org/vid/Bowman_SemanticSLAM_ICRA17.mp4#t=145)


- #### 2017

  - Probabilistic Data Association for Semantic SLAM. [\[PDF\]](https://www.cis.upenn.edu/~kostas/mypub.dir/bowman17icra.pdf)

- #### 2016

  - SLAM with Objects using a Nonparametric Pose Graph. [\[PDF\]](https://arxiv.org/abs/1704.05959) [\[Code\]](https://github.com/mubeipeng/objectSLAM) [\[Video\]](https://www.youtube.com/watch?v=YANUWdVLJD4&ab_channel=AerospaceControlsLab)


### Reviews

- #### 2021

  - Advances in Inference and Representation for Simultaneous Localization and Mapping. [\[PDF\]](https://arxiv.org/abs/2103.05041)

- #### 2020

  - Semantics for Robotic Mapping, Perception and Interaction: A Survey. [\[PDF\]](https://arxiv.org/abs/2101.00443)

----------------------

## Resources

### Datasets

- [ApolloScape](http://apolloscape.auto/)
- [Cityscapes](https://www.cityscapes-dataset.com/)
- [ICL-NUIM](https://www.doc.ic.ac.uk/~ahanda/VaFRIC/iclnuim.html)
- [KITTI](https://www.cvlibs.net/datasets/kitti/index.php)
- [Microsoft-RGBD](https://www.microsoft.com/en-us/research/project/rgb-d-dataset-7-scenes/)
- [NYU Depth v2](https://cs.nyu.edu/~silberman/datasets/nyu_depth_v2.html)
- [Redwood-OS](http://redwood-data.org/3dscan/)
- [RGBD Scenes v1](https://rgbd-dataset.cs.washington.edu/)
- [RGBD Scenes v2](https://rgbd-dataset.cs.washington.edu/dataset/rgbd-scenes-v2/)
- [ScanNet](http://www.scan-net.org/)
- [TUM](https://vision.in.tum.de/data/datasets/rgbd-dataset/download)
- [YCB-Video](https://rse-lab.cs.washington.edu/projects/posecnn/)

