### 意见性分享


***
### 课程和报告分享


***
### 成果推荐及讨论
- ##### ResNet strikes back: An improved training procedure in timm 
[Ross Wightman](https://twitter.com/wightmanr)

pdf: [https://arxiv.org/pdf/2110.00476.pdf…](https://t.co/PDtD3ViJ0W?amp=1) 

abs: [https://arxiv.org/abs/2110.00476](https://t.co/YQe70YBhZn?amp=1) 

with more demanding training setting, a vanilla ResNet-50 reaches 80.4% top-1 accuracy at resolution 224×224 on ImageNet-val without extra data or distillation

<div align=center><img src="https://pbs.twimg.com/media/FA0ZoT6WEAQSp9s?format=jpg&name=medium" alt="Cover" width="75%"/></div>

- [Leo Boytsov](https://twitter.com/srchvrs):This seems to be a 4 pt increase from their previous result, but why not to explore what's possible with extra data & distillation? Could it be that resnet-50 capacity isn't big enough?
- [Hervé Jegou](https://twitter.com/hjegou):I would expect distillation to improve the results as well.  But in this ResNet50 paper, we wanted to establish a baseline that couldn't be ignored.  (In DeiT, many subsequent papers did not report our performance with distillation because the considered it a different setting).


reference:https://twitter.com/ak92501/status/1444839293390934021

- ##### Neural implicit humans

  [Michael Black](https://twitter.com/Michael_J_Black)
  
  Neural implicit humans are coming. The key: define a forward skinning deformation field in a pose-independent space. SNARF learns this without direct supervision. At #ICCV2021. Code online.
  
  Video: https://ait.ethz.ch/projects/2021/snarf/downloads/sample2.mp4
  
  - **Gerard Pons-Moll:** Congrats! nice generalization! We also have a neural implicit human paper at ICCV (Neural-GIF). 

  reference: https://twitter.com/Michael_J_Black/status/1444904457007992834?s=20
  
- ##### Indoor Inverse Rendering

  [Zian Wang](https://twitter.com/zianwang97)
  
  Excited to share our #ICCV2021 paper “Learning Indoor Inverse Rendering with 3D Spatially-Varying Lighting”! It handles 3D lighting, disentangles spatially-varying effects, and benefits AR applications.
  
  project page: https://nv-tlabs.github.io/inverse-rendering-3d-lighting/
  
  reference: https://twitter.com/zianwang97/status/1445226424324038657?s=20
