# HSOD-BIT-V2 AAAI-25

## Paper

The paper "HSOD-BIT-V2: A New Challenging Benchmarkfor Hyperspectral Salient Object Detection" has been accepted at `AAAI 2025`. Paper will be avaliable soon.

#### Abstract
Salient Object Detection (SOD) is crucial in computer vision, yet RGB-based methods face limitations in challenging scenes, such as small objects and similar color features. Hyperspectral images provide a promising solution for more accurate Hyperspectral Salient Object Detection (HSOD) by abundant spectral information, while HSOD methods are hindered by the lack of extensive and available datasets. In this context, we introduce HSOD-BIT-V2, the largest and most challenging HSOD benchmark dataset to date. Five distinct challenges focusing on small objects and foreground-background similarity are designed to emphasize spectral advantages and real-world complexity. To tackle these challenges, we propose Hyper-HRNet, a high-resolution HSOD network. Hyper-HRNet effectively extracts, integrates, and preserves effective spectral information while reducing dimensionality by capturing the self-similar spectral features. Additionally, it conveys fine details and precisely locates object contours by incorporating comprehensive global information and detailed object saliency representations. Experimental analysis demonstrates that Hyper-HRNet outperforms existing models, especially in challenging scenarios.

![overall](https://github.com/QYH-BIT/HSOD-BIT-V2/blob/main/figure/moxing.jpg)

## Dataset

HSOD-BIT-V2 is a new and the largest, most challenging HSOD benchmark dataset to date, now released. Our previous work, the first large-scale, high-quality HSOD benchmark dataset HOSD-BIT (V1), is also available for access on [DMSSN](https://github.com/q2479036243/DMSSN/tree/main).

#### Description

HSOD-BIT-V2 overcomes limitations in scale, quality, and challenge of current datasets, aimed at leveraging the advantages of spectral and showcase the complexity of real-world scenarios. Building upon [HOSD-BIT (V1)](https://github.com/q2479036243/DMSSN/tree/main), it further extends the data scale and diversity of backgrounds while introducing challenge attributes. This dataset provides pixel-level manual annotations for `500 hyperspectral data cubes` and generates corresponding pseudo-color images. Each data cube contains `200 bands` covering spectral information from visible light to near-infrared bands, with a spatial resolution of up to `1240×1680 pixels`. In addition to common scenes, this dataset covers `8 natural backgrounds` and `5 challenge attributes` with diverse and challenging data, highlighting small objects and foreground-background similarity.

![dataset](https://github.com/QYH-BIT/HSOD-BIT-V2/blob/main/figure/dataset.jpg)

##### Challenge Attributes
To evaluate HSOD method thoroughly, we categorize challenges into 5 attributes: Complex Background (CB), Color Similarity (CS), High Dynamic Range (HDR), Small Object (SO), and Material Similarity (MS), detailed in table below. Each challenging data is classified into one or more attributes based on its specific characteristics.

| Challenge Attribute  | Description |
| ------------- | ------------- |
| CB  |  Complex Background (282): The color and spectral characteristics of the background are complex  |
| CS  |  Color Similarity (160): The object and background color features are similar, but spectral features are different  |
| HDR |  High Dynamic Range (134): The light intensity in the scene has a high dynamic range, including overexposure and shadow scenes  |
| SO  |  Small Object (185): The object size is very small, occupying less than 1\% of the image area  |
| MS  |  Material Similarity (24): Foreground and background materials are similar, and their spectral curves are close  |

##### Natural Backgrounds
HSOD-BIT-V2 comprises 8 natural backgrounds around university campus and surrounding areas under different weather conditions: lawn (18%), fallen leaves (5%), path (21%), wall (19%), playgrounds (10%), sky (9%), snowfield (2%), and other natural settings. Notably, snowfield and fallen leaves scenes are introduced to the field for `the first time`.  Each scene type presents a variety of scenarios, characterized by different seasons, lighting conditions, and background clusters, as depicted below.

![scenes](https://github.com/QYH-BIT/HSOD-BIT-V2/blob/main/figure/scenes.jpg)

#### Download: 

Dataset is avaliable at [HSOD-BIT-V2](https://pan.baidu.com/s/1I8Ysfi7LB5ujuuedV2PwOg?pwd=tftf).

## Important Update

For more efficient data storage, the hyperspectral image data format is changed from the original MAT to H5.

```python
import h5py
def dataload(path):
    data = h5py.File(path, "r")['dataset'][:]
    return data
```

## Citation

If you use this benchmark in your research, please cite this project.

```
Paper will be coming soon.
```

