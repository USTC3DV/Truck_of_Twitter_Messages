### 意见性分享

#### 如何让教授回复你的邮件

[Jia-Bin Huang](https://twitter.com/jbhuang0604)

**How do I get professors to answer my emails? You have sent SO MANY emails to professors for scheduling your prelim, looking for research opportunities, or asking questions about courses etc. But they just don't reply at all!** 

**How do I get things done? A few tips below.**

1.*Group scheduling*  Don't send out Doodle/When2meet with 30+ entries! Look up their (course) schedules and propose only a few (3-5) time slots.  If they need to spend 15 mins filling out your scheduling request, they will simply ignore your email.

2.*Give them the control for planning their day*  Scheduling a meeting: Don't: When will you be available? Do: I am available ... Will you be available in one of the time slots? When you ask for availability, you are effectively asking for commitment for ALL of the time slots.

3.*Calendar invite*  Once you scheduled a meeting. Please do send a calendar invite with all the required information (e.g., zoom link).  Whatever that's not on their calendar does not exist.

4.*Go 90% and let them finish the 10%*  

• Need a form? Pre-fill it as much as you can (you know their name and email).

• Need a cover letter? Write a draft first. 

• Need a ref. letter? Send an updated CV and SOP. 

• Need to ask about a course? Read the syllabus first.

5.*cc all parties involved*  Asking for some code/data/clarification? cc'ing your PI and their PI definitely helps you get a prompt reply!

6.*Don't cc all parties involved* Don't send requests to MULTIPLE people in the same thread. Everyone will assume others will do it and therefore no one will do it. Send INDIVIDUAL emails instead.

7.*One email one topic* Help your professors respond your email quickly. Make your emails simple, clear, and actionable.

8.*Formatting* You are not writing in plain texts.  Formatting your email so that it's easy to read, e.g.,  

• bullet points for parallel concepts 

• bold font for highlighting 

 • bold phrase for organizing your email 

 • italic for sentence stress

9.*Timeline* Provide specific action and specific date that the task needed to be completed. This helps them plan their schedule to make time for your requests.

reference:https://twitter.com/jbhuang0604/status/1441548826645602309

#### 手把手教你做深度学习研究
  **Matthias Niessner:** How to start a deep learning project?

  We use a remarkably streamlined step-by-step process to set up deep learning projects. At the same time, people who are new to deep learning tend to always make the same (avoidable) mistakes. Check out the thread below!

  General advice: start simple -> use a small architecture (less than 1 mio params). In vision, ENet or a crippled ResNet-18 (only the first blocks) is a good choice. Common mistake: train model with 100mio+ params for 3 weeks only to notice that the data loader is broken.

  No fancy features: disable dropout, no batchnorm, no learning rate decay, etc. These may give you a few % points at the end, but at the beginning they complicate everything; e.g., LR decay often falsely makes train curves look like they are converged.

  Set up train/val: loss curves are all you have for debugging (TensorBoard is a great tool). Make sure to log loss for every batch (not just once an epoch); log val the same way as train: i.e., after every iteration run a forward pass for a random batch from the val set.

  Overfit to a single train sample first: this debugs your output, which you expect the network to fully memorize. If you turn off all regularizes, such as weight decay, train loss should go to zero. Note that the input to the network will be ignored in this experiment.

  Overfit to 5-10 train samples: now the network needs to predict different outputs depending on the input. For tasks like classification, train loss should still go to zero and training should take at most a few minutes. Val loss will go up as you don’t learn anything yet.

  With the previous steps, you verified data loading and whether basic optimizing works. Now it’s time to throw more data at the problem. Here, the goal is generalize for the first time – if your val loss goes down (even just slightly), congrats, you learned something :)

  Training speed: given that deep learning is so empirical, it’s critical that your setup facilitates fast turnaround times for debugging. Make sure you understand where the bottle neck lies (data loading vs backprop); a single batch should be processed in under a second.

  Once you have the basic setup running, it’s finally time to improve the overall performance. In addition to the train/val curves, you want to log curves for metrics, such as mIoU, accuracy, F1, etc., on the val set; visualize these during training.

  Run many ablations at the same time: already after a few iterations / few minutes of training, loss curves and metrics tell you whether an experiment has promise or not. Kill experiments that don’t show promise and start new ones with different hyper parameters.

  Data engineering: mostly, your performance is limited due to data (e.g., overfitting). Here, weight balancing between classes and augmentations (e.g., rotations, noise, etc.) come into play. Important: never augment the val set as it would make it impossible to compare.

  For generative models, such as GANs, always start without a discriminator loss. Instead, just do a simple L1 regression first - only once that works, add the D (Wasserstein is a good choice). GANs mostly struggle due to data issues -> start with a simple distribution.

  Finally, it’s time to try out bigger architectures. ResNet-XXX, InceptionNet, XceptionNet etc. are good choices, and try out other features which we removed before (dropout, batchnorm, LR decay, etc.). If you have the compute resources, make sure multi-GPU training works.

  reference: https://twitter.com/MattNiessner/status/1441027241870118913?s=20

