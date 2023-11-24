# Week7
本周的工作目标是：看三篇文献，撰写论文大纲

## 文献

### Landscape Art Image Style Reconstruction Algorithm Based on Machine Learning

摘要：本文讨论了使用具有注意力机制的循环一致性生成对抗网络（GANs）进行图像风格转换，尤其是景观艺术图像风格转换。 它强调增强图像的特定特征以获得更好的风格转换效果。

简介：该论文强调了人工智能和深度学习的兴起，尤其是在非逼真渲染方面。论文强调了图像风格转移在各个领域日益增长的重要性，从社交媒体上的个人表达到电影和动画等商业应用。

艺术图像风格重构：神经风格转移概述： 本文概述了神经风格转移，这是一种使用卷积神经网络将一个图像的内容与另一个图像的风格相结合的技术。 论文引用了为这一领域奠定基础的 Gatys 等人的研究成果。

景观艺术图像风格重构算法：论文深入探讨了GANs在图像风格转换中的应用，强调了使用这些模型生成多视角图像转换和自动描述生成所面临的挑战和机遇。

结论：文章最后讨论了图像风格转换技术的广泛应用和研究价值。本文提出了一种景观图像风格转换模型，该模型使用具有注意力机制的 GANs 来增强特定特征，以提高风格化效果。

### Mechanisms of Face Perception

摘要：人脸感知被认为是一种独特的信息刺激，在人脑中与众不同，在猕猴中也能观察到。一种假说认为，人脸处理的特殊性是由于一个强制性的检测过程，本文旨在通过各种实验来澄清和证明这一点。

导言：本文将人脸识别与物体识别进行了比较，强调了在位置、光照和遮挡发生变化的情况下辨别细微差别的必要性。这种比较将人脸感知作为物体识别的一个缩影。

机理回顾：本文从计算理论、算法和神经实现等不同层面回顾了人脸处理过程，详细阐述了人脸处理过程中的相关机制问题。

计算机视觉算法：计算机视觉中的人脸处理分为检测、测量和分类。检测包括识别人脸的存在，测量包括根据人脸的特征区分各个人脸，而分类则是根据身份、性别和年龄等属性对人脸进行分类。

算法回顾：介绍了对人脸识别可能的生物机制提供见解的算法的综述，如 Viola-Jones 和 Sinha 的算法以及 Eigenface 算法。其中包括对基于特征的方法和整体方法的讨论。

人类行为和功能成像：讨论了行为研究和功能成像数据，如在人脸感知任务中纺锤形回和纺锤形面区（FFA）的激活。这一部分强调了大脑中人脸处理过程的独特性，并提出了一个独特的人脸检测阶段。

测量与分类：通过fMRI研究探讨了人脑中存在单独的人脸测量和分类系统的可能性，这些研究表明枕叶人脸区（OFA）和FFA在人脸处理中扮演着不同的角色。

猴子 fMRI 和单一单元生理学：详细介绍了利用 fMRI 和单单元生理学研究猴子的面孔选择性细胞及其在检测和整体处理面孔中的作用。本节包括对人脸细胞的解剖特化和特征组合反应的时间过程的讨论。

未来研究方向：本文最后提出了未来的研究方向，质疑了人脸处理的独特性、其模块化性质以及检测-门控假说对理解人脸识别和检测处理的影响。

- 在撰写论文大纲时，参考了之前分析过的文献，这也是我记录读过的文献是分章节来写的原因。

## 论文draft

- Title
A Comparative Study of Human and Artificial Intelligence in Perceiving Image Realism

- Abstract
Provides a brief overview of the research question, which is how artificial intelligence discriminates between true and false images compared to human perception. Briefly describe the research methodology, including human studies, computational metrics, and thematic analyses. Highlights key findings, such as differences between human and AI judgements of image authenticity, and suggests implications for wider online disinformation.

- 1 Introduction
1.1 Motivation: the problem of misinformation in contemporary internet communication and the harm it causes is drawn from the hyper-conventionalisation of documentary films, with the characteristics of misinformation: no scientific basis/one-sidedness/intentional amplification. (US Election 2016) points out that most of the visual misleading information on the Internet is machine-generated. Humans can be misled by generated images, what about machines? To introduce the challenges of humans and machines for recognising the authenticity of visual content in contemporary society.

