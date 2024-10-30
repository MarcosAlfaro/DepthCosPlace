# DepthCosPlace
In this project we tackle place recognition with panoramic images and depth maps obtain with Depth Anything v2. We also explore different strategies of data fusion.

The images belong to the COLD database, which can be downloaded from their official website https://www.cas.kth.se/COLD/. This dataset contains omnidirectional images captured by a mobile robot in different indoor environments: Freiburg Part A and B and Saarbrücken Part A and B. The images have been captured under three different lighting conditions: Cloudy, Night and Sunny. In this study, cloudy images from Freiburg Part A are used to train the CNNs, which are tested under every environment and lighting condition.

The CNN model that has been selected is CosPlace. Transfer learning technique has been applied in every layer. A triplet architecture has been employed to train the CNNs. One model has been trained with panoramic images, another with depth maps, obtained by means of Depth Anything v2, and another with both types combined (early fusion). 

Three different strategies of data fusion are evaluated: early fusion, middle fusion and late fusion. 
Different techniques of late fusion are compared as well. 

The experiments reveal that combining visual and depth information enhance the robustness against lighting changes and improves substantially the performance in the zero-shot place recognition task. 
