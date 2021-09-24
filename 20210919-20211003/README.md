### 意见性分享

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
  **Keenan Crane：** If you need to interpolate rotations across space or time, there are much better options than Euler angles. 
  Here, rotations at the four corners are interpolated via the exp/log map.
  
  Want to know more?
  
  Some exercises: http://15462.courses.cs.cmu.edu/fall2021content/exercises/Exercises06.pdf
  
  & solutions: http://15462.courses.cs.cmu.edu/fall2021content/exercises/Solutions06.pdf*
  
  - Keenan Crane:As long as you’re careful about sign, should be the same. Quaternions live in the 3-sphere S^3, which double covers the rotation group SO(3) and locally has the   same geometry. I like log because it naturally yields the smallest rotation & you don’t have to mess around with signs.
  - Jacopo Bertotolli:Euler angles have a nice and simple interpretation (rotation is a change in the third Euler angle, precession is a change in the first Euler angle, nutation is a change in the second Euler angle).Is there a simple interpretation for the exp/log map too?
  - Keenan Crane:Yep—check out the linked exercises.Exp map turns a rotation matrix into axis/angle of rotation.Log map turns axis/angle into a rotation matrix.(There’s also a beautiful geometric picture of Lie groups/Lie algebras not covered there.)
  

### 课程和报告分享

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
  
  
