# Res-GCNN
We present a novel network called Residual Graph Convolutional Neural Network (Res-GCNN) for pedestrians trajectory prediction. We design Res-GCNN for onboard application in autonomous vehicles, therefore, real-time performance is a key factor.<br>
The Res-GCNN models the interactive behaviors of pedestrians by using the adjacent matrix of the constructed graph for the current scene. Though the proposed Res-GCNN is quite lightweight with only about **6.4** kilo parameters which outperforms all other methods in terms of parameters size, our experimental results show an improvement over the state of art by **13.3%** on the Final Displacement Error (FDE) which reaches **0.65** meter. As for the Average Displacement Error (ADE), we achieve a suboptimal result (the value is **0.37** meter), which is also very competitive. The Res-GCNN is evaluated in the platform with an NVIDIA GeForce RTX1080Ti GPU, and its mean inference time of the whole dataset is only about **2.2** microseconds. Compared with other methods, the proposed method shows strong potential for onboard application accounting for forecasting accuracy and time efficiency.

## Model Architecture


## The ADE / FDE metrics of Res-GCNN compared with other methods
The positions are observed every 0.4 second. The same as our superior counterparts, we use 8 historical data frames to forecast the coming 12 data frames.<br>
|**Model\Dataset**|ETH|HOTEL|UNIV|ZARA1|ZARA2|AVG|
|:---|:---|:---|:---|:---|:---|:---|
|Linear|1.33 / 2.94 |0.39 / 0.72	|0.82 / 1.59	|0.62 / 1.21	|0.77 / 1.48	|0.79 / 1.59|
|SR-LSTM-2|0.63 / 1.25	|0.37 / 0.74	|0.51 / 1.10	|0.41 / 0.90	|0.32 / 0.70	|0.45 / 0.94|
|S-LSTM|1.09 / 2.35	|0.79 / 1.76	|0.67 / 1.40	|0.47 / 1.00	|0.56 / 1.17	|0.72 / 1.54|
|S-GAN-P|0.87 / 1.62	|0.67 / 1.37	|0.76 / 1.52	|0.35 / 0.68	|0.42 / 0.84	|0.61 / 1.21|
|SoPhie|0.70 / 1.43	|0.76 / 1.67	|0.54 / 1.24	|0.30 / 0.63	|0.38 / 0.78	|0.54 / 1.15|
|CGNS|0.62 / 1.40	|0.70 / 0.93	|0.48 / 1.22	|0.32 / 0.59	|0.35 / 0.71	|0.49 / 0.97|
|PIF|0.73 / 1.65	|**0.30** / 0.59	|0.60 / 1.27	|0.38 / 0.81	|0.31 / 0.68	|0.46 / 1.00|
|STSGN|0.75 / 1.63	|0.63 / 1.01	|0.48 / 1.08	|0.30 / 0.65	|0.26 / 0.57	|0.48 / 0.99|
|GAT|0.68 / 1.29	|0.68 / 1.40	|0.57 / 1.29	|0.29 / 0.60	|0.37 / 0.75	|0.52 / 1.07|
|Social-BiGAT|0.69 / 1.29	|0.49 / 1.01	|0.55 / 1.32	|0.30 / 0.62	|0.36 / 0.75	|0.48 / 1.00|
|Social-STGCNN|0.64 / 1.11	|0.49 / 0.85	|0.44 / 0.79	|0.34 / 0.53	|0.30 / 0.48	|0.44 / 0.75|
|Meituan|**0.39 / 0.79**	|0.51 / 1.05	|**0.25 / 0.56**	|0.30 / 0.61	|0.36 / 0.73	|**0.36** / 0.75|
|**Res-GCNN**|0.65 / 1.12	|0.31 / **0.50**	|0.38 / 0.72	|**0.28 / 0.50**	|**0.24 / 0.41**	|0.37 / **0.65**|

## [参考链接](https://blog.csdn.net/u012234115/article/details/41778701 "悬停显示")
