# Res-GCNN
We present a novel network called Residual Graph Convolutional Neural Network (Res-GCNN) for pedestrians trajectory prediction. We design Res-GCNN for onboard application in autonomous vehicles, therefore, real-time performance is a key factor.<br>
The Res-GCNN models the interactive behaviors of pedestrians by using the adjacent matrix of the constructed graph for the current scene. Though the proposed Res-GCNN is quite lightweight with only about 6.4 kilo parameters which outperforms all other methods in terms of parameters size, our experimental results show an improvement over the state of art by 13.3% on the Final Displacement Error (FDE) which reaches 0.65 meter. As for the Average Displacement Error (ADE), we achieve a suboptimal result (the value is 0.37 meter), which is also very competitive. The Res-GCNN is evaluated in the platform with an NVIDIA GeForce RTX1080Ti GPU, and its mean inference time of the whole dataset is only about 2.2 microseconds. Compared with other methods, the proposed method shows strong potential for onboard application accounting for forecasting accuracy and time efficiency.

## The ADE / FDE metrics of Res-GCNN compared with other methods
此处插入表格<br>
|Model\Dataset|ETH|HOTEL|UNIV|ZARA1|ZARA2|AVG|
|:---|:---|:---|:---|:---|:---|:---|
|Linear|1.33 / 2.94 |0.39 / 0.72	|0.82 / 1.59	|0.62 / 1.21	|0.77 / 1.48	|0.79 / 1.59|
|SR-LSTM-2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|
|S-LSTM|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|
|S-GAN-P|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|
|SoPhie|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|
|CGNS|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|
|PIF|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|
|STSGN|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|
|GAT|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|
|Social-BiGAT|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|
|Social-STGCNN|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|
|Meituan|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|
|Res-GCNN|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|列2的内容2|

## [参考链接](https://blog.csdn.net/u012234115/article/details/41778701 "悬停显示")
