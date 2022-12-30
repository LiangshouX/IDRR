源码目录结构如下：

```
source code
├─Dataset
│  ├─data	# 切分后的训练集、测试集和验证集等
│  ├─log	# 训练中输出的log信息
│  └─saved_dict	# 保存训练权重的位置，可下载放入此路径
├─pretrained
│  └─roberta-base	# RoBERTa预训练模型
├─raw
│  ├─pdtb2			# PDTB2.0 语料库
│  │  └─__pycache__
│  └─__pycache__
└─__pycache__
```



准备：

​	从[roberta-base](https://huggingface.co/roberta-base/tree/main)中下载`pytorch_model.bin`文件，置于RoBERTa预训练模型路径下

运行：

```shell
python preprocess.py
```

```shell
python run.py
```

