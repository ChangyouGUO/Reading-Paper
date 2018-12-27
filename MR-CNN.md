# Object detection via a multi-region & semantic segmentation-aware CNN model  
### Abastract  
* 迭代定位，box目标区域打分/使用深层CNN回归模型修正定位。 
## Introduction  
 
* 15年前几年，深度学习方面，标杆性检测模型就是Overfeat和RCNN。  
* Overfeat 滑动窗口，多尺度。两个CNN，一个用于分类，一个用于定位；最后通过greeedy algorithm进行融合。  
* RCNN的提升非常大，比起传统的deformable parts models 和 non-linear multi-kernel approaches方法都好（两篇文章传统-最好的方法）。因为不再使用人造的HOG 和 SIFT特征。  

* 两点改进： 1. 目标表达。多尺寸，图片的多个局部。学习额外的语义分割的特征。  

