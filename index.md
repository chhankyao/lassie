LASSIE: Learning Articulated Shape from Sparse Image Ensemble via 3D Part Discovery (NeurIPS 2022)


<p style="text-align: center;">
<a href="https://www.chhankyao.com/" style="color: ##6495ED"> Chun-Han Yao </a>
	&emsp;
<a href="https://hfslyc.github.io" style="color: ##6495ED"> Wei-Chih Hung </a>
	&emsp;
<a href="http://people.csail.mit.edu/yzli/" style="color: ##6495ED"> Yuanzhen Li </a>
	&emsp;
<a href="http://people.csail.mit.edu/mrub/" style="color: ##6495ED"> Michael Rubinstein </a>
</p>

<p style="text-align: center;">
<a href="http://faculty.ucmerced.edu/mhyang/" style="color: ##6495ED"> Ming-Hsuan Yang </a>
	&emsp;
<a href="http://varunjampani.github.io" style="color: ##6495ED"> Varun Jampani </a>
</p>


## Abstract

Creating high-quality articulated 3D models of animals is challenging either via manual creation or using 3D scanning tools. 
Therefore, techniques to reconstruct articulated 3D objects from 2D images are crucial and highly useful. 
In this work, we propose a practical problem setting to estimate 3D pose and shape of animals given only a few (10-30) in-the-wild images of a particular animal species (say, horse). 
Contrary to existing works that rely on pre-defined template shapes, we do not assume any form of 2D or 3D ground-truth annotations, nor do we leverage any multi-view or temporal information. 
Moreover, each input image ensemble can contain animal instances with varying poses, backgrounds, illuminations, and textures. 
Our key insight is that 3D parts have much simpler shape compared to the overall animal and that they are robust w.r.t. animal pose articulations. 
Following these insights, we propose LASSIE, a novel optimization framework which discovers 3D parts in a self-supervised manner with minimal user intervention. 
A key driving force behind LASSIE is the enforcing of 2D-3D part consistency using self-supervisory deep features. 
Experiments on Pascal-Part and self-collected in-the-wild animal datasets demonstrate considerably better 3D reconstructions as well as both 2D and 3D part discovery compared to prior arts.


## Framework

<center>
<figure>
    <div id="projectid">
    <img src="https://chhankyao.github.io/lassie/figures/cover.png" width="900px" />
    </div>
    <br />
    <figcaption>
    </figcaption>
</figure>
</center>

Given sparse images of an articulated class and a generic 3D skeleton, we optimize the shared skeleton and neural parts as well as the instance-specific camera viewpoint and bone transformations. Our method is able to produce high-quality outputs without any pre-defined shape model or instance-specific annotations. The part-based representation also allows applications like animation and texture or pose transfer.


## Example outputs

<p float="center">
    <img src="https://chhankyao.github.io/lassie/figures/proc_5.png" width="20%" />
    <img src="https://chhankyao.github.io/lassie/figures/part_5.gif" width="20%" /> 
    <img src="https://chhankyao.github.io/lassie/figures/text_5.gif" width="20%" />
    <img src="https://chhankyao.github.io/lassie/figures/animate_5.gif" width="20%" />
</p>
<p float="center">
    <img src="https://chhankyao.github.io/lassie/figures/proc_22.png" width="20%" />
    <img src="https://chhankyao.github.io/lassie/figures/giraffe_part_22.gif" width="20%" /> 
    <img src="https://chhankyao.github.io/lassie/figures/giraffe_text_22.gif" width="20%" />
    <img src="https://chhankyao.github.io/lassie/figures/giraffe_animate_22.gif" width="20%" />
</p>
<p float="center">
    <img src="https://chhankyao.github.io/lassie/figures/proc_21.png" width="20%" />
    <img src="https://chhankyao.github.io/lassie/figures/part_21.gif" width="20%" /> 
    <img src="https://chhankyao.github.io/lassie/figures/text_21.gif" width="20%" />
    <img src="https://chhankyao.github.io/lassie/figures/animate_21.gif" width="20%" />
</p>

(Left to right: input images, part outputs, textured outputs, animations)



## Animations

<p float="center">
    <img src="https://chhankyao.github.io/lassie/figures/proc_3.png" width="20%" />
    <img src="https://chhankyao.github.io/lassie/figures/mask_pred_3.png" width="20%" /> 
    <img src="https://chhankyao.github.io/lassie/figures/video_part_3.gif" width="20%" />
    <img src="https://chhankyao.github.io/lassie/figures/video_text_3_side.gif" width="20%" />
</p>
<p float="center">
    <img src="https://chhankyao.github.io/lassie/figures/proc_5.png" width="20%" />
    <img src="https://chhankyao.github.io/lassie/figures/mask_pred_5.png" width="20%" /> 
    <img src="https://chhankyao.github.io/lassie/figures/video_part_5.gif" width="20%" />
    <img src="https://chhankyao.github.io/lassie/figures/video_text_5_side.gif" width="20%" />
</p>

(Left to right: input images, predicted masks, part animations, textured animations)



## Paper

- Paper: [PDF](https://arxiv.org/pdf/2207.03434.pdf)

- Supplementary: [PDF](https://github.com/chhankyao/papers/blob/main/arxiv_lassie_supp.pdf)


## Video

<center>
<iframe width="800" height="500" src="https://www.youtube.com/embed/MhQaHzC4Sn0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</center>


## Bibtex

```markdown
@inproceedings{yao2022lassie,
  title={LASSIE: Learning Articulated Shape from Sparse Image Ensemble via 3D Part Discovery},
  author={Yao, Chun-Han and Hung, Wei-Chih and Rubinstein, Michael and Lee, Yuanzhen and Jampani, Varun and Yang, Ming-Hsuan},
  booktitle={Conference on Neural Information Processing Systems},
  year={2022}
}
```
