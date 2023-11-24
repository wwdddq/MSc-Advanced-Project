# Week4
本周主要进行了StyleGAN3部分的测试，同时看了两篇与我研究有很大相关性的文献。

## Tech

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

测试结果表明，D的判别对于不同数据集都有着跟基础理论相差很多的误差。此问题保留到下周和导师的meeting中。

## Literatures

### Seeing is not always believing: Benchmarking Human and Model Perception of AI-Generated Images

主要发现：

AIGC 背景对检测的影响： 有人工智能生成内容（AIGC）背景的人在识别人工智能生成图像方面略胜一筹，比没有此类背景的人提高了 3.7%。

区分图像类别的难度： 区分真假图像的难度因类别而异。与 "物体 "类别相比，受试者在识别 "多人 "类别的图像时更为准确。

人工智能生成图像的常见问题： 人工智能生成的图像中常见的缺陷包括细节和平滑度问题，这使得人们很难描述明显的缺陷。

模型评估： 该研究引入了 MPBench，这是一种利用大型数据集对人工智能模型区分人工智能生成的图像和真实图像的能力进行综合评估的方法。

模型性能差异： 根据训练数据集和验证数据集的特征，模型性能差异很大，这突出了多样化数据集对提高准确性的重要性。

最佳模型性能： 使用数据集设置 D 训练的 ConvNext-S 模型被认定为检测假图像最有效的模型，但仍有 13% 的失败率。

图像生成模型的进展： 先进的文本到图像合成方法在图像保真度和多样性方面超越了之前基于 GAN 的模型。

人工智能算法在假图像检测中面临的挑战： 当前的人工智能算法在虚假图像检测方面仍面临重大挑战，这体现在相当高的误判率上。

- 这篇文献给了我很大启发，尤其是文中对比人类和奇迹的感知差异的方法。

### Seeing is Believing: Exploring Perceptual Differences in DeepFake Videos

人类的视觉和认知特性：人类在视觉识别和处理信息时，自然地倾向于关注面部特征和其他显著的视觉元素。面部特征，如眼睛、鼻子、嘴巴，以及表情通常是人类识别和理解图像，尤其是判断人物身份和情绪的关键因素。因此，在检测DeepFake视频时，用户自然会关注这些区域，以寻找可能的不一致之处。

DeepFake生成技术的局限性：DeepFake技术虽然在模仿和替换面部特征方面取得了长足的进步，但仍存在一些技术局限性。例如，在头发的边缘、眼睛或嘴唇的对齐等细节上可能出现不自然的痕迹。这些局限性导致了视觉上的不一致，成为检测DeepFake的重要线索。

实验数据和用户反馈：论文中的研究方法包括用户调查和眼动追踪数据的分析。通过这些方法，作者能够收集到关于用户在观看视频时自然聚焦的区域的数据。用户的反馈和眼动数据揭示了他们在检测DeepFake时倾向于关注的特定区域。

与现有文献的对比：现有的关于人类视觉感知和DeepFake检测的文献也为这些视觉线索的选择提供了理论支持。以往的研究表明，在进行视觉真实性判断时，人们会特别关注那些在日常经验中被认为是身份和情感表达的关键因素的区域。

- 此文章使用的这些基础视觉线索对我的研究很有参考性。
