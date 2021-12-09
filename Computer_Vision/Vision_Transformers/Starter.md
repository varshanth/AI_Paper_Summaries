# Transformers for Vision

## Image and Video Classification
### Vision Transformer (ViT)
Paper: https://arxiv.org/abs/2010.11929  
Explanation: https://theaisummer.com/vision-transformer/

### Data Efficient Image Transformer (DeiT)
Paper: https://arxiv.org/pdf/2012.12877.pdf  
Explanation: https://storrs.io/deit/

### Swin Transformer
Paper: https://arxiv.org/abs/2103.14030  
Explanations:  
1) https://www.youtube.com/watch?v=tFYxJZBAbE8&ab_channel=AIBites  
2) https://www.youtube.com/watch?v=SndHALawoag&ab_channel=AICoffeeBreakwithLetitia
3) https://crossminds.ai/video/swin-transformer-hierarchical-vision-transformer-using-shifted-windows-606d0de375292b321dd08f80/

#### Keep in mind:
1) Patch Merging Block: Takes as input say (H/4) x (W/4) x C, concats neighboring 2x2 patches along the feature axis (H/8) x (W/8) x 4C, and then applies a linear layer to compress 4C into 2C. 

### Convolutional Vision  Transformer (CvT)
Paper:  https://openaccess.thecvf.com/content/ICCV2021/papers/Wu_CvT_Introducing_Convolutions_to_Vision_Transformers_ICCV_2021_paper.pdf  
Explanation:  
* Uses Depthwise Separable Convolution to perform Q, K, V projections in the MHSA block. The MHSA block is called the Conv. Transformer Block (CBT)
* Uses stride=2 DSC for K, V projection and stride 1 for Q projection. This is to increase efficiency while not compromising performance as much since spatially near pixels/tokens correspond to similar information.
* After a CBT block, a conv. block (called the Conv. Token Embedding) is employed for further spatial feature extraction.
* No positional encoding is used since input is being processed as a spatial structure

## Object Detection
### Detection Transformer (DETR): 
Paper: https://arxiv.org/abs/2005.12872  
Explanation:  
https://www.youtube.com/watch?v=T35ba_VXkMY&ab_channel=YannicKilcher  
https://chadrick-kwag.net/paper-review-end-to-end-detection-with-transformers-a-k-a-detr/  
