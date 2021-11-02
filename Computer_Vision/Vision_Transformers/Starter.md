# Transformers for Vision

## Vision Transformer (ViT)
https://theaisummer.com/vision-transformer/
## Swin Transformer: https://arxiv.org/abs/2103.14030
1) https://www.youtube.com/watch?v=tFYxJZBAbE8&ab_channel=AIBites  
2) https://www.youtube.com/watch?v=SndHALawoag&ab_channel=AICoffeeBreakwithLetitia
3) https://crossminds.ai/video/swin-transformer-hierarchical-vision-transformer-using-shifted-windows-606d0de375292b321dd08f80/
### Keep in mind:
1) Patch Merging Block: Takes as input say (H/4) x (W/4) x C, concats neighboring 2x2 patches along the feature axis (H/8) x (W/8) x 4C, and then applies a linear layer to compress 4C into 2C. 