#### 角度插值
  **Keenan Crane:** If you need to interpolate rotations across space or time, there are much better options than Euler angles. 
  Here, rotations at the four corners are interpolated via the exp/log map.

  Want to know more?

  Some exercises: http://15462.courses.cs.cmu.edu/fall2021content/exercises/Exercises06.pdf

  & solutions: http://15462.courses.cs.cmu.edu/fall2021content/exercises/Solutions06.pdf*

  - Keenan Crane:As long as you’re careful about sign, should be the same. Quaternions live in the 3-sphere S^3, which double covers the rotation group SO(3) and locally has the   same geometry. I like log because it naturally yields the smallest rotation & you don’t have to mess around with signs.
  - Jacopo Bertotolli:Euler angles have a nice and simple interpretation (rotation is a change in the third Euler angle, precession is a change in the first Euler angle, nutation is a change in the second Euler angle).Is there a simple interpretation for the exp/log map too?
  - Keenan Crane:Yep—check out the linked exercises.Exp map turns a rotation matrix into axis/angle of rotation.Log map turns axis/angle into a rotation matrix.(There’s also a beautiful geometric picture of Lie groups/Lie algebras not covered there.)

#### 读博的意义
  **Shreya Shankar:** my college friend who also just started her PhD said "some people leave their jobs to go backpacking around the world for a few years. that's basically us except we're doing mental backpacking" and i can't stop thinking about how true that is. also, both have extended periods of social isolation + involve repeatedly questioning the decision + sometimes lead to cool TED talks by the end!

  reference: https://twitter.com/sh_reya/status/1441194510738853897?s=20

### 课程和报告分享


#### NYU:Deep Learning Spring 2021 class

course page:https://twitter.com/NYUDataScience/status/1443635953101275136

<div align=center><img src="https://pbs.twimg.com/media/FAjTDoUVQAMGqZ_?format=jpg&name=small" alt="Cover" width="50%"/></div>

reference:https://twitter.com/MLStreetTalk/status/1439517187119722497


#### Geometric deep learning lecture

 Epic special edition MLST on geometric deep learning! Been in the works since May!

<div align=center><img src="https://pbs.twimg.com/media/E_owvmfWEAUgWaL?format=jpg&name=large" alt="Cover" width="50%"/></div>

webpage: https://anchor.fm/machinelearningstreettalk/episodes/60-Geometric-Deep-Learning-Blueprint-Special-Edition-e17i495

reference: https://twitter.com/MLStreetTalk/status/1439517187119722497

#### Physics based DeepLearning Book

New #Physics based #DeepLearning Book (v0.1)

http://physicsbaseddeeplearning.org/intro.html

<div align=center><img src="https://pbs.twimg.com/media/E_un_dgX0Ag9d1P?format=jpg&name=large" alt="Cover" width="35%"/></div>

