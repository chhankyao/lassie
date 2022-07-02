# Learning Articulated Shape from Sparse Image Ensemble via 3D Part Discovery


<p style="text-align: center;">
<a href="https://www.chhankyao.com/" style="color: ##6495ED"> Chun-Han Yao </a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://hfslyc.github.io" style="color: ##6495ED"> Wei-Chih Hung </a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="http://varunjampani.github.io" style="color: ##6495ED"> Varun Jampani </a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="http://faculty.ucmerced.edu/mhyang/" style="color: ##6495ED"> Ming-Hsuan Yang </a>
</p>

<p style="text-align: center;">
<a href="https://www.chhankyao.com/" style="color: ##6495ED"> Michael Rubinstein </a>
&emsp;
<a href="https://hfslyc.github.io" style="color: ##6495ED"> Yuanzhen Li </a>
</p>


## Abstract

Creating high-quality articulated 3D models of animals is challenging either via manual creation or using 3D scanning tools. 
Therefore, techniques to reconstruct articulated 3D objects from 2D images are crucial and highly useful. 
In this work, we propose a practical problem setting of estimating 3D shape and pose of animals given only a few (10-30) in-the-wild images of a particular animal species (say, horse). 
Contrary to existing works that rely on pre-defined template shapes, we do not assume any form of 2D or 3D ground-truth annotations, nor do we assume any multi-view or temporal information. 
Our input image ensemble can have animal instances with varying poses, backgrounds, illuminations and also textures. 
Our key insight is that 3D parts have much more simplistic shapes compared to the overall animal and that the part shapes are robust w.r.t. animal pose articulations. 
Using these insights, we propose LASSIE, a novel optimization framework that discovers 3D parts in a self-supervised manner using minimal user intervention. 
A key driving force behind LASSIE is the enforcing of 2D-3D part consistency using self-supervisory deep features. 
Experiments on Pascal Part and self-collected in-the-wild animal datasets demonstrate considerably better 3D reconstructions as well as both 2D and 3D part discovery compared to prior art.


<center>
<figure>
    <div id="projectid">
    <img src="https://chhankyao.github.io/lassie/figures/cover.png" width="900px" />
    </div>
    <br />
    <figcaption>
	  Given 10-30 images of an articulated class and a generic 3D skeleton, we optimize the shared skeleton and neural parts as well as the instance-specific camera viewpoint and bone transformations. Our method is able to produce high-quality outputs without any pre-defined shape model or instance-specific annotations. The part-based representation also allows applications like texture and pose transfer, animation, etc.
    </figcaption>
</figure>
</center>


## Paper & Code

- Paper [PDF]

- Supplementary [PDF]

- PyTorch Code [Github]


## Video

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/MhQaHzC4Sn0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</center>


## Bibtex
