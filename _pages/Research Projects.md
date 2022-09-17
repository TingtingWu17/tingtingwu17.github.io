---
title: "Research Projects"
permalink: /_pages/research-projects/
layout: single
author_profile: true
classes: wide
---
# <span style="color:black; font-family:Comic Sans MS;font-size: 30px;">Single-Molecule Orientation Localization Microscopy</span>

Traditional fluorescence imaging measures the spatial structure of targets by focusing on measuring __where__ lights come from.  
In my projects, I measure both __where__ lights come from and the __shape__ of lights. This measurement gives us information on how fluorescent emitters interact with imaging targets, e.g. the __binding direction (3D orientation)__ of fluorescence probes to target structure.

<!-- <figure>
  <img src="{{ '_pages/amyloid_example.png' | relative_url }}"  alt="amyloid image">
</figure>
__3D orientations tells the secondary structure of biological samples__
Amyloid fibril is composed with beta sheet structure -->



## <span style="color:teal; font-family:Comic Sans MS;font-size: 25px;">Point spread function engineering</span>

<span style="color:teal; font-family:Comic Sans MS;font-size: 15px;">__Tingting Wu__, Jin Lu, and Matthew D. Lew. Optica (2022). [[Article]](http://dx.doi.org/10.1364/optica.451899) [[Data&Code]](https://doi.org/10.17605/OSF.IO/97GMV) [[Summary video]](/_pages/files/pixOL summary  video.mp4) </span>


In this work, we "ruin" the microscope to generate point spread functions (PSFs) that deviate from the traditional Gaussian pattern.
We designed an optimization algorithm to optimize a phase mask that we will put into the back focal plane of a polarized 4f microscope. __The optimized microscope output PSFs with shapes vary distinctively for fluorescent probes with different orientations and axial positions.__

The optimized microscope enables us to simultaneously measure the 3D position and 3D orientation of fluorescent probes. We reconstructed the shape of a spherical supported lipid bilayer (SLB). All the fluorescent emitters have orientation perpendicular to the spherical surface for SLB with cholesterol, however, once we delete the cholesterol, the SLB becomes more spacious for fluorescent probes to rotate. Therefore, we notice more random orientations for SLB without cholesterol.

<img src="/_pages/files/pixOL one-slide summary3.gif" width="800" height="800" />



## <span style="color:teal; font-family:cursive;font-size: 25px;">Deep-learning based estimation algorithm design</span>

<span style="color:teal; font-family:cursive;font-size: 15px;">__TingtingWu__, Peng Lu†, Md Ashequr Rahman†, Xiao Li†, and Matthew D. Lew. Optics Express (2022). [[Article]](http://dx.doi.org/10.1101/2022.07.31.502237) [[Code]](https://github.com/Lew-Lab/Deep-SMOLM) [[Data]](https://osf.io/x6p8r/). </span>

Using engineered PSF, emitters with different orientations will generate PSFs with different shapes on our camera. In this work, we design a deep-learning-based algorithm to estimate the 3D orientation and 2D position from the noise-crrupted PSFs. 

We smartly designed our network to handle this high dimensional estimation challenge: 1) __we encode the 3D orientation and 2D position orthogonally__ into the spatial position and intensity of the gaussian patterns on the output images; 2) __we leverage the forward model__ to output the orientational second moments instead of the three orientation angles.  

Deep-SMOLM outwins the iterative estimation algorithm in terms of 1) handling overlapped emitters, 2) being close to optimal precision due to its ability to output global minima instead of sticking in the local minima, and 3) ~10 times faster estimation speed.

<img src="/_pages/files/Deep-SMOLM one slide summary.jpg" width="800" height="800" />


## <span style="color:teal; font-family:cursive;font-size: 25px;">Adaptive microscopy design</span>

<span style="color:teal; font-family:cursive;font-size: 15px;"> ongoing project, more details will be added later </span>

Most of the microsocpes are fixed once built. In this project, we configure the strucuture of the microscope to adapt to the current measurement to achieve better imaging. 


## <span style="color:teal; font-family:cursive;font-size: 25px;">Mapping dynamic and heterogeneous 6D network of bio-condensates </span>
<span style="color:teal; font-family:cursive;font-size: 15px;"> paper is under written, more details will be added later </span>

Biomolecular condensates are formed by proteins and nucleic acids and are liquid-like, membraneless structures that play critical roles in various cellular activities such as gene regulation, cell-cell signaling, and actin assembly. The mechanisms of how condensates form and dissolve, which can be viewed as the network architecture formed by interactions between proteins, are not well understood. 

In this project, we use single molecule techniques to study the internal archetecture of biomolecular condensates.



## <span style="color:teal; font-family:cursive;font-size: 25px;">Evaluation metric design based on information theory </span>

<span style="color:teal; font-family:cursive;font-size: 15px;">Tianben Ding†, __Tingting Wu__†, Hesam Mazidi, Oumeng Zhang, and Matthew Lew. Optica 7.6
(2020) [[Article]](http://dx.doi.org/10.1364/optica.388157) [[Data&Code]](https://osf.io/pe3qu/?view_only=081206495472426889c1055f21971e9a) [[Summary slide]](/_pages/files/summary page_optica_VUB_TAB.png)</span>


In this project, we developed a metric, termed variance upper bound (VUB), to quickly select the best microscope for single-molecule orientation measurements.
VUB, the global upper bound of Cramér-Rao bound (CRB) for all possible molecular orientations, efficiently quantifies the orientation sensitivity of a point spread function (PSF) ~1000X faster than calculating the average CRB over orientation space. 

VUB enables us to realize that the polarized standard PSF (polar) provides superior measurement precision when molecules are near a refractive index (RI) interface. We then used the polarized standard PSF to measure the 3D orientation and 2D position of Nile red that transiently bind to the amyloid fibril.

<span style="color:black;font-size: 15px;font-family:cursive;" align = "center"> Orientations of indivual Nile reds on amyloid fibril </span>
<img src="/_pages/files/TAB_flyover.gif" width="600" height="600"  />

<span style="color:gray;font-size: 15px;" align="right"> Image credit to Prof. Matthew D. Lew and Dr. Tianben Ding </span>

<!-- <p align = "left">
<p align = "center">
<span style="color:black;font-size: 15px;font-family:cursive;"> Orientations of indivual Nile reds on amyloid fibril </span>
<p align = "left">
<img src="/_pages/files/TAB_flyover.gif" width="800" height="800" />
</p>
<p align = "right">
<span style="color:gray;font-size: 15px;"> Image credit to Prof. Matthew D. Lew and Dr. Tianben Ding </span>
</p> -->




## <span style="color:teal; font-family:cursive;font-size: 25px;">Optical fiber sensor </span>

<span style="color:teal; font-family:cursive;font-size: 15px;">__Tingting Wu__, Linlin Xu, and Xinhai Zhang. Journal of Physics Communications 2.6 (2018), p. 065009. [[Article]](http://dx.doi.org/10.1088/2399-6528/aacb0b).</span>


<img src="/_pages/files/fiber_sensor_image.jpg" align="right" width="500px"/>
In this project, we designed a refractive index sensor by creating U-shaped optical fibers. The interference between the lights in the cladding mode and core mode, the optical fiber show different interference valley for solution with different refractive indexes.

<br clear="left"/>

