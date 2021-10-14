### 意见性分享
#### 线上参会建议

[Jia-Bin Huang](https://twitter.com/jbhuang0604)

**How to network in a virtual conference?**

**Excited to attend your first (virtual) conference?**

**How do we meet new people and expand the professional network?  Some ideas that I found useful** 

1.*Establish your goals before the conference* Check out the papers/workshops/networking sessions early. Identify the people you would really love to meet and create opportunities (cold-email, attend poster, ask questions.) You may find many people are incredibly approachable.

2.*Attend zoom poster sessions* Unlike in-person conferences where you barely squeeze through the crowd, zoom poster sessions are great opportunities to meet people with similar interests.  Oh, and please turn on your camera! It's not THAT awkward (maybe just a bit).

3.*Introduce yourself like Inigo Montoya* Like writing a cold email. The Inigo style is a simple and direct way of establishing a connection.

4.*Blame your advisor* Homework assignment for my students attending a conference: Send me a list of 10 people (names/affiliations/research interests) that they did not know before each day. It's a good excuse for you to reach out and meet new people (in order to do your HW).

5.*Sharing interesting contents with others* Sharing papers you like, talks you found inspiring, and quotes you found insightful.

6.*Follow-up with your new connections* Send a short follow-up email could go a long way.

7.*Be a decent human being* Don't discriminate, harass, and retaliate. It's really not that hard...

8.*Explore collaboration* The best way to deepen the connection is to explore collaboration.

***
### 课程和报告分享

#### 3DV线上讨论会

NEW APPROACHES TO 3D VISION 1st-4th November 2021 

Pleased to announce this Royal Society (royalsociety) online meeting on 3D vision bringing together researchers in computer vision, animal vision, and human vision.  

Website: [https://royalsociety.org/science-events-and-lectures/2021/11/3d-vision/…](https://t.co/s9OfSMHtgT?amp=1) 

DAY 1 (1st Nov) – Seeing Beyond SLAM  Chair: Andrew Fitzgibbon ([@Awfidius](https://twitter.com/Awfidius))

Session 1: Neural Scene Representation Ali Eslami ([@arkitus](https://twitter.com/arkitus)) + Ida Momennejad ([@criticalneuro](https://twitter.com/criticalneuro)) 

Session 2: Perception-Action Loop Sergey Levine ([@svlevine](https://twitter.com/svlevine)) + Andrew Glennerster([@ag3dvr](https://twitter.com/ag3dvr))

DAY 2 (2nd Nov) – Animals in Action  Chair: Matteo Carandini ([@MatteoCarandini](https://twitter.com/MatteoCarandini)) 

Session 1: Locating Prey + Reward Jenny Read ([@jcaread](https://twitter.com/jcaread)) + Aman Saleem ([@Aman_sal](https://twitter.com/Aman_sal)) 

Session 2: Navigation in 3D Space Kate Jeffery ([@drkjjeffery](https://twitter.com/drkjjeffery)) + Gily Ginosar ([@gilyginosar](https://twitter.com/gilyginosar))

DAY 3 (3rd Nov) – Experiencing Space Chair: Mar Gonzalez-Franco ([@twi_mar](https://twitter.com/twi_mar)) 

Session 1: Theories of Visual Space Dhanraj Vishwanath + Paul Linton ([@LintonVision](https://twitter.com/LintonVision)) 

Session 2: Challenges for Virtual Reality Sarah Creem-Regehr ([@SarahCreem](https://twitter.com/SarahCreem)) + Douglas Lanman ([@douglaslanman](https://twitter.com/douglaslanman))

DAY 4 (4th Nov) - Panel Discussion  The Chairs, Andrew Fitzgibbon ([@Awfidius](https://twitter.com/Awfidius)), Matteo Carandini ([@MatteoCarandini](https://twitter.com/MatteoCarandini)), Mar Gonzalez-Franco ([@twi_mar](https://twitter.com/twi_mar)), + Jody Culham ([@CulhamARI_Lab](https://twitter.com/CulhamARI_Lab)), share their thoughts on future directions for 3D vision

reference:https://twitter.com/LintonVision/status/1446146817608060928

***
### 成果推荐及讨论
- ##### A Constraint-based Formulation of Stable Neo-Hookean Materials
  [Miles Macklin](https://twitter.com/milesmacklin)

  Our latest paper shows how to add Neo-Hookean FEM to PBD using two simple constraint functions. 
  Paper: https://mmacklin.com/neohookean.pdf, 
  Video: https://mmacklin.com/neohookean_mig.mp4, 
  Demo: https://mmacklin.com/neohookean.html

  reference:https://twitter.com/milesmacklin/status/1445853253145559047
  
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

- ##### Compilable Markdown for Linear Algebra

  [Yong Li](https://twitter.com/liontigeryong)
  
  Excited to share our SIGGRAPH Asia'21 paper with Shoaib Kamil, @_AlecJacobson and @yig: "I love LA: Compilable Markdown for Linear Algebra"
  
  <div align=center><img src="https://pbs.twimg.com/media/FBMAn0vXICAXMMe?format=jpg&name=large" alt="Cover" width="75%"/></div>
  
  Mathematicians conventionally communicate linear algebra like this on a chalkboard or notepad. But on a computer, they must choose between writing in a semantically-underdefined language like LaTeX and languages with well-defined semantics but notation that no longer resembles chalkboard math, such as C++, Python, or MATLAB. We introduce I love LA, a language designed to closely mimic conventionally-written linear algebra and compile the same source code into LaTeX, C++, Python, and MATLAB. We designed I love LA by analyzing 1987 equations from all 142 papers in SIGGRAPH North America 2019. We demonstrate I love LA by translating examples and replacing code in open source projects. And the examples still run! Try it now!
  
  Project Page: https://iheartla.github.io/
  
  - **Jordan Ford:** Cool project! Would it make sense to intersperse lines of math as comments in the generated C++? That way you can see which lines of C++ correspond to which lines of math.

  reference: https://twitter.com/liontigeryong/status/1446501415833292801?s=20

- ##### Neo-Hookean model

  [Miles Macklin](https://twitter.com/milesmacklin)
  
  Our latest paper shows how to add Neo-Hookean FEM to PBD using two simple constraint functions. Paper: https://mmacklin.com/neohookean.pdf, Video: https://mmacklin.com/neohookean_mig.mp4, Demo: https://mmacklin.com/neohookean.html
  
  The great thing about the Neo-Hookean model is that it doesn't require a polar decomposition or SVD, which is a common stumbling block for implementation. Also, unlike models based on Green strain (e.g.: St. Venant-Kirchhoff) it has strong volume conservation / inversion recovery.
  
  reference: https://twitter.com/milesmacklin/status/1445853253145559047?s=20

- ##### cross-domain transfer in non-trivial continuous control

  [Arnaud Fickinger](https://twitter.com/arnaudfickinger)
  
  We provably achieve cross-domain transfer in non-trivial continuous control domain by minimizing the Gromov-Wasserstein distance with deep RL.
  
  Paper: http://arxiv.org/abs/2110.03684
  
  Site: https://arnaudfickinger.github.io/gwil/
  
  <div align=center><img src="https://pbs.twimg.com/media/FBbg8htVgAMY4IL?format=jpg&name=4096x4096" alt="Cover" width="50%"/></div>
  
  Imitation Learning is a good way to alleviate reward engineering. However, it generally fails when the expert’s and agent’s domains are too different, hence achieving only weak transfer. We create a benchmark to study cross-domain transfer, ranging from simple rigid transformation of the expert domain to arbitrary transformation of the state-action space, and propose Gromov-Wasserstein Imitation Learning (GWIL) to solve the benchmark. GWIL solves the benchmark while only requiring a single demonstration in the expert domain. In particular, GWIL does not require proxy tasks, unlike previous work in cross-domain imitation learning. GWIL can transfer from pendulum to cartpole with only one demonstration in the pendulum domain and without any external reward. A walker applying GWIL with a single cheetah demonstration and without any external reward can learn to move backward and forward by literally imitating a cheetah! Our theory formally characterizes the scenarios where GWIL preserves optimality, revealing its possibilities and limitations.
  
  <div align=center><img src="https://pbs.twimg.com/media/FBbhkj2VIAMKv9N?format=png&name=large" alt="Cover" width="75%"/></div>
  
  <div align=center><img src="https://pbs.twimg.com/media/FBbhmNjVcAQinRi?format=jpg&name=large" alt="Cover" width="75%"/></div>
  
  reference: https://twitter.com/arnaudfickinger/status/1447592679433375755?s=20

- ##### Neural-GIF

  [Gerard Pons-Moll](https://twitter.com/GerardPonsMoll1)
  
  Neural-GIF #ICCV2021. We use generalized Neural Implicit functions to control a neural implicit with pose. The trick to output such rich detail is to learn a deformation field before evaluating the neural distance field. Can be trained from raw scans without registration, and can be used to animate people and clothing. The formulation is clean and simple. The idea of expanding the shapes by deforming the underlying space is quite powerful. Check also the seminal Sclaroff and Pentland Siggraph'91 paper which inspires our work.
  
  reference: https://twitter.com/GerardPonsMoll1/status/1446915670667575299?s=20
  
- ##### NeRF series

  [Ajay Jain](https://twitter.com/ajayj_)
  
  Check out our new paper - we put NeRF on a diet! Given just 1 to 8 images, DietNeRF renders consistent novel views of an object using prior knowledge from large visual encoders like CLIP ViT. Given photos of a scene from many viewpoints, NeRF learns a volumetric representation that can be rendered from novel perspectives. NeRF works well given ~20-100 photos, but often not with a few (8, on left). DietNeRF adds an auxiliary loss that removes most artifacts (right). The core problem is that NeRF computes loss in pixel space, so renderings need to align pixel-wise with an observation. However, *a bulldozer is a bulldozer from any viewpoint*: images from different viewpoints share high-level semantic properties like object identity. Our DietNeRF regularizes the NeRF scene representation with a semantic consistency loss, computed in *a feature space*. This allows us to compare renderings from arbitrary poses. We use pre-trained CLIP and ImageNet Vision Transformers in experiments. pixelNeRF tackled the same problem by training NeRF on multiple similar scenes. This allows generalization to new scenes with only a few views. Using our loss, "DietPixelNeRF" synthesizes novel views with higher perceptual quality from *only a single monocular photo*. Our paper has details and bonus results, including extrapolation to completely unseen regions and tips for making this fast. Watch our video explanation for a quick overview: https://youtu.be/RF_3hsNizqw
  
  paper: https://arxiv.org/abs/2104.00677
  
  project: ajayj.com/dietnerf
  
  reference: https://twitter.com/ajayj_/status/1379475290154356738?s=20
