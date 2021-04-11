# Task Definitions and Related Tasks
* **Motion Segmentation:** pixel-wise classification of the scene to moving/static, and its extension to instance-wise segmentation.
* **Zero-shot Video Object Segmentation:** Segmentation of visual and motion salient objects in a video sequence as defined on DAVIS benchmark. Zero-shot, indicates no prior initialization required. It is also called unsupervised-VOS or Primary object segmentation in the literature.
* **Few-shot Video Object Segmentation:** Tracking the segmented objects in a video sequence using an initialization mask. Few/One-shot indicates the need for an initialization for the tracking method, and is also called semi-supervised-VOS in the literature.

Each of these tasks have methods that are trained **fully supervised** and **self supervised**. Each of them as well can be categorized into **pixel-wise** or **instance-wise** segmentation. I prefer to use the term Zero-shot-VOS instead of Unsupervised-VOS as it can be ambiguous whether it indicates no labelled training data or just no initialization in the video sequence. I am mainly focusing on motion segmentation and its related zero-shot segmentation task papers.

# Zero-shot Video Object Segmentation
## Datasets and Benchmarks

* SegTrack V2
* DAVIS:
    * Pixel-wise segmentation: 2016 Unsupervised Benchmark
    * Instance-wise segmentation: 2017 Unsupervised Benchmark (using the 2019 paper with updated unsupervised segmentation definition and annotations)

## Methods

### Fully Supervised

#### Pixel-wise Segmentation
 * MPNet
 * FusionSeg
 * LVO
 * MotAdapt
 * COSNet
 * Anchor Diffusion
 * MatNet
 * Epo-Net

#### Instance-wise Segmentation
* RVOS
* AGS

### Self Supervised

#### Instance-wise Segmentation
* MUG-W

# Deep Motion Segmentation in AD 

## Datasets and Benchmarks
* [City-KITTI-Motion](http://deepmotion.cs.uni-freiburg.de/)
* [KITTIMoSeg](http://webdocs.cs.ualberta.ca/~vis/kittimoseg/)
* [KITTIMoSeg Extended](https://sites.google.com/view/fusemodnet)
* [VCAS Benchmark - Motion Segmentation Track](https://msiam.github.io/vca/)


## Methods
### Fully Supervised
#### Pixel-wise Segmentation
* SMSNet - **IROS'17** \[ [Paper](https://ieeexplore.ieee.org/abstract/document/8202211/), [Code](https://github.com/deepmotionseg/SMSnet) \]
* MODNet - **NeuripsW'17, ITSC'18** \[ [Paper](https://arxiv.org/abs/1709.04821) \]
* Real-time Motion Segmentation - **IROS'18** \[ [Paper](https://ieeexplore.ieee.org/document/8594088) \]
* FuseMODNet - **ICCVW'19**  \[ [Paper](https://arxiv.org/abs/1910.05395) \]

#### Instance-wise Segmentation
* InstanceMotSeg - **NeuripsW'20** \[ [Paper](https://ml4ad.github.io/files/papers2020/Real-time%20Semantic%20and%20Class-agnostic%20Instance%20Segmentation%20in%20Autonomous%20Driving.pdf) \]
* Video Class Agnostic Segmentation - **Arxiv** \[ [Paper](https://arxiv.org/abs/2103.11015), [Code](https://github.com/MSiam/video_class_agnostic_segmentation) \]

### Self Supervised
* SFMNet \[ [Paper](https://arxiv.org/abs/1704.07804) \]
* Competitive Collaboration Framework \[ [Paper](https://arxiv.org/pdf/1805.09806.pdf) \]

#### Instance-wise Segmentation
* Instance-wise Motion and Depth \[ [Paper](https://arxiv.org/abs/1912.09351) \]

If you want to add your paper you can create an issue.