- 2.1 Objective:
Research question: to analyse the differences between humans and Generative Adversarial Networks (GANs) in judging the authenticity of portraits of people in paintings
Inspiration: the use of generative images by others as misleading information to get Trump elected as president in the 2016 US election
Artistic theme of special interest: the difference in perception between humans and AI in relation to portraits of people in paintings, e.g. a human judging whether a picture of a portrait of a person in a painting is real or generated might judge it in terms of colours, texture details, style of painting, etc., but what about GAN? And what are the factors by which the discriminator of GAN determines whether a picture is real or generated.
Objective of Technology Development and Application: to extract the authenticity result scores assessed by the discriminator of styleGAN3 for portraits of people in real paintings and portraits of people in generated paintings, and to analyse the results to derive the commonalities and differences. The purpose of this operation is to do human experiments with these pictures, i.e., whether a human and a machine agree on the authenticity judgement of the same picture, and to study the reasons for their agreement or disagreement. The goal of the application is to make human beings feel the influence of images on misleading information in the process of doing the experimental experience, as well as to warn people to keep their own subjectivity and not to be influenced by others who use the machine's subjectivity.

- 2 Background and related work
2.1 The role of images in information dissemination: a discussion of the prevalence of online information dissemination and the key role of images as a medium. Review the literature on human and computer vision systems for assessing the veracity of images. Humans judge the authenticity of an image based on those characteristics of the image.

2.2 Image Generation in Machine Learning: discuss the intrusive nature of image generation as technology evolves for misleading information and the subjectivity of the technology. Discuss previous research involving GANs and the principles of StyleGAN3.

2.3 GAN Detector: a review of the background of image authenticity discrimination techniques, and the connection with the discriminator of GAN.

3 Methodology
Overview of the research design:
Aims and Objectives: a brief description of the main aims and objectives of the study, e.g., to assess human judgement of the authenticity of real versus generated images.
Overall research methodology: an overview of the basic structure of the study, including the design of the experiments, data collection methods, and analysis methods.

3.1 stylegan3: Explain why styleGAN3 was chosen as the image generation tool, including its unique advantages and applicability. Describe in detail the process of generating images using styleGAN3, including the dataset used, model parameters, and the type of images generated.
3.2 Calculating Metrics: Describe how StyleGAN3's discriminator assesses image authenticity and what metrics will be extracted for analysis.
3.3 Human Pilot Study: Describes the procedure for conducting a human pilot study.
3.4 Thematic analyses: outlines the plan for comparing and contrasting human responses with AI assessments, including qualitative and quantitative methods.

4 Implementation 
4.1 Stylegan3's process for extracting data for d
4.2 Calculating metrics: describes how StyleGAN3's discriminators will assess image authenticity and which metrics will be extracted for analysis.
4.3 Table of results
4.4 A short analysis

5. A Project Write Up 
Document the experiment from setup to execution, including any challenges faced and how they were overcome.
5.1 Human Pilot Study:
5.1.1 Human Visual Cognition Context
5.1.2 Problem Design.
By observing and evaluating details with reference to previous literature, participants can more accurately judge the authenticity of an image. This approach is not only applicable to traditional portraits, but also to AI-generated images such as StyleGAN3, which allows for a more comprehensive understanding of the differences in human perceptions of the authenticity of different types of images.

5.2 Summary Discussion


6 Evaluation and analysis
A detailed description of the methods used to assess human and AI performance, including the statistical analyses used and the assessment criteria.
6.1 Interview three people, detailed interview questions to be defined
6.2 Thematic analysis - several directions

7. Discussion and future work Reflection & shortcomings
Reflect on the findings of the study and discuss their implications for AI and human perception. Acknowledge the limitations of the research and suggest directions for future research.
Analyse the points as directions for specific optimisation of GAN and GAN detectors.

8 Conclusion
Summarise

9. bibliography (citations in Harvard style)