reference: https://twitter.com/CSProfKGD/status/1439929218851278850?s=20

#### Urban Modeling (3DGV)

#3DGV 3DGV welcomes topics on urban modeling. Our next speaker is Peter Wonka (KAUST). Talk title: "Modeling Urban Environments". Panelist: Yasutaka Furukawa (SFU).

Link: https://www.youtube.com/watch?v=jsFztFXiPTM&ab_channel=3DGVSeminar

9/29 9:00 am (Pacific) 9/29 19:00 pm (Thuwal)

reference: https://twitter.com/qixing_huang/status/1442929109038862337?s=20


***
### 成果推荐及讨论
- ##### Torch.manual_seed(3407)

  [Dmytro Mishkin](https://twitter.com/ducha_aiki)
  
  Torch.manual_seed(3407) is all you need: On the influence of random seeds in deep learning architectures for computer vision
  
  One can easily get +0.2 pp accuracy on ImageNet just by changing random seed. And much more on CIFAR10.
  
  ArXiv: https://arxiv.org/abs/2109.08203
  
  <div align=center><img src="https://pbs.twimg.com/media/E_tglAwXIAM5k0j?format=jpg&name=900x900" alt="Cover" width="50%"/></div>
  
  - **Dmytro Mishkin:** Similar study was published at #ICLR2016 workshop: Neural Network Training Variations in Speech and Subsequent Performance Evaluation (https://openreview.net/forum?id=OM0jKROjrFp57ZJjtNkv)

  reference: https://twitter.com/ducha_aiki/status/1439850704559034369?s=20

- ##### Cloud based reconstruction

  [EveryPoint](https://twitter.com/EveryPointIO)
  
  Our cloud based reconstruction enginee can handle most about any image source. Here is our own @jonstephens85 out capturing field data with a @SkydioHQ 2 and an @Apple iPad Pro! He also filmed the video with his #RayBanStories which works for #3D modeling.

  reference: https://twitter.com/EveryPointIO/status/1441070951416799246?s=20
  
- ##### Differentiable Rendering

  [Wenzel Jakob](https://twitter.com/wenzeljakob)
  
  Differentiable rendering of meshes tends to produce horrible, tangled geometry. We propose a simple and efficient way to fix this, to appear in SIGGRAPH Asia'21.
  
  Differentiable rendering can be surprisingly fragile whenever meshes are involved. A noisy gradient descent step is all it takes to turn the current reconstruction inside-out. The standard countermeasure for those kinds of problems is called Laplacian regularization.
  
  <div align=center><img src="https://pbs.twimg.com/media/E_-PsYeXMAAhwWu?format=jpg&name=4096x4096" alt="Cover" width="50%"/></div>
  
  Roughly speaking, a Laplacian regularizer wants each vertex to be at the center of its neighbors. This tightly couples the optimization variables, which is something that first-order methods like gradient descent really struggle with. Regularization is also always a compromise: we must give up on finding the best solution in exchange for one that is reasonably smooth. Our method addresses both of these limitations.
  
  The core idea is to go to second order (think: Newton's method) in the smoothness term, within an overall first-order optimization. The result can be interpreted as Sobolev preconditioned descent, or as a mesh reparameterization via @OlgaSorkineH's differential coordinates. The overhead of doing this is tiny compared to the rest of the differentiable rendering pipeline. Hooray! The paper and video are available here: https://rgl.epfl.ch/publications/Nicolet2021Large
  
  Disclaimer: Sobolev preconditioned gradient descent involving mesh energies has been used by others, in some cases decades ago. The contribution of this paper is to realize how useful such techniques can be for differentiable rendering, and to show how it all fits together.
  
  reference: https://twitter.com/wenzeljakob/status/1441030070240481283?s=20

- ##### Dense Prediction Transformers

  [Alexey Bochkovskiy](https://twitter.com/alexeyab84)
  
  DPT (Dense Prediction Transformers) is accepted to ICCV2021 - State of the art Real-time (>30 FPS) neural network for Semantic segmentation and Mono-Depth estimation from one RGB image
  
  Paper: https://arxiv.org/abs/2103.13413
  
  Code: https://github.com/isl-org/MiDaS
  
  - **PYXIS Robocar:** Dear Alexey, Do you use a personal code to convert depth map into point cloud, or do you use a library like OPEN3D or PCL?
    - Alexey Bochkovskiy: I used Open3D.
  
  reference: https://twitter.com/alexeyab84/status/1441393585836855313?s=20
  
- ##### Real-Time SLAM System

  [Edgar Sucar](https://twitter.com/SucarEdgar)
  
  We will be presenting our new real-time SLAM system iMAP at #ICCV2021! With a neural implicit scene representation it can map scenes efficiently, fill holes, and jointly optimise the 3D map and camera poses.
  
  Project Page: https://edgarsucar.github.io/iMAP/
  
  - **Andrew Davison:** #ICCV2021, Dyson Robotics Lab at Imperial: iMAP is the first SLAM system based on continual, real-time learning of an implicit neural representation. In 3 minutes a 1MB MLP model captures global shape and detail, with convincing scene completion despite no prior training data.

  reference: https://twitter.com/SucarEdgar/status/1441358051966013440?s=20
  
- ##### Differentiable Delaunay Triangulation

  [GraphicsSurvey](https://twitter.com/GraphicsSurvey)
  
  Differentiable Delaunay Triangulation to convert 2D vertices into soft triangulation.
  
  It enables gradient descent for any per-vertex/face objectives such as minimization of triangle size.
  
  <div align=center><img src="https://pbs.twimg.com/media/FADFj3bUUAEuHAB?format=jpg&name=4096x4096" alt="Cover" width="50%"/></div>
  
  reference: https://twitter.com/GraphicsSurvey/status/1441372150535897093?s=20
  
- ##### Pri3D code is released

  [Ji Hou](https://twitter.com/sekunde_)

  Happy to release our Pri3D code and pre-trained models. Pre-training on 3D Priors helps 2D downstream tasks. 
  Code and pre-trained models: https://github.com/Sekunde/Pri3D
  Video: https://youtube.com/watch?v=S2VodtyfQbQ

  

  ![Pri3D](https://github.com/Sekunde/Pri3D/raw/main/assets/pri3d.jpg)

- ##### real-time SLAM system iMAP

  [Edgar Sucar](https://twitter.com/SucarEdgar)
  
  We will be presenting our new real-time SLAM system iMAP at #ICCV2021! With a neural implicit scene representation it can map scenes efficiently, fill holes, and jointly optimise the 3D map and camera poses https://edgarsucar.github.io/iMAP/
  
- ##### Self-Supervised Vessel Enhancement Using Flow-Based Consistencies

  [Rohit Jena](https://twitter.com/rohitrango)
  
  If you're attending MICCAI this year, be sure to check out our poster titled "Self-Supervised Vessel Enhancement Using Flow-Based Consistencies" on Sep 28 (Tuesday) from 14:00-15:30 EDT. Star-struck
  
  Paper: https://arxiv.org/abs/2101.05145
  
  Code: https://bit.ly/flow-seg
  
  ![img](https://pbs.twimg.com/card_img/1440637485449576454/Zv92MBE-?format=jpg&name=900x900)
  
- ##### 3D representation

  [Andrea Tagliasacchi](https://twitter.com/taiyasaki)
  
  Sun et al. "Canonical Capsules: Unsupervised Capsules in Canonical Pose"
  
  A network design that realizes the concept of "mental picture" for unsupervised 3D deep learning.
  
  This representation enables state-of-the-art results across a number of applications, such as  canonicalization (i.e. registration), reconstruction (i.e. auto-encoding), as well as unsupervised classification.
  
  project page: https://canonical-capsules.github.io/
  
  - **Geoffrey Hinton:** Finding the natural parts of an object and their intrinsic coordinate frames without supervision is a crucial step in learning to parse images into part-whole hierarchies. If we start with point clouds, we can do it!

  reference: https://twitter.com/taiyasaki/status/1336843955619520521?s=20
  
- ##### Shape from Blur @ NeurIPS 2021

  [Denys Rozumnyi](https://twitter.com/DRozumnyi)
  
  Shape from Blur will appear in NeurIPS 2021! We jointly reconstruct the 3D shape, texture, and 6D motion of a motion-blurred object from a single image.
  
  video: https://www.youtube.com/watch?v=hPYWh9KGiu8&ab_channel=DenysRozumnyi
  
  arXiv: https://arxiv.org/abs/2106.08762
  
  reference: https://twitter.com/DRozumnyi/status/1443187927861841921?s=20
  
- ##### Neural Trees for Learning on Graphs @ NeurIPS 2021

  [Luca Carlone](https://twitter.com/lucacarlone1)
  
  Our Neural Tree paper has been accepted at #Neurips2021! kudos to Rajat, Siyi, & Lisa! The paper connects graph neural nets with inference in probabilistic graphical models, and provides a new architecture with strong theoretical & practical performance.
  
  paper: https://arxiv.org/pdf/2105.07264.pdf
  
  reference: https://twitter.com/lucacarlone1/status/1443210220302331906?s=20

- ##### a textless NLP model

  [Facebook AI](https://twitter.com/facebookai)

  GSLM, our first-of-its-kind “textless #NLP” model, learns to generate expressive speech using only raw audio as input. https://ai.facebook.com/blog/textless-nlp-generating-expressive-speech-from-raw-audio/. It generates novel content & prosody congruently with a prompt’s expressive style.
  
  reference: https://twitter.com/facebookai/status/1443991702297927683?s=20
  
- ##### Time of Flight Sensor + NERF

  [AK](https://twitter.com/ak92501)
  
  TöRF: Time-of-Flight Radiance Fields for Dynamic Scene View Synthesis
  
  pdf: https://arxiv.org/pdf/2109.15271.pdf
  abs: https://arxiv.org/abs/2109.15271
  project page: https://imaging.cs.cmu.edu/torf/
  
  - **Aaron Gokaslan:** Time of Flight Sensor + NERF = ToRF. Dynamic Scene View Synthesis is an underconstrained problem. We tackle this problem by incorporating measurements from Time of Flight cameras, which are often used as depth cameras on modern smartphones.

  - **Christian Richardt:** What do you get when you combine Time-of-Flight imaging with NeRF? — TöRF, of course! By modelling raw phasor measurements, our method becomes robust to phase wrapping, multi-path interference, low reflectance, and erroneous camera calibration. #NeurIPS2021

  reference: https://twitter.com/ak92501/status/1443741010471923713?s=20

- ##### Hilti SLAM Challenge Dataset

  [Davide Scaramuzza](https://twitter.com/davsca1)
  
  The datasets will remain publicly available and we hope they will become a new benchmark to improve state of the art  accuracy and robustness of SLAM systems for construction sites! The paper describing the dataset is here: https://arxiv.org/abs/2109.11316
  
  reference: https://twitter.com/davsca1/status/1444264714670903296?s=20
  
  
- ##### PASS Dataset

  [Yuki](https://twitter.com/y_m_asano)
  
  Today we  Oxford_VGG release the dataset 𝐏𝐀𝐒𝐒: 1.4M, CC-BY licensed images that do not depict humans, human parts or other PID. It can be used for self-supervised pretraining and works as well as ImageNet.
 
  info & models: https://github.com/yukimasano/PASS/
  paper: https://arxiv.org/abs/2109.13228
  
  <div align=center><img src="https://github.com/yukimasano/PASS/blob/main/pass.gif?raw=true" alt="Cover" width="75%"/></div>
  
  reference: https://twitter.com/y_m_asano/status/1442764357713244160
  
