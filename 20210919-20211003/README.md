### 意见性分享

#### 角度插值
  *Keenan Crane：If you need to interpolate rotations across space or time, there are much better options than Euler angles. 
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


