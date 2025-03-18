# HSOD-BIT-V2

## Paper

The paper "HSOD-BIT-V2: A New Challenging Benchmarkfor Hyperspectral Salient Object Detection" has  been published at AAAI 2025.

#### Abstract
Salient Object Detection (SOD) is crucial in computer vision, yet RGB-based methods face limitations in challenging scenes, such as small objects and similar color features. Hyperspectral images provide a promising solution for more accurate Hyperspectral Salient Object Detection (HSOD) by abundant spectral information, while HSOD methods are hindered by the lack of extensive and available datasets. In this context, we introduce HSOD-BIT-V2, the largest and most challenging HSOD benchmark dataset to date. Five distinct challenges focusing on small objects and foreground-background similarity are designed to emphasize spectral advantages and real-world complexity. To tackle these challenges, we propose Hyper-HRNet, a high-resolution HSOD network. Hyper-HRNet effectively extracts, integrates, and preserves effective spectral information while reducing dimensionality by capturing the self-similar spectral features. Additionally, it conveys fine details and precisely locates object contours by incorporating comprehensive global information and detailed object saliency representations. Experimental analysis demonstrates that Hyper-HRNet outperforms existing models, especially in challenging scenarios.

![overall](https://github.com/QYH-BIT/HSOD-BIT-V2/blob/main/figure/moxing.jpg)

## Dataset

HSOD-BIT-V2 overcomes limitations in scale, quality, and challenge of current datasets. It surpassing existing HS-SOD and HSOD-BIT, with `500 HSIs`,  `1240×1680 spatial resolutions`, and `200 spectral bands`. 
Unlike HS-SOD, which focuses on common scenes, and HSOD-BIT, with limited challenging data, HSOD-BIT-V2 covers 8 natural backgrounds with diverse and challenging data, highlighting small objects and foreground-background similarity.

HSOD-BIT-V2, the largest and most challenging hyperspectral saliency object detection benchmark dataset to date, has been released. Our previous work, HOSD-BIT (V1), has been released at [DMSSN](https://github.com/q2479036243/DMSSN/tree/main).

#### Description

HSOD-BIT-V2 overcomes limitations in scale, quality, and challenge of current datasets. It surpassing existing HS-SOD and HSOD-BIT, with `500 HSIs`,  `1240×1680 spatial resolutions`, and `200 spectral bands`. 
Unlike HS-SOD, which focuses on common scenes, and HSOD-BIT, with limited challenging data, HSOD-BIT-V2 covers 8 natural backgrounds with diverse and challenging data, highlighting small objects and foreground-background similarity.
HSOD-BIT is the first large-scale, high-quality benchmark dataset for hyperspectral salient object detection, aimed at leveraging the advantages of spectral information to achieve higher precision in salient object detection tasks. Addressing the data requirements of contemporary deep learning models, this dataset provides pixel-level manual annotations for 319 hyperspectral data cubes and generates corresponding pseudo-color images. Each data cube contains 200 bands covering spectral information from visible light to near-infrared bands, with a spatial resolution of up to 1240×1680 pixels. In addition to conventional scenes, this dataset also specifically gathers challenging data to reflect the complexity of the real world, such as similar background interference, uneven lighting, overexposure, and other challenging scenarios. This further enhances the practicality and evaluation capabilities of the dataset.

![图片1](https://github.com/QYH-BIT/HSOD-BIT-V2/blob/main/figure/dataset.jpg)

#### Download: 


Dataset is avaliable at [https://pan.baidu.com/s/1I8Ysfi7LB5ujuuedV2PwOg?pwd=tftf](https://pan.baidu.com/s/1I8Ysfi7LB5ujuuedV2PwOg?pwd=tftf).

