> 公众号：[3D视觉工坊](https://mp.weixin.qq.com/s?__biz=MzU1MjY4MTA1MQ==&mid=2247484684&idx=1&sn=e812540aee03a4fc54e44d5555ccb843&chksm=fbff2e38cc88a72e180f0f6b0f7b906dd616e7d71fffb9205d529f1238e8ef0f0c5554c27dd7&token=691734513&lang=zh_CN#rd)
>
> 主要关注：3D视觉算法、SLAM、vSLAM、计算机视觉、深度学习、自动驾驶、图像处理以及技术干货分享
>
> 运营者和嘉宾介绍：运营者来自国内一线大厂的算法工程师，深研3D视觉、vSLAM、计算机视觉、点云处理、深度学习、自动驾驶、图像处理、三维重建等领域，特邀嘉宾包括国内外知名高校的博士硕士，旷视、商汤、百度、阿里等就职的算法大佬，欢迎一起交流学习

# SLAM

## 优秀开源项目汇总

[https://github.com/OpenSLAM/awesome-SLAM-list](https://github.com/OpenSLAM/awesome-SLAM-list)

[https://github.com/tzutalin/awesome-visual-slam](https://github.com/tzutalin/awesome-visual-slam)

https://github.com/kanster/awesome-slam

https://github.com/YoujieXia/Awesome-SLAM

[Recent_SLAM_Research](https://github.com/YiChenCityU/Recent_SLAM_Research)

[https://github.com/youngguncho/awesome-slam-datasets](https://github.com/youngguncho/awesome-slam-datasets)

[https://github.com/marknabil/SFM-Visual-SLAM](https://github.com/marknabil/SFM-Visual-SLAM)

[https://github.com/ckddls1321/SLAM_Resources](https://github.com/ckddls1321/SLAM_Resources)

## 激光SLAM

> 分为前端和后端。其中前端主要完成匹配和位置估计，后端主要完成进一步的优化约束。
>
> 整个SLAM大概可以分为前端和后端，前端相当于VO（视觉里程计），研究帧与帧之间变换关系。首先提取每帧图像特征点，利用相邻帧图像，进行特征点匹配，然后利用RANSAC去除大噪声，然后进行匹配，得到一个pose信息（位置和姿态），同时可以利用IMU（Inertial measurement unit惯性测量单元）提供的姿态信息进行滤波融合。
>
> 后端则主要是对前端出结果进行优化，利用滤波理论（EKF、UKF、PF）、或者优化理论TORO、G2O进行树或者图的优化。最终得到最优的位姿估计。

### 数据预处理

### 点云匹配

### 地图构建

## 视觉SLAM

### Books

- [视觉SLAM十四讲]() 高翔
- [机器人学中的状态估计]()
- [概率机器人]()
- [Simultaneous Localization and Mapping for Mobile Robots: Introduction and Methods](http://www.igi-global.com/book/simultaneous-localization-mapping-mobile-robots/66380) by Juan-Antonio Fernández-Madrigal and José Luis Blanco Claraco, 2012
- [Simultaneous Localization and Mapping: Exactly Sparse Information Filters ](http://www.worldscientific.com/worldscibooks/10.1142/8145/)by Zhan Wang, Shoudong Huang and Gamini Dissanayake, 2011
- [An Invitation to 3-D Vision -- from Images to Geometric Models](http://vision.ucla.edu/MASKS/) by Yi Ma, Stefano Soatto, Jana Kosecka and Shankar S. Sastry, 2005
- [Multiple View Geometry in Computer Vision](http://www.robots.ox.ac.uk/~vgg/hzbook/) by Richard Hartley and Andrew Zisserman, 2004
- [Numerical Optimization](http://home.agh.edu.pl/~pba/pdfdoc/Numerical_Optimization.pdf) by Jorge Nocedal and Stephen J. Wright, 1999

### Courses&&Lectures

- [SLAM Tutorial@ICRA 2016](http://www.dis.uniroma1.it/~labrococo/tutorial_icra_2016/)
- [Geometry and Beyond - Representations, Physics, and Scene Understanding for Robotics](http://rss16-representations.mit.edu/) at Robotics: Science and Systems (2016)
- [Robotics - UPenn](https://www.coursera.org/specializations/robotics) on Coursera by Vijay Kumar (2016)
- [Robot Mapping - UniFreiburg](http://ais.informatik.uni-freiburg.de/teaching/ws15/mapping/) by Gian Diego Tipaldi and Wolfram Burgard (2015-2016)
- [Robot Mapping - UniBonn](http://www.ipb.uni-bonn.de/robot-mapping/) by Cyrill Stachniss (2016)
- [Introduction to Mobile Robotics - UniFreiburg](http://ais.informatik.uni-freiburg.de/teaching/ss16/robotics/) by Wolfram Burgard, Michael Ruhnke and Bastian Steder (2015-2016)
- [Computer Vision II: Multiple View Geometry - TUM](http://vision.in.tum.de/teaching/ss2016/mvg2016) by Daniel Cremers ( Spring 2016)
- [Advanced Robotics - UCBerkeley](http://www.cs.berkeley.edu/~pabbeel/) by Pieter Abbeel (Fall 2015)
- [Mapping, Localization, and Self-Driving Vehicles](https://www.youtube.com/watch?v=x5CZmlaMNCs) at CMU RI seminar by John Leonard (2015)
- [The Problem of Mobile Sensors: Setting future goals and indicators of progress for SLAM](http://ylatif.github.io/movingsensors/) sponsored by Australian Centre for Robotics and Vision (2015)
- [Robotics - UPenn](https://alliance.seas.upenn.edu/~meam620/wiki/index.php?n=Main.HomePage) by Philip Dames and Kostas Daniilidis (2014)
- [Autonomous Navigation for Flying Robots](http://vision.in.tum.de/teaching/ss2014/autonavx) on EdX by Jurgen Sturm and Daniel Cremers (2014)
- [Robust and Efficient Real-time Mapping for Autonomous Robots](https://www.youtube.com/watch?v=_W3Ua1Yg2fk) at CMU RI seminar by Michael Kaess (2014)
- [KinectFusion - Real-time 3D Reconstruction and Interaction Using a Moving Depth Camera](https://www.youtube.com/watch?v=bRgEdqDiOuQ) by David Kim (2012)

### Code

1. [ORB-SLAM](https://github.com/raulmur/ORB_SLAM)
2. [LSD-SLAM](https://github.com/tum-vision/lsd_slam)
3. [ORB-SLAM2](https://github.com/raulmur/ORB_SLAM2)
4. [DVO: Dense Visual Odometry](https://github.com/tum-vision/dvo_slam)
5. [SVO: Semi-Direct Monocular Visual Odometry](https://github.com/uzh-rpg/rpg_svo)
6. [G2O: General Graph Optimization](https://github.com/RainerKuemmerle/g2o)
7. [RGBD-SLAM](https://github.com/felixendres/rgbdslam_v2)

| Project                                                      | Language | License                    |
| ------------------------------------------------------------ | -------- | -------------------------- |
| [COSLAM](http://drone.sjtu.edu.cn/dpzou/project/coslam.php)  | C++      | GNU General Public License |
| [DSO-Direct Sparse Odometry](https://github.com/JakobEngel/dso) | C++      | GPLv3                      |
| [DTSLAM-Deferred Triangulation SLAM](https://github.com/plumonito/dtslam) | C++      | modified BSD               |
| [LSD-SLAM](https://github.com/tum-vision/lsd_slam/)          | C++/ROS  | GNU General Public License |
| [MAPLAB-ROVIOLI](https://github.com/ethz-asl/maplab)         | C++/ROS  | Apachev2.0                 |
| [OKVIS: Open Keyframe-based Visual-Inertial SLAM](https://github.com/ethz-asl/okvis) | C++      | BSD                        |
| [ORB-SLAM](https://github.com/raulmur/ORB_SLAM2)             | C++      | GPLv3                      |
| [REBVO - Realtime Edge Based Visual Odometry for a Monocular Camera](https://github.com/JuanTarrio/rebvo) | C++      | GNU General Public License |
| [SVO semi-direct Visual Odometry](https://github.com/uzh-rpg/rpg_svo) | C++/ROS  | GNU General Public License |
