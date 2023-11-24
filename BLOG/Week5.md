# Week5
在本周和导师的meeting中，我提出了上周发现的问题。

同时，我在本周搜索相关的内容时，也注意到一条在GitHub上的评论。

- https://github.com/NVlabs/stylegan3/issues/180

这条评论指出，不同的数据集和模型会导致StyleGAN判别器的输出分数有所不同，较高分代表图像真实，较低分代表图像为伪造。

经过和导师的讨论，我决定选定一个数据集，进行数量多一些的数据对比，并尝试从中找到一些规律。

我选择了MetFaces数据集，因为先前的研究大多是基于FFHQ的人脸检测，但我想从艺术图像上去探索人类和机器的感知差异。还有一点是，MetFaces是真实画作中的人物肖像画，此数据集也是Nvidia官方发布，在标准型上具有一定的优势。

在分析过程中，我使用基于Metfaces的StyleGAN3预训练模型生成了100张合成的人物肖像画图像，并将其编号为seed0001-0100。同样，我从metfaces数据集中随机选取了100张真实的人物肖像画图像，并编号为MF1-100。随后，我对这200张图像逐一使用判别器进行了评分并记录了结果。

我对这些数据进行了从低到高的排列，结果可以下面的链接中看到。（图中标注颜色的是被选作实验样本的图像）
- https://github.com/wwdddq/MSc-Advanced-Project/blob/main/StyleGAN3-D/data-D.pdf

我处理了 200 个有效数据点的分数，结果显示平均分数约为 -1.34，范围从最低值 -5.24 到最高值 3.31。值得注意的是，82% 的分数为负，这表明虽然大多数倾向于负值，但总体分数分布中仍有很大一部分低于零。

由此得出的结论是，尽管判别器的输出分数与其基础理论之间存在差异，但这些分数在单个数据集中表现出了可辨别的模式。具体来说，在基于 MetFaces 数据集的模型中，较低的鉴别器 (D) 输出分数表明生成图像的可能性较高，反之亦然。

利用计算指标中的分数阈值理论框架，我建立了一个分数阈值（这 200 个图像的 D 输出的中值分数），以区分该数据集中的真实图像和生成图像。因此，在我的实验设置中，得分高于 -1.6163 的图像被归类为真实图像，而那些得分低于 -1.6163 的图像被视为伪造。

我从表格中提取出了20张图片。这20张图片分别有10张原本是真实的，10张原本是生成的。10张真实的图像中，有五张是机器认为假的图像。而10张生成的图像中，也有五张是机器认为真实的图像。

本周的最后，我用这20张图像进行了简短的问卷调查，但人们反馈图片有些太多了。所以我从这20张图像又进一步随机筛选出了10张图像，结果如下。

![MSc-Advanced-Project](https://github.com/wwdddq/MSc-Advanced-Project/blob/main/BLOG/img/paper_img.001.jpeg)