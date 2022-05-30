## 该文件夹是用来存模式识别作业——vision transformer模型文件的目录
### 下面将针对子文件夹及模型文件进行简单的介绍： 
* （1）文件夹
```
├── plot_img（传入TensorBoard进行可视化的图片，以及predict.py脚本单次预测的图片路径）
├── Post_experimental_processing（存放生成混淆矩阵及模型指标的脚本及图片，同时还有Grad_CAM可视化脚本及结果）
├── runs（传入TensorBoard进行可视化的参数文件，通过train.py脚本生成）
├── tensorboard_results（TensorBoard可视化得到的结果图）
└── weights（保存了训练epochs为50次过程中验证集的val_accuracy最高的权重文件ViT_best.pth）
```
* （2）文件
``` 
├── class_indices.json（生成的json文件用于TensorBoard和predict.py中类别可视化索引）
├── flops.py（统计模型的参数以及FLOPs的脚本）
├── my_dataset.py（自定义数据集的方法脚本）
├── predict.py（模型的预测脚本）
├── README.md（文件类型解释）
├── train.py（模型训练脚本）
├── utils.py （划分数据集，多GPU并行训练，构建TensorBoard可视化，动态学习率等功能的脚本）
├── vit_base_patch16_224_in21k.pth（官方下载的预训练模型权重文件）
├── model.py（alexnet模型文件）
└── vit_model.py（vision transformer模型文件）
```
### 权重文件获取链接：
* （1）vision_transformer网络使用迁移学习所用的预训练权重文件：[vit_base_patch16_224_in21k.pth](https://drive.google.com/file/d/1psvtt5iSWINWk6ePg5K-vTmVAXxU9JRZ/view?usp=sharing)
* （2）vision_transformer网络使用迁移学习训练得到的权重文件：[ViT_best.pth](https://drive.google.com/file/d/1bZQ38N9Ys6uK82MOQt02r4WqDJ2S1821/view?usp=sharing)
