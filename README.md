# 3D-Pedestrian-Detection-in-Farmland

Paper: **3D pedestrian detection in farmland by monocular RGB image and infrared sensing**

This repository is the PyTorch implementation for the framework of 3D pedestrian detection in farmland, which includes **D5F**: Dual-Input Depth-guided Dynamic-Depthwise-Dilated Fusion network.  
  
  
## Abstract

The automated driving of agricultural machinery is of great significance for the agricultural production efficiency, yet is still challenging due to significantly varied environmental conditions through day and night. To address operation safety for pedestrians in farmland, this paper proposes a 3D person sensing approach based on monocular RGB and infrared images. Since public available datasets for agricultural 3D pedestrian detection are scarce,  we propose a new dataset,  named as "FieldSafePedestrian", which includes field images in both day and night.  We also elaborate the implemented data augmentations of night images and semi-automatic labeling approach to facilitate the 3D annotation of pedestrians. To fuse heterogeneous images of sensors with non-parallel optical axis, we propose the Dual-Input Depth-guided Dynamic-Depthwise-Dilated Fusion network (D5F), which assists the pixel alignment between infrared and RGB images with estimated depth information and deploys a dynamic filtering to guide the heterogeneous information fusion. Extensive experiments on field images in both daytime and nighttime demonstrate that our proposed method gains a significant improvement on both detection precision and runtime efficiency for 3D pedestrian detection in farmland.  

  
## Framework

![Architecture](./Architecture.png)
  
The framework of 3D pedestrian detection in farmland. Dataset generation and pedestrian detection are included in this work.  The infrared image pixels are aligned with RGB image pixels by the estimated depth map. Concatenated image channels and transferred pseudo point clouds are respectively imported to convolution networks to extract deep semantic features, which are further fused to estimate the 3D cylinder label of each pedestrian in agricultural field.  

  

## Citation

If you find this project useful in your research, please consider citing us.  