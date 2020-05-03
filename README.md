# CTR学习笔记
python main.py --model DeepFM --step train --input_type sparse --clear_model 1

1. 已完成模型列表

- FM 
- FFM 
- Embedding+MLP
- wide & Deep
- DeepFM [sparse & dense]
- PNN 
- FNN 
- AFM [sparse & dense]
- NFM [sparse & dense]

2. 数据集
所有模型都支持dense输入的model_fn，部分模型支持sparse输入的model_fn。考虑到只有两份数据集，input_type直接和data_dir，training_parameter绑定了，丑是丑了点以后要是加别的数据集再改吧。。。
- dense：https://archive.ics.uci.edu/ml/machine-learning-databases/adult
- sparse：http://baltrunas.info/research-menu/frappe

3. 参考论文列表
- [GBDT+LR] Practical Lessons from Predicting Clicks on Ads at Facebook
- [FM] S. Rendle, Factorization machines
- [FM Model] Fast Context-aware Recommendations with Factorization Machines
- [FFM] Yuchin Juan，Yong Zhuang，Wei-Sheng Chin，Field-aware Factorization Machines for CTR Prediction
- [Wide&Deep] Cheng H T, Koc L, Harmsen J, et al. Wide & deep learning for recommender systems
- [FNN] Weinan Zhang, Tianming Du, and Jun Wang. Deep learning over multi-field categorical data - - A case study on user response
- [PNN] Qu Y, Cai H, Ren K, et al. Product-based neural networks for user response prediction
- [DeepFM] Huifeng Guo et all. DeepFM: A Factorization-Machine based Neural Network for CTR Prediction
- [AFM] Attentional Factorization Machines - Learning the Weight of Feature Interactions via Attention Networks
- [NFM] Neural Factorization Machines for Sparse Predictive Analytics
- [DIN] Deep Interest Network for Click-Through Rate Prediction.
- [DIEN] Deep Interest Evolution Network for Click-Through Rate Prediction
- [DCN] Deep & Cross Network for Ad Click Predictions
- [xDeepFM] xDeepFM- Combining Explicit and Implicit Feature Interactions for Recommender Systems

4. 总结博客
- CTR学习笔记&代码实现1-深度学习的前奏LR->FFM https://www.cnblogs.com/gogoSandy/p/12501846.html
- CTR学习笔记&代码实现2-深度ctr模型 MLP->Wide&Deep https://www.cnblogs.com/gogoSandy/p/12658051.html
- CTR学习笔记&代码实现3-深度ctr模型 FNN->PNN->DeepFM https://www.cnblogs.com/gogoSandy/p/12742417.html
- CTR学习笔记&代码实现4-深度ctr模型 NFM/AFM https://www.cnblogs.com/gogoSandy/p/12814804.html
