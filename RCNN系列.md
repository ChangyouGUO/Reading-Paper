## RCNN:
  Abstract:  
  　1. 对region proposal使用卷积网络。  
  　2. 训练数据少，通过fine-tuning来提升性能。  
  Introduction:  
  &nbsp;&nbsp;过去的视觉识别任务主要使用SIFT和HOG.   
  &nbsp;&nbsp;目标检测需要解决两个问题：1. 定位目标；2. 用稀少的标注数据训练大网络。  
  &nbsp;&nbsp;定位物体: 1.将其看作回归问题。2.建立滑动窗口检测器   
  &nbsp;&nbsp;数据稀少: 采用ILSVRC大数据集首先进行监督预训练，然后在PASCAL的小数据集上进行网络的微调。  
  &nbsp;&nbsp;在inference的时候，首先在输入图片中抽取2000个无关类别的区域；忽略区域尺寸，warp到固定的尺寸作为CNN的输入；  
  &nbsp;&nbsp;CNN网络抽取出固定长度的特征向量；用每一类的线性SVM进行分类。
     
  　　
    
  
