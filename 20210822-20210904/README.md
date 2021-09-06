### 意见性分享

- **关于论文迭代修改**
  
  [Matthias Niessner](https://twitter.com/MattNiessner)
  
  **Research can be quite brutal when a paper gets rejected.**
  
  Successful groups have the problem with many rejected submissions; but they don't give up, take reviewer feedback, and keep improving their work until it's ready for publication. Key is to recognize what was missing.
  
  **Abdullah Hamdi:** How to deal with deteriorating motivation to work on rejected papers and to ignore the exciting new topics that are emerging all the time?
  
  **Alessandro Saccon:** Even unsuccessful groups face the same issue. Just the key idea is neither good nor new enough, and their paper will never get accepted or less cited. So the real question for me is: how do you get a great idea?
  
  reference: https://twitter.com/MattNiessner/status/1429856784420900868?s=20
  
 - **关于期刊投稿**
 
   [Keenan Crane](https://twitter.com/keenanisalive)
   
   PSA: If you're waiting many months for a review to come back from ACM Transactions on Graphics (and, I suspect, many other journals), you can and should politely nudge the Editor in Chief.  TOG reviews are supposed to take only 1 month, and the EiC already knows the author names.
   
   reference: https://twitter.com/keenanisalive/status/1433422779311869957?s=20
  
- **关于AI技术的思考**

  [Matthias Niessner](https://twitter.com/MattNiessner)
  
  There's still this illusion that "AI" is somewhat intelligent: these are models fitted to large datasets using non-linear optimizations, hoping to replicate their distributions. While these are incredibly useful tools, there is nothing we would consider human-like intelligence.
  
  - **Theodore Galanos:** GPT3 has definitely shown instances of human-like intelligence, although I doubt that qualification is all important for AGI. I agree it's not specifically the model or the architecture but I do entirely believe it is the 'large datasets',  specifically the language ones.
    - **John Manoochehri:** inb4 it's like something computational which we have detected in human intelligence.
    - **Theodore Galanos:** Very far from an expert, my view is generalization to, if not arbitrary, rather novel downstream tasks with very little experience (and I believe generalization is a standard aspect of human intelligence?). Few-shot, zero-shot, prompt engineering, have shown glimpses of that.
    - **John Manoochehri:** Except it's the opposite: all the ML training req'd is exactly what we have to assume humans don't have, at least in the very prominent case of language acquisition.
  
  - **Zayd:** True intelligence is the unsupervised learning. GPT-3 is good at data (and combinations of) it has seen. It can't go beyond that.

  reference: https://twitter.com/MattNiessner/status/1434504873073156105?s=20
  
***
### 课程和报告分享

#### Symposium on Computer Animation 2021

##### original twitter link（from Michiel van de Panne）：
https://twitter.com/Mvandepanne/status/1429182659859820548

##### webpage：
http://computeranimation.org/program.html#Session1

##### location & time：

September 7-10,2021. Online.

registration web: [http://computeranimation.org/#Registration](https://t.co/3P1KvcK6gf?amp=1)

##### 计算机动画相关论文报告会

***
#### Geometric Deep Learning - Algorithms

##### original twitter link（from Isaac Newton Institute）:
https://twitter.com/NewtonInstitute/status/1430084967858589715?s=20

##### webpage:
https://www.newton.ac.uk/seminar/20210824100011001/

##### location & time:
24 August 2021 – 10:00 to 11:00

##### video page:
https://www.youtube.com/watch?v=9mOX_JbVTNY&ab_channel=INISeminarRoom1

##### 几何深度学习算法

***
#### Advances in Neural Rendering is now freely available on YouTube

##### original twitter link（from Justus Thies）:
https://twitter.com/JustusThies/status/1431291841404719109

##### video page
https://www.youtube.com/watch?v=otly9jcZ0Jg
https://www.youtube.com/watch?v=aboFl5ozImM

##### 神经渲染前沿介绍视频公开![Image](https://pbs.twimg.com/media/E9z3WO1WQAMz5FZ?format=jpg&name=900x900)

***
#### creating yarn art in using Metropolis-Hastings sampling


### 成果推荐及讨论


- ##### [Seungbae Bang](https://twitter.com/Seungbae13)
  **Happy to announce our "Complementary Dynamics" source code is now publicly available.**
  
  <div align=center><img src="https://github.com/seungbaebang/complementary-dynamics-cpp/blob/master/showcases/elephant_arap.gif" alt="Cover" width="75%"/></div>
  
  Matlab repo: https://github.com/ErisZhang/complementary-dynamics
  
  C++ repo: https://github.com/seungbaebang/complementary-dynamics-cpp

  reference: https://twitter.com/Seungbae13/status/1429905759270277131?s=20
  
- ##### [Tomasz Malisiewicz](https://twitter.com/quantombone)
  **3D Reconstruction from public webcams**
  
  Hey @AmirRubin, check out this 3D #computervision project which uses SuperGlue, a deep feature-based matcher—extremely useful for creating a robust #digitaltwin of outdoor spaces. Thanks @ducha_aiki for sharing!

  <div align=center><img src="https://pbs.twimg.com/media/E9jm_PyX0Bwm06X?format=jpg&name=small" alt="Cover" width="75%"/></div>
  
  abs: https://arxiv.org/abs/2108.09476
  
  - **Amir Rubin:** I love this! SuperGlue and deep front ends are game changers for 3D reconstruction. The robustness of learned features+homography is bringing digital twin creation into the hands of non-expert users. I mean, I’m not talking metaverse scale just yet but who knows?

  - **Noé:** Wow indeed, this is wild. It's the difference between an idea not working at all, and working quite well. There have to be ideas from the past which did not pan out that have to be re-investigated! Do you have insights on use-cases where it made a large difference?

  <div align=center><img src="https://pbs.twimg.com/media/E9lPVSAWEAg28Fi?format=jpg&name=small" alt="Cover" width="75%"/></div>
  reference: https://twitter.com/quantombone/status/1430146858773630994?s=20

- ##### [Thiemo Alldieck](https://twitter.com/thmo_a)
  **imGHUM: Implicit Generative Models of 3D Human Shape and Articulated Pose**
  
  pdf：https://arxiv.org/pdf/2108.10842.pdf
  
  code：https://github.com/google-research/google-research/tree/master/imghum
  
  imGHUM shares it parameterization with the explicit body model GHUM (https://github.com/google-research/google-research/tree/master/ghum). But imGHUM is a SDF, thus fitting to point clouds is straight-forward and fully differentiable. Here we use imGHUM to recover pose and shape parameters of (partial) scans. 
  
  ![Image](https://pbs.twimg.com/media/E9nrF7cXIAILtXt?format=jpg&name=900x900)
  
  The implicit semantics returned by imGHUM allows e.g. for surface coloring or texturing. Together with the signed distance they are also a 4D descriptor of points in space.
  
  <div align=center><img src="https://pbs.twimg.com/media/E9nrxNeXIAAi8hY?format=jpg&name=900x900" alt="Cover" width="50%"/></div>
  
  imGHUM generalizes well to novel shapes and poses. We provide gender-neutral, male and female imGHUM models of the full body, head, left and right hand. 
  
  <div align=center><img src="https://pbs.twimg.com/media/E9nspWNXoAMLF1Q?format=jpg&name=900x900" alt="Cover" width="70%"/></div>
  
- ##### [Tomasz Malisiewicz](https://twitter.com/quantombone)
  **DROID-SLAM: Deep Visual SLAM for Monocular, Stereo, and RGB-D Cameras**
  
  pdf: https://arxiv.org/abs/2108.10869
  
  The method uses recurrent iterative updates of camera pose and pixelwise depth through a Dense Bundle Adjustment layer. Runs in real-time with two 3090 GPUs.
  
  ![Image](https://pbs.twimg.com/media/E9mxwLCXoAMYa6q?format=jpg&name=900x900)
  
- ##### [Andrew Davison](https://twitter.com/AjdDavison)
  **Semantic NeRF**
  **We add semantics outputs to NeRF models of 3D occupancy/colour. Joint representation allows very sparse or noisy in-place supervision to generate high quality dense prediction.**
  
  project page:https://shuaifengzhi.com/Semantic-NeRF/


  - **Andrew Davison**: Of course this is just the beginning of potential more general use of neural implicit models to represent scene properties, such as surface properties or affordances which could be very useful in robotics.

  reference:https://twitter.com/AjdDavison/status/1430884726705901568

- ##### [TensorFlow](https://twitter.com/TensorFlow)
  **MoveNet is now on mobile!**
  
  The state-of-the-art pose estimation model finally comes to mobile via TensorFlow Lite with CPU acceleration enabled. Now you can run pose estimation in realtime on modern smartphones.
  
  [Learn more](https://t.co/lmGgSVEbz4?amp=1)
  
  - **Glooface**: Does it work on cats? My one has always fanatasised about being a saber-toothed tiger.
    - **Khanh**: This model can only detect human poses at this moment, but I took note of the feature request.
  
  - **Khanh**: This MoveNet model is provided as a standalone TFLite model with sample implementation written in Kotlin, Python and Swift (coming soon) while MediaPipe requires you to be familiar with Bazel and C++. I think MoveNet is easier to use for mobile developers.

  - **hichem le s**: This one seems to be better,  i used years ago mediapipe and the model was not so performant as this one, maybe mediapipe become better than years ago i dont know.

  reference: https://twitter.com/TensorFlow/status/1427300403494928386?s=20
  
- ##### [Ankur Handa](https://twitter.com/ankurhandos)
  **We are excited to share Isaac Gym tech report https://arxiv.org/abs/2108.10470.** Physics simulation data is directly passed to pytorch without ever going through any CPU bottlenecks in the process allowing blazing fast training on many challenging environments.
  
  We can train shadow hand cube rotation with all sorts of randomisations (as detailed in https://arxiv.org/abs/1808.00177) in  ~ 1 hour using feed forward networks and ~6 hours with LSTMs.
  
  <div align=center><img src="https://pbs.twimg.com/media/E9xkex0UUAUBthn?format=png&name=small" alt="Cover" width="50%"/></div>
  
  Many other interesting results are available here: https://sites.google.com/view/isaacgym-nvidia
  
  reference: https://twitter.com/ankurhandos/status/1431130561804865538?s=20

- ##### [Kostas Daniilidis](https://twitter.com/KostasPenn)
  **Guess the dance!** Produced by [the amazing notebook](https://github.com/nkolot/ProHMR) developed by @nikoskolot @geopavlakos based on our #ICCV2021 ProHMR.(So easy to run that even I an old professor can run it. Video cut to hide the name of the dance).
  
  reference: https://twitter.com/KostasPenn/status/1432351412885676033?s=20
  
- ##### [Alex Mordvintsev](https://twitter.com/zzznah)
  **"Controlling Neural CA with noise"** -- new tutorial where I'm trying to document the exploration precess (idea -> experiment -> early results). I'd really appreciate your feedback!
  
  [![Watch the video](https://img.youtube.com/vi/i59K8UT9UK4/hqdefault.jpg)](https://youtu.be/i59K8UT9UK4)
  
  [final colab code](https://colab.research.google.com/github/google-research/self-organising-systems/blob/master/notebooks/noise_controlled_nca.ipynb)
  
  - **MΞMO AKTEN**: AFAIU noise amt is essentially a conditioning signal. In fact have you already tried any arbitrary (real valued?) signal? i.e. 0=> bubbles, 1=> tiles, & then vary this signal spatially & temporally? in this case Up pointing backhand index, it's still one (albeit parametrized) neural controller shared by all agents. Of course broader question is :), have you had a chance to try Neural CA w two populations of agents (coop and/or competitive) with one controller per population (but trained together)?

  - **Scott Condron**: I don’t think there’s enough of these types of videos where you’re brought through the process of experimentation. I personally would enjoy a distill-style post about this, but just the video and colab get the ideas across without it. As for future ideas, I thought the way the bubble stayed intact over the noise boundary was surprising and could be interesting to study further. Is there certain patterns that are more robust than others? Can you encourage that robustness through training?
    - **Alex Mordvintsev**: I began with training a noise-robust CA, then switched to noise-controlled. I think there are so many curious aspects that deserve deeper study about these models, that I decided to do tutorials to show how to do that, rather than have all fun myself and never release most it. I'm thinking about making a few more small tutorials and then combining them into more in-depth article.
  
  reference: https://twitter.com/zzznah/status/1432322113856229379?s=20

- ##### [Kangxue Yin](https://twitter.com/kangxue_yin)

  **3DStyleNet**

  Excited to share [#3DStyleNet](https://twitter.com/hashtag/3DStyleNet?src=hashtag_click), a Neural Style Transfer method for 3D Shapes!  The work is accepted to [#ICCV2021](https://twitter.com/hashtag/ICCV2021?src=hashtag_click) as an oral presentation. 

  arXiv:  [https://arxiv.org/abs/2108.12958](https://t.co/V34VYVNK1L?amp=1) 

  Project page: [https://nv-tlabs.github.io/3DStyleNet/](https://t.co/dSuOYsMPwj?amp=1)

<div align=center><img src="https://nv-tlabs.github.io/3DStyleNet/assets/teaser.jpg" alt="Cover" width="75%"/></div>
  reference:https://twitter.com/kangxue_yin/status/1432833663453040643

- ##### [NAVER LABS Europe](https://twitter.com/naverlabseurope)

  Just released !- largest indoor localization dataset with 130K images (5 datasets). Captured with [@NAVERLABSHQ](https://twitter.com/NAVERLABSHQ)

  techno & available in unified data format 'kapture'. 

  Datasets: [https://naverlabs.com/en/datasets](https://t.co/uytql7Al4c?amp=1) 

  CVPR21 paper: [https://bit.ly/3ymnmVY](https://t.co/35kq79eSF7?amp=1)

  reference:https://twitter.com/naverlabseurope/status/1395255973862940672

- ##### [Tomasz Malisiewicz](https://twitter.com/quantombone)

  **What You Can Learn by Staring at a Blank Wall**
  
  arxiv: [arxiv.org/abs/2108.13027](https://t.co/LzmwOJXZW3?amp=1) 
  
  This [#computervision](https://twitter.com/hashtag/computervision?src=hashtag_click) paper from [@MIT_vision](https://twitter.com/MIT_vision) introduces a passive non-line-of-sight method that infers the number of people or activity of a person from the observation of a blank wall in an unknown room.
  
    <div align=center><img src="https://pbs.twimg.com/media/E-FX4O0XEAI1KJa?format=jpg" alt="Cover" width="75%"/></div>

- ##### [Daniele Panozzo](https://twitter.com/DanielePanozzo)
  Are you developing new data-driven algorithms to simulate physical systems? Check out our new dataset generator and benchmark! We discovered that outperforming classical time integrator algorithms is not easy even with large datasets. 
  [@NeurIPSConf](https://twitter.com/NeurIPSConf)[https://arxiv.org/abs/2108.07799]

    <div align=center><img src="https://pbs.twimg.com/media/E-Egrq_WQAcP4Id?format=jpg" alt="Cover" width="75%"/></div>
