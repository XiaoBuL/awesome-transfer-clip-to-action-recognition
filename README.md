# Awesome Transfer CLIP to Video Recognition: [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
A curated list of vision-language model based video action recognition resources, inspired by [awesome-computer-vision](https://github.com/jbhuang0604/awesome-computer-vision).

## Contents
 - [Dataset for VLM pretraining and video action recognition](#Dataset-for-VLM-pretraining-and-video-action-recognition)
 - [SOTA Result On Different Datasets And Task Settings](#SOTA-Result-On-Different-Datasets-And-Task-Settings)
 - [Related Survey](#Related-Survey)
 - [Pretrained Vision-Language Model](#Pretrained-Vision-Language-Model)
 - [Adaption From Image-Language Model To Video Model](#Adaption-From-Image-Language-Model-To-Video-Model)
 - [VLM-Based Few-Shot Video Action Recognition](#VLM-Based-Few-Shot-Video-Action-Recognition)
 - 

## Dataset for VLM pretraining and video action recognition
* [Video Dataset Overview from Antoine Miech](https://www.di.ens.fr/~miech/datasetviz/)
* [HACS](http://hacs.csail.mit.edu/)
* [Moments in Time](http://moments.csail.mit.edu/), [paper](http://moments.csail.mit.edu/data/moments_paper.pdf)
* [AVA](https://research.google.com/ava/), [paper](https://arxiv.org/abs/1705.08421), [[INRIA web]](http://thoth.inrialpes.fr/ava/getava.php) for missing videos
* [Kinetics](https://deepmind.com/research/open-source/open-source-datasets/kinetics/), [paper](https://arxiv.org/pdf/1705.07750.pdf), [download toolkit](https://github.com/activitynet/ActivityNet/tree/master/Crawler/Kinetics)
* [OOPS](https://oops.cs.columbia.edu/data/) - A dataset of unintentional action, [paper](https://arxiv.org/abs/1911.11206)
* [COIN](https://coin-dataset.github.io/) - a large-scale dataset for comprehensive instructional video analysis, [paper](https://arxiv.org/abs/1903.02874)
* [YouTube-8M](https://research.google.com/youtube8m/), [technical report](https://arxiv.org/abs/1609.08675)
* [YouTube-BB](https://research.google.com/youtube-bb/), [technical report](https://arxiv.org/pdf/1702.00824.pdf)
* [DALY](http://thoth.inrialpes.fr/daly/) Daily Action Localization in Youtube videos. Note: Weakly supervised action detection dataset. Annotations consist of start and end time of each action, one bounding box per each action per video.
* [20BN-JESTER](https://www.twentybn.com/datasets/jester), [20BN-SOMETHING-SOMETHING](https://www.twentybn.com/datasets/something-something)
* [ActivityNet](http://activity-net.org/) Note: They provide a download script and evaluation code [here](https://github.com/activitynet) .
* [Charades](http://allenai.org/plato/charades/)
* [Charades-Ego](https://prior.allenai.org/projects/charades-ego), [paper](https://arxiv.org/pdf/1804.09626.pdf) - First person and third person video aligned dataset
* [EPIC-Kitchens](https://epic-kitchens.github.io/), [paper](https://arxiv.org/abs/1804.02748) - First person videos recorded in kitchens. Note they provide download scripts and a python library [here](https://github.com/epic-kitchens)
* [Sports-1M](http://cs.stanford.edu/people/karpathy/deepvideo/classes.html) - Large scale action recognition dataset.
* [THUMOS14](http://crcv.ucf.edu/THUMOS14/) Note: It overlaps with [UCF-101](http://crcv.ucf.edu/data/UCF101.php) dataset.
* [THUMOS15](http://www.thumos.info/home.html) Note: It overlaps with [UCF-101](http://crcv.ucf.edu/data/UCF101.php) dataset.
* [HOLLYWOOD2](http://www.di.ens.fr/~laptev/actions/hollywood2/): [Spatio-Temporal annotations](https://staff.fnwi.uva.nl/p.s.m.mettes/index.html#data)
* [UCF-101](http://crcv.ucf.edu/data/UCF101.php), [annotation provided by THUMOS-14](http://crcv.ucf.edu/ICCV13-Action-Workshop/index.files/UCF101_24Action_Detection_Annotations.zip), and [corrupted annotation list](https://github.com/jinwchoi/Jinwoo-Computer-Vision-and-Machine-Learing-papers-to-read/blob/master/UCF101_Spatial_Annotation_Corrupted_file_list),  [UCF-101 corrected annotations](https://github.com/gurkirt/corrected-UCF101-Annots) and [different version annotaions](https://github.com/jvgemert/apt). And there are also some pre-computed spatiotemporal action detection [results](https://drive.google.com/drive/folders/0B-LzM05qEdk0aG5pTE94VFI1SUk)
* [UCF-50](http://crcv.ucf.edu/data/UCF50.php).
* [UCF-Sports](http://crcv.ucf.edu/data/UCF_Sports_Action.php), note: the train/test split link in the official website is broken. Instead, you can download it from [here](http://pascal.inrialpes.fr/data2/oneata/data/ucf_sports/videos.txt).
* [HMDB](http://serre-lab.clps.brown.edu/resource/hmdb-a-large-human-motion-database/)
* [J-HMDB](http://jhmdb.is.tue.mpg.de/)
* [LIRIS-HARL](http://liris.cnrs.fr/voir/activities-dataset/)
* [KTH](http://www.nada.kth.se/cvap/actions/)
* [MSR Action](https://www.microsoft.com/en-us/download/details.aspx?id=52315) Note: It overlaps with [KTH](http://www.nada.kth.se/cvap/actions/) datset.
* [Sports Videos in the Wild](http://cvlab.cse.msu.edu/project-svw.html)
* [NTU RGB+D](https://github.com/shahroudy/NTURGB-D)
* [Mixamo Mocap Dataset](http://mocap.cs.cmu.edu/)
* [UWA3D Multiview Activity II Dataset](http://staffhome.ecm.uwa.edu.au/~00053650/databases.html)
* [Northwestern-UCLA Dataset](https://users.eecs.northwestern.edu/~jwa368/my_data.html)
* [SYSU 3D Human-Object Interaction Dataset](http://www.isee-ai.cn/~hujianfang/ProjectJOULE.html)
* [MEVA (Multiview Extended Video with Activities) Dataset](http://mevadata.org)

## SOTA Result On Different Datasets And Task Settings 

## Related Survey

## Pretrained Vision-Language Model
### Image-Language Model
### Video-Language Model

## Adaption From Image-Language Model To Video Model
### Pure Adapter-Based
### Pure Prompt-Based
### Mixture Of Adapter And Prompt
### Full-Finetuning-Based

## VLM-Based Few-Shot Video Action Recognition

#### Useful Code Repos on Video Representation Learning
* [[3D ResNet PyTorch]](https://github.com/kenshohara/3D-ResNets-PyTorch)
* [[PyTorch Video Research]](https://github.com/gsig/PyVideoResearch)
* [[M-PACT: Michigan Platform for Activity Classification in Tensorflow]](https://github.com/MichiganCOG/M-PACT)
* [[Inflated models on PyTorch]](https://github.com/hassony2/inflated_convnets_pytorch)
* [[I3D models transfered from Tensorflow to PyTorch]](https://github.com/hassony2/kinetics_i3d_pytorch)
* [[A Two Stream Baseline on Kinectics dataset]](https://github.com/gurkirt/2D-kinectics)
* [[MMAction]](https://github.com/open-mmlab/mmaction)
* [[MMAction2]](https://github.com/open-mmlab/mmaction2)
* [[PySlowFast]](https://github.com/facebookresearch/slowfast)
* [[Decord]](https://github.com/dmlc/decord) Efficient video reader for python
* [[I3D models converted from Tensorflow to Core ML]](https://github.com/lukereichold/VisualActionKit)
* [[Extract frame and optical-flow from videos, #docker]](https://github.com/epic-kitchens/epic-kitchens-100-annotations/blob/master/README.md#erratum)
* [[NVIDIA-DALI, video loading pipelines]](https://docs.nvidia.com/deeplearning/dali/user-guide/docs/examples/sequence_processing/video/video_reader_label_example.html)
* [[NVIDIA optical-flow SDK]](https://developer.nvidia.com/opticalflow-sdk)

### Miscellaneous
* [What and How Well You Performed? A Multitask Learning Approach to Action Quality Assessment](https://arxiv.org/pdf/1904.04346.pdf) - P. Parma and B. T. Morris. CVPR2019.
* [PathTrack: Fast Trajectory Annotation with Path Supervision](http://openaccess.thecvf.com/content_ICCV_2017/papers/Manen_PathTrack_Fast_Trajectory_ICCV_2017_paper.pdf) - S. Manen et al., ICCV2017.
* [CortexNet: a Generic Network Family for Robust Visual Temporal Representations](https://arxiv.org/pdf/1706.02735.pdf) A. Canziani and E. Culurciello - arXiv2017. [[code]](https://github.com/atcold/pytorch-CortexNet) [[project web]](https://engineering.purdue.edu/elab/CortexNet/)
* [Slicing Convolutional Neural Network for Crowd Video Understanding](http://www.ee.cuhk.edu.hk/~jshao/papers_jshao/jshao_cvpr16_scnn.pdf) - J. Shao et al, CVPR2016. [[code]](https://github.com/amandajshao/Slicing-CNN)
* [Two-Stream (RGB and Flow) pretrained model weights](https://github.com/craftGBD/caffe-GBD/tree/master/models/action_recognition)

## Licenses
License

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Jinwoo Choi](https://sites.google.com/site/jchoivision/) has waived all copyright and related or neighboring rights to this work.

## Contributing
Please read the [contribution guidelines](contributing.md). Then please feel free to send me [pull requests](https://github.com/jinwchoi/Action-Recognition/pulls) or email (jinchoi@vt.edu) to add links.
