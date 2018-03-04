## An Innovative Saliency Guided RoI Selection Model for Panoramic Images Compression




|  ![DCC 2018 logo][logo-DCC] | Paper accepted at [2018 Data Compression Conference](http://www.cs.brandeis.edu/~dcc/index.html) Cliff Lodge, Snowbird, UT, Tuesday - Friday, March 27 - 30. |
|:-:|---|

[logo-DCC]: https://github.com/ChunbiaoZhu/DCC-2018/blob/master/logo/DCCbanner_text.png "DCC 2018 logo"




## Abstract

Saliency detection has been an increasingly important tool for ROI selection in image compression. Most previous works on saliency detection are dedicated to conventional images, however, with the rapid development of VR or AR technology, it is becoming more and more important to obtain visual attention for panoramic images. Meanwhile, panoramic images have more potential for improvement in compression performance compared with the conventional case.

In this work, we propose an innovative saliency guided ROI selection model, shown in Fig.1. We first employ a spatial density pattern detection method based on region growing to roughly extract the proposal objects. And the eye fixation model is employed to predict the visual attention, which is inspired by neurobiological mechanisms of the human vision system. Then, the previous saliency information is combined by the maxima normalization to produce the coarse saliency map. Finally, a geodesic distance based refinement is utilized to derive the final saliency map.

Extensive evaluations show the proposed approach outperforms other methods in saliency accuracy especially for panoramic images. Meanwhile, we improve the compression quality of standard JPEG by using a higher bit rate to encode image regions flagged by our model and lower bit rate elsewhere in the image. With our proposed ROI selection model, we improve the compression performance compared with the standard JPEG by 10~35%. To our consideration, this research also help to figure out the perception characteristics of the human visual system for large-scale visual contents over a wide field of view.

 


## Framework
![QFramework saliency detection](https://github.com/ChunbiaoZhu/DCC-2018/blob/master/images/fig1.png)


## Code & Results

Source code will be released soon! You can download in [here](https://github.com/ChunbiaoZhu/DCC-2018/)

More results will be public soon in [here](https://github.com/ChunbiaoZhu/DCC-2018/)

## FAQ about image compression
Is the final image really a standard JPEG?

Yes, the final image is a standard JPEG as it is encoded using standard JPEG.

But how can you improve JPEG using JPEG ?

Standard JPEG uses a image level Quantization scaling Q. However, not all parts of the image be compressed at same level. Our method allows to use variable Q.


## Acknowledgements

This work was supported by the grant of National Natural Science Foundation of China (No.U1611461), Shenzhen Peacock Plan (20130408-183003656), and Science and Technology Planning Project of Guangdong Province, China (No. 2014B090910001).


## Contact

If you have any general doubt about our work or code which may be of interest for other researchers, please use the [public issues section](https://github.com/ChunbiaoZhu/DCC-2018/issues) on this github repo. Alternatively, drop us an e-mail at <mailto:zhuchunbiao@pku.edu.cn>.


