# SSKDNet
This project provides the code for "Cross-resolution collaborative distilaltion network for Low-resolution salient object detection in single-modal and multi-modal images", which is submitted to CGI2026(TVCJ track).
   
   
# Requirements
   python 3.8 + pytorch 1.9.0
      
# Data 
We use down-sampling operator to process each dataset mentioned in paper. i.e., for any one dataset, we extend two variants: 1/2 resolution and 1/4 resolution. We use data augment technology to process training samples for RSI SOD, matlab code is also shwon.

  
# Training
 1 We use data_aug.m for data augmentation. 
   
 2  Download [pvt_v2_b2.pth](https://pan.baidu.com/s/1U6Bsyhu0ynXckU6EnJM35w) (code: sxiq), and put it in './model/'. 
   
 3  Modify paths of datasets, then run train_CRCDNet.py to generate the teacher model. Note that we only regard thermal infrared images as input in this stage

 4 Put train.pth into ./model/.

 5 Modify paths of datasets, then run train_SSKDNet.py to generate the student model. Note that we regard RGB-T images as input in this stage


%Testing
1. Run test_CRCDNet.py.






   
