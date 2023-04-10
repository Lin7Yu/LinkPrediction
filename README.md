# 异质图自编码器实现miRNA与疾病之间的链路预测

本项目基于异质图自编码器，使用DGL深度学习库和MXNet模型实现miRNA与疾病之间的链路预测。该项目旨在探索miRNA与疾病之间的潜在关联，从而为疾病的早期预测和治疗提供新的思路和方法。

## 项目背景

miRNA是一类非编码RNA，能够通过调节基因表达来影响多种生物过程，如细胞增殖、分化和凋亡等。近年来，越来越多的研究表明miRNA与疾病之间存在着密切的关系。因此，探索miRNA与疾病之间的关联对于疾病的研究和治疗具有重要的意义。

## 项目目标

本项目旨在基于异质图自编码器，预测miRNA与疾病之间的链路。通过训练模型，预测潜在的miRNA-disease链路，从而为疾病的早期预测和治疗提供新的思路和方法。

## 数据集

本项目使用miRNA-disease数据集，该数据集包括miRNA-disease的相互作用关系以及miRNA和疾病的其他信息，如miRNA的序列和疾病的症状等。该数据集来自从HMDD数据库（2013年6月），共包括495个miRNA和383个疾病，以及miRNA-disease之间的相互作用关系。

## 方法

本项目使用了DGL深度学习库和MXNet模型，构建了异质图自编码器，用于预测miRNA-disease之间的链路。具体而言，我们首先构建miRNA-disease的异质图，将miRNA和疾病作为节点，将miRNA-disease之间的相互作用关系作为边。然后，我们使用异质图自编码器对miRNA-disease异质图进行编码和解码，从而预测潜在的miRNA-disease链路。

### 安装准备

本项目需要的库通过pip进行安装，使用以下命令进行安装：

```
Copy code
pip install mxnet==1.6.0 dgl==0.4.3post1 pandas==1.0.3 numpy==1.16.6 scikit-learn==0.20.3 pytorch==1.2.0 matplotlib
```

另外，本项目需要CUDA 10.2的支持，需要在安装时进行相应的配置。

### 数据准备

本项目使用的miRNA-disease数据集可以从公共数据集中获取。数据集包括miRNA-disease之间的相互作用关系以及miRNA和疾病的其他信息，如miRNA的序列和疾病的症状等。

本项目的灵感和数据集来自GAEMDA（A graph auto-encoder [model](https://so.csdn.net/so/search?q=model&spm=1001.2101.3001.7020) for miRNA-disease associations prediction）项目。我们使用GAEMDA提供的数据集进行了miRNA-disease链路预测的实验，感谢GAEMDA项目提供的支持。

### 运行代码

本项目的代码可以通过Git进行获取。

获取代码后，可以使用以下命令运行代码：

```
python main.py
```

代码将会自动进行miRNA-disease链路的预测，并输出预测结果。

## 总结

本项目基于异质图自编码器，使用DGL深度学习库和MXNet模型实现miRNA与疾病之间的链路预测。实验结果表明，本项目的异质图自编码器模型能够有效地预测miRNA-disease之间的链路，从而为疾病的早期预测和治疗提供新的思路和方法

