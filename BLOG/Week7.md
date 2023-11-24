# Week7
This week's work goal is to read three pieces of literature and write an outline for a paper

and Completion of web page refinement.

## Literature

### Landscape Art Image Style Reconstruction Algorithm Based on Machine Learning

Abstract: This paper discusses the use of recurrently consistent Generative Adversarial Networks (GANs) with attentional mechanisms for image style reconstruction, especially for landscape art images. It emphasises on enhancing specific features of an image for better style transformation results.

Synopsis: The paper highlights the rise of Artificial Intelligence and Deep Learning, especially in non-realistic rendering. The paper highlights the growing importance of image style shifting in various domains, from personal expression on social media to commercial applications such as film and animation.

Artistic image style reconstruction: an overview of neural style transfer: This paper provides an overview of neural style transfer, a technique that uses convolutional neural networks to combine the content of one image with the style of another. The paper cites Gatys et al. who laid the groundwork for this field.

Algorithms for Stylistic Reconstruction of Landscape Art Images: the paper delves into the use of GANs for image style transformation, highlighting the challenges and opportunities of using these models to generate multi-view image transformations and automatic description generation.

CONCLUSION: The paper concludes with a discussion of the wide range of applications and research value of image style transformation techniques. This paper proposes a landscape image style transformation model that uses GANs with attentional mechanisms to augment specific features for improved stylisation.

## Mechanisms of Face Perception

Abstract: Face perception is thought to be a unique information stimulus, distinctive in the human brain and observed in macaques. One hypothesis suggests that the specificity of face processing is due to an obligatory detection process, which this paper aims to clarify and demonstrate through various experiments.

INTRODUCTION: This paper compares face recognition with object recognition, highlighting the need to recognise subtle differences in the presence of changes in position, illumination and occlusion. This comparison treats face perception as a microcosm of object recognition.

Mechanism review: this paper reviews the face processing process at different levels of computational theory, algorithms and neural implementations, and elaborates on the related mechanism issues in the face processing process.

Computer vision algorithms: face processing in computer vision is divided into detection, measurement and classification. Detection involves recognising the presence of a face, measurement involves distinguishing individual faces based on their features, and classification classifies faces based on attributes such as identity, gender and age.

ALGORITHM REVIEW: A review of algorithms that provide insights into possible biological mechanisms of face recognition, such as Viola-Jones and Sinha's algorithm and the Eigenface algorithm, is presented. A discussion of feature-based and holistic approaches is included.

Human Behavioural and Functional Imaging: Behavioural studies and functional imaging data such as activation of the fusiform gyrus and fusiform face area (FFA) in face perception tasks are discussed. This section highlights the uniqueness of face processing in the brain and presents a unique stage of face detection.

Measurement and classification: The possibility of separate face measurement and classification systems in the human brain has been explored through fMRI studies that have shown that the occipital face area (OFA) and the FFA play distinct roles in face processing.

Monkey fMRI and single-unit physiology: details of the use of fMRI and single-unit physiology to study face-selective cells in monkeys and their role in detecting and processing faces as a whole. This section includes a discussion of the time course of anatomical specialisation and feature combination responses in human face cells.

FUTURE RESEARCH DIRECTIONS: the paper concludes with future research directions that question the uniqueness of face processing, its modular nature, and the implications of the detection-gating hypothesis for understanding face recognition and detection processing.

- The outline of the paper was written with reference to previously analysed literature, which is why my record of the literature read was written in chapters.

## thesisdraft

Title

A Comparative Study of Human and Artificial Intelligence in Perceiving Image Realism

Abstract

Provides a brief overview of the research question, which is how artificial intelligence discriminates between true and false images compared to human perception. Briefly describe the research methodology, including human studies, computational metrics, and thematic analyses. Highlights key findings, such as differences between human and AI judgements of image authenticity, and suggests implications for wider online disinformation.

1 Introduction

1.1 Motivation: the problem of misinformation in contemporary internet communication and the harm it causes is drawn from the hyper-conventionalisation of documentary films, with the characteristics of misinformation: no scientific basis/one-sidedness/intentional amplification. (US Election 2016) points out that most of the visual misleading information on the Internet is machine-generated. Humans can be misled by generated images, what about machines? To introduce the challenges of humans and machines for recognising the authenticity of visual content in contemporary society.

1.2 Objective:

Research question: to analyse the differences between humans and Generative Adversarial Networks (GANs) in judging the authenticity of portraits of people in paintings

Inspiration: the use of generative images by others as misleading information to get Trump elected as president in the 2016 US election

Artistic theme of special interest: the difference in perception between humans and AI in relation to portraits of people in paintings, e.g. a human judging whether a picture of a portrait of a person in a painting is real or generated might judge it in terms of colours, texture details, style of painting, etc., but what about GAN? And what are the factors by which the discriminator of GAN determines whether a picture is real or generated.

Objective of Technology Development and Application: to extract the authenticity result scores assessed by the discriminator of styleGAN3 for portraits of people in real paintings and portraits of people in generated paintings, and to analyse the results to derive the commonalities and differences. The purpose of this operation is to do human experiments with these pictures, i.e., whether a human and a machine agree on the authenticity judgement of the same picture, and to study the reasons for their agreement or disagreement. The goal of the application is to make human beings feel the influence of images on misleading information in the process of doing the experimental experience, as well as to warn people to keep their own subjectivity and not to be influenced by others who use the machine's subjectivity.

2 Background and related work

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


