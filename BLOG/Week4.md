# Week4
本周主要进行了StyleGAN3部分的测试

在上周，我在使用FFHQ数据集的预训练模型进行了D输出数据的基础测试。

我们发现D的输出评分范围为-1到1，这与一般的预期（D的评分应在0到1之间，且越接近1表示图像越真实）有所不同。

通过进一步测试ffhq数据集，我们意外发现，当D的输出接近0时，图像更可能被认为是真实的，而输出接近1时，则被认为是生成的。

基于此基础测试，我尝试对现有的使用不同数据集的StyleGAN3的预训练模型都进行一些基础测试。
- Datasets Source: https://github.com/justinpinkney/awesome-pretrained-stylegan3/blob/main/README.md

以下是测试的记录

![MSc-Advanced-Project](https://github.com/wwdddq/MSc-Advanced-Project/blob/main/BLOG/img/1.png)
![MSc-Advanced-Project](https://github.com/wwdddq/MSc-Advanced-Project/blob/main/BLOG/img/2.png)
![MSc-Advanced-Project](https://github.com/wwdddq/MSc-Advanced-Project/blob/main/BLOG/img/3.png)
![MSc-Advanced-Project](https://github.com/wwdddq/MSc-Advanced-Project/blob/main/BLOG/img/4.png)
![MSc-Advanced-Project](https://github.com/wwdddq/MSc-Advanced-Project/blob/main/BLOG/img/5.png)
![MSc-Advanced-Project](https://github.com/wwdddq/MSc-Advanced-Project/blob/main/BLOG/img/6.png)
![MSc-Advanced-Project](https://github.com/wwdddq/MSc-Advanced-Project/blob/main/BLOG/img/7.png)
![MSc-Advanced-Project](https://github.com/wwdddq/MSc-Advanced-Project/blob/main/BLOG/img/8.png)
![MSc-Advanced-Project](https://github.com/wwdddq/MSc-Advanced-Project/blob/main/BLOG/img/9.png)
![MSc-Advanced-Project](https://github.com/wwdddq/MSc-Advanced-Project/blob/main/BLOG/img/10.png)
![MSc-Advanced-Project](https://github.com/wwdddq/MSc-Advanced-Project/blob/main/BLOG/img/11.png)
![MSc-Advanced-Project](https://github.com/wwdddq/MSc-Advanced-Project/blob/main/BLOG/img/12.png)
