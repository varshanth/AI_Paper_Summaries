# Data Cleaning and Learning with Noisy Labels

## Simple Pipeline
1) On the Fly Data Denoising: https://arxiv.org/pdf/2003.10647.pdf
    a. Remove training samples incurring high loss  
    b. Start with a high LR and find optimal high LR which does not lead to model overfitting. Remove those samples whose loss is above threshold.  
    c. Train with remaining samples with lower LR
2) Eliminating Semantic Redundancies: https://arxiv.org/pdf/1901.11409.pdf
    a. Use an initial model to extract image features for all images in dataset  
    b. Employ clustering algorithm on the image features  
    c. Retain 90% of the data (bonus is retain the top N members in the clusters who are furthest from the cluster center [outliers])
3) Dataset Valuation: http://proceedings.mlr.press/v97/ghorbani19c/ghorbani19c.pdf
    a. Determine the value of each datapoint in the dataset by calculating its Shapley value  
    b. Retain only the top N valuable members
    
## Paper Reading List
https://github.com/subeeshvasu/Awesome-Learning-with-Label-Noise
