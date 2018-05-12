## An Innovative Saliency Guided RoI Selection Model for Panoramic Images Compression




|  ![DCC 2018 logo][logo-DCC] | Paper accepted at [2018 Data Compression Conference](http://www.cs.brandeis.edu/~dcc/index.html) Cliff Lodge, Snowbird, UT, Tuesday - Friday, March 27 - 30. |
|:-:|---|

[logo-DCC]: https://github.com/ChunbiaoZhu/DCC-2018/blob/master/logo/DCCbanner_text.png "DCC 2018 logo"




## Abstract

Saliency detection has been an increasingly important tool for ROI selection in image compression. Most previous works on saliency detection are dedicated to conventional images, however, with the rapid development of VR or AR technology, it is becoming more and more important to obtain visual attention for panoramic images. Meanwhile, panoramic images have more potential for improvement in compression performance compared with the conventional case.

In this work, we propose an innovative saliency guided ROI selection model, shown in Fig.1. We first employ a spatial density pattern detection method based on region growing to roughly extract the proposal objects. And the eye fixation model is employed to predict the visual attention, which is inspired by neurobiological mechanisms of the human vision system. Then, the previous saliency information is combined by the maxima normalization to produce the coarse saliency map. Finally, a geodesic distance based refinement is utilized to derive the final saliency map.

Extensive evaluations show the proposed approach outperforms other methods in saliency accuracy especially for panoramic images. Meanwhile, we improve the compression quality of standard JPEG by using a higher bit rate to encode image regions flagged by our model and lower bit rate elsewhere in the image. With our proposed ROI selection model, we improve the compression performance compared with the standard JPEG by 10~35%. To our consideration, this research can also help to figure out the perception characteristics of the human visual system for large-scale visual contents over a wide field of view.

 


## Framework
![QFramework saliency detection](https://github.com/ChunbiaoZhu/DCC-2018/blob/master/images/fig1.png)

## Full Version
Full version can be downloaded in [here](https://www.researchgate.net/publication/324027465_Automatic_Salient_Object_Detection_for_Panoramic_Images_Using_Region_Growing_and_Fixation_Prediction_Model)  or [here](https://arxiv.org/abs/1710.04071)

## Code & Results
1.ROI selection model code is released! You can download in [here](https://github.com/ChunbiaoZhu/DCC-2018/)

2.Compression code we use the source code released in [here](https://github.com/iamaaditya/image-compression-cnn) 

## SalPan Dataset
The dataset proposed in our paper is one of our contributions to the research community. This dataset is collected for saliency evaluation on panoramic images, and contain a variety of challenging cases. It contains at most eighteen salient objects in one panoramic images.

You can download in [here](https://github.com/ChunbiaoZhu/DCC-2018/)

If you use this dataset.

Please cite as:

    1. "An Innovative Saliency Guided RoI Selection Model for Panoramic Images Compression. " Chunbiao Zhu, Kan Huang and Ge Li. Data Compression Conference (DCC), 2018

    2. arXiv:1710.04071 [cs.CV]

        @article{DBLP:journals/corr/abs-1710-04071,
        author    = {Chunbiao Zhu and
                     Kan Huang and
                     Ge Li},
        title     = {Automatic Salient Object Detection for Panoramic Images Using Region
                     Growing and Fixation Prediction Model},
        journal   = {CoRR},
        volume    = {abs/1710.04071},
        year      = {2017},
        url       = {http://arxiv.org/abs/1710.04071},
        archivePrefix = {arXiv},
        eprint    = {1710.04071},
        timestamp = {Wed, 01 Nov 2017 19:05:43 +0100},
        biburl    = {https://dblp.org/rec/bib/journals/corr/abs-1710-04071},
        bibsource = {dblp computer science bibliography, https://dblp.org}
      }


## FAQ about image compression
1.Is the final image really a standard JPEG?

Yes, the final image is a standard JPEG as it is encoded using standard JPEG.

2.How can you improve JPEG using JPEG ?

Standard JPEG uses a image level Quantization scaling Q. However, not all parts of the image be compressed at same level. Our method allows to use variable Q.

3.How to plot PR curve?

Precision-recall curve is plotted by comparing the results with the ground-truth through varying thresholds within the range [0, 255]. They are computed for adaptive threshold, which is defined as twice the mean saliency of the image.

## Acknowledgements

This work was supported by the grant of National Natural Science Foundation of China (No.U1611461), Shenzhen Peacock Plan (20130408-183003656), and Science and Technology Planning Project of Guangdong Province, China (No. 2014B090910001).


## Contact

If you have any general doubt about our work or code which may be of interest for other researchers, please use the [public issues section](https://github.com/ChunbiaoZhu/DCC-2018/issues) on this github repo. Alternatively, drop us an e-mail at <mailto:zhuchunbiao@pku.edu.cn>.


