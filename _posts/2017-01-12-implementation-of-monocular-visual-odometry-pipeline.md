---
ID: 710
post_title: Implementation of Monocular Visual Odometry Pipeline
author: Dongho Kang
date: 2017-01-12 23:13:35
post_excerpt: ""
layout: post
permalink: http://eastskykang.net/2017/01/12/implementation-of-monocular-visual-odometry-pipeline/
published: false
---
<p>This project is from the course <a href="http://rpg.ifi.uzh.ch/teaching.html">"Vision Algorithms for Mobile Robotics"</a> of ETH Zurich in Autumn 2016.</p>

<p>The goal of the project is implementing a monocular visual odometry pipeline. </p>

<p>Jihwan Youn, Dongho Kang and Jaeyoung Lim contributed to the project and the course was instructed by <a href="http://rpg.ifi.uzh.ch/people_scaramuzza.html">Prof. Davide Scaramuzza</a></p>


<hr>
<h2>Overview</h2>

<p>Our Visual Odometry pipeline(VO pipeline) consists of initialization, continuous operation, and bundle adjustment as shown in figure 1. A loop closure module was also implemented but excluded from the experimental result.</p>

<figure>
	<img src="http://eastskykang.net/wp-content/uploads/2017/06/Overview.png" alt="" width="1429" height="558" class="alignnone size-full wp-image-716" />
	<figcaption align="bottom">Figure 1: Overview of the visual odometry pipeline.</figcaption>
</figure>

<p>The initialization module outputs the initial pose and landmarks based on the manually selected two images, I0 and I1. The process frame uses the pre- viously estimated pose and landmarks to continuously estimate the current pose.</p>

<p> Additionally, VO pipeline performs window-based bundle adjustment to optimize the poses and the landmarks by minimizing the reprojection error in a nonlinear fashion.</p>

<p> A loop closure feature was added by storing the landmark history. However, due to the poor robustness of place recognition function, the loop closure feature is not demonstrated properly in the demo videos</p>


<hr>
<h2>Demos</h2>

<p>The code was implemented in MATLAB language and was tested in MATLAB R2016b version. Four datasets were used to assess the performance of our VO pipeline.</p>


<br>
<h3>KITTI dataset</h3>

<table style="width:100%">
	<tr>
		<td width="50%">
			<iframe width="100%" height="100%" src="https://www.youtube.com/embed/dS4KoISoAcE" allowfullscreen></iframe>
		</td>
		<td width="50%">
			<img src="http://eastskykang.net/wp-content/uploads/2017/06/Results_KITTI.png" alt="" width="100%" height="100%" class="alignnone size-full wp-image-721" />
		</td>
	</tr>
</table>

<p><a href="http://www.cvlibs.net/datasets/kitti/">KITTI dataset</a> shows significant scale drift without the bundle adjustment implementation. After bundle adjustment, the VO pipeline is robust enough to run to the end of the dataset.</p>


<br>
<h3>MALAGA dataset</h3>

<table style="width:100%">
	<tr>
		<td width="50%">
			<iframe width="100%" height="100%" src="https://www.youtube.com/embed/3fxA7I47CuM" allowfullscreen></iframe>
		</td>
		<td width="50%">
			<img src="http://eastskykang.net/wp-content/uploads/2017/06/Results_MALAGA.png" alt="" width="100%" height="100%" class="alignnone size-full wp-image-722" />
		</td>
	</tr>
</table>

<p><a href="http://www.mrpt.org/MalagaUrbanDataset">MALAGA dataset</a> shows scale drift even after bundle adjustment. This is thought to be from the large variations of landmark distance from the camera.</p>


<br>
<h3>PARKING dataset</h3>

<table style="width:100%">
	<tr>
		<td width="50%">
			<iframe width="100%" height="100%" src="https://www.youtube.com/embed/WfOTkpfoyzY" allowfullscreen></iframe>
		</td>
		<td width="50%">
			<img src="http://eastskykang.net/wp-content/uploads/2017/06/Results_Parking.png" alt="" width="100%" height="100%" class="alignnone size-full wp-image-723" />
		</td>
	</tr>
</table>

<p>Parking dataset shows robust performance even though the camera is facing the right angle to the direction of travel. Parking has an accumulative error as the dataset has no loop even though running bundle adjustment.</p>

<br>
<h3>SEOUL dataset</h3>

<table style="width:100%">
	<tr>
		<td width="50%">
			<iframe width="100%" height="100%" src="https://www.youtube.com/embed/Y0lDwR3oK0w" allowfullscreen></iframe>
		</td>
		<td width="50%">
			<img src="http://eastskykang.net/wp-content/uploads/2017/06/Results_OWN.png" alt="" width="100%" height="100%" class="alignnone size-full wp-image-726" />
		</td>
	</tr>
</table>


<p>A custom dataset was constructed to verify that the visual odometry pipeline is robust enough to work in various environments. The custom dataset is based on 360 sequence of images taken from an iPhone 6s. While taking the images the camera had a fixed focal length and the images were down sam- pled by a factor of 0.2 for computational issues in calibrating the camera and rectifying images. Images were filmed in a narrow alley in Seoul, Republic of Korea in December 27th 2016.</p>

<p>The successful trajectory estimation of the VO pipeline in a narrow alley with large variations of landmark distance and illumination changes shows robust performance of the VO pipeline.</p>


<hr>
<h2>Conclusion</h2>

We successfully implemented a fully working and robust monocular visual odometry pipeline as well as the additional features as the following:

<ul>
	<li>An appealing visualization was implemented including keypoint tracking information, camera heading and trajectory in each frame. A full landmark and trajectory visualization is also implemented.</li>
	<li>Many ideas for improving the performance of the VO pipeline.</li>
	<li>Refined estimated pose by minimizing reprojection error.</li>
	<li>VO pipeline verification on a custom recorded dataset.</li>
	<li>Full bundle adjustment(motion and structure)</li>
	<li>Not fully working but implemented loop closure module using place recognition.</li>
</ul>
