# 预测手写数字序列（From Udacity）

MNIST是一个手写体数字识别数据集，它是NIST数据集的一个子集，包含了60,000张图片作为训练数据，10,000张图片作为测试数据。

在MNIST数据集中的每一张图片都代表了0～9中的一个数字。图片的大小都为28×28，且数字都会出现在图片的正中间。下面展示了数据集中的样例图片：

![MNIST](https://github.com/TIFOSI528/MNIST/raw/master/raw/原始数据集.png)

## 我们将利用MNIST原始数据集，随机取出随机（1-5）张图片，然后将它们拼接成新的图片。最后，我们再搭建卷积神经网络对数字序列进行识别。
+ 需要注意的是，空白的图片将用‘10’来表示。

下面是一些拼接的图片：

![MNIST](https://github.com/TIFOSI528/MNIST/raw/master/raw/数字序列.png)

### 我们虽然得到了模型预测每个数字的准确率，但我们需要计算整体准确率，按照完全预测正确数字序列的标准来计算。

比如 1,2,3,10,10 预测成了 1,2,10,10,10 算错，而不是算对了80%。

digit_recognition.ipynb中的模型能实现92%的整体准确率，我们也可以对预测结果进行可视化：

![MNIST](https://github.com/TIFOSI528/MNIST/raw/master/raw/预测结果.png)












这个项目使用 **Keras** 完成，需要安装下面这些 Python 包：

- [NumPy](http://www.numpy.org/)
- [TensorFlow](http://tensorflow.org)
- [Keras](https://keras.io)
