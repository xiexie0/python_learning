# 基于MNIST数据集的深度学习

使用PyTorch在 MNIST 数据集上进行神经网络的搭建，训练和测试（详细步骤请见实验步骤和文件说明）

## 环境配置

下载并安装Anaconda，配置环境变量  [安装教程](https://blog.csdn.net/qq_45281589/article/details/134597810)

实验环境：Python 3.12.2

使用以下命令安装所需的依赖：

```
# 安装 numpy
!pip install numpy
# 安装 matplotlib
!pip install matplotlib
# 安装 PyTorch 和 torchvision
!pip install torch 
!pip install torchvision
```

## 实验步骤

环境配置好后先进行最简单的神经网络搭建训练（mnist_classifier.ipynb），会自动下载MNIST数据集到data文件夹并进行格式转换。生成模型的权重会保存在mnist_model.pth中。然后可以使用已生成的权重随机选取MNIST数据集中的图像进行直观测试（model_test.ipynb）。

随后可以进行卷积神经网络CNN的搭建，训练和评估。生成模型的权重保存在mnist_model_cnn.pth中。最后可以通过已生成的模型对随意输入的图片（test_number.jpg）进行数字判断（model_test_cnn.ipynb）。

## 文件说明

mnist_classifier.ipynb：使用PyTorch在MNIST数据集上训练一个简单的神经网络，包括数据加载、模型定义、训练和验证步骤。最后保存生成的模型权重。

model_test.ipynb：随机选取MNIST数据集中图像对生成的模型进行可视化测试。

mnist_classifier_CNN.ipynb：使用PyTorch构建和训练一个简单的卷积神经网络模型，以识别MNIST手写数字。包括数据预处理、模型定义、训练模型以及评估模型准确率。

model_test_cnn.ipynb：通过已生成的模型对输入的图片进行数字判断。

minst_model_cnn.pth，minst_model.pth：生成的模型权重

data：MNIST数据集

## 学习资料

[PyTorch官方教程](https://pytorch.org/tutorials/)

[TensorFlow 官方教程](https://www.tensorflow.org/tutorials)

[Sentdex](https://www.youtube.com/user/sentdex)(PyTorch和TensorFlow教程)

[PyTorch Examples](https://github.com/pytorch/examples) (PyTorch示例项目)

[TensorFlow Models](https://github.com/tensorflow/models) (TensorFlow模型)
