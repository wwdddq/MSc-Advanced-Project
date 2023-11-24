# Week4
This week was mostly spent testing the StyleGAN3 portion, as well as looking at two pieces of literature that have a lot of relevance to my research.

## Tech

In the last week, I was performing basic tests on D output data using a pre-trained model of the FFHQ dataset.

We found that the output scores of D ranged from -1 to 1, which is different from the general expectation (that D should be scored between 0 and 1, and that closer to 1 indicates a more realistic image).

By further testing the ffhq dataset, we unexpectedly found that images are more likely to be considered real when the output of D is close to 0, and are considered generated when the output is close to 1.

Based on this basic test, I tried to perform some basic tests on all the existing pre-trained models of StyleGAN3 using different datasets.
- Datasets Source: https://github.com/justinpinkney/awesome-pretrained-stylegan3/blob/main/README.md

Here are the transcripts of the tests

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

The test results show that the discrimination of D has an error much different from the underlying theory for different datasets. This issue is reserved for next week's meeting with the tutor.

## Literatures

### Seeing is not always believing: Benchmarking Human and Model Perception of AI-Generated Images

Key Finding:

Impact of AIGC Background on Detection: Individuals with a background in AI-generated content (AIGC) were slightly better at recognising AI-generated images, improving by 3.7% over those without such a background.

Difficulty in distinguishing between image categories: The difficulty in distinguishing between true and false images varied by category. Subjects were more accurate at recognising images from the "Multiple People" category compared to the "Objects" category.

COMMON PROBLEMS WITH ARTIFICIAL INTELLIGENCE-GENERATED IMAGES: Common flaws in AI-generated images include detail and smoothness issues, which make it difficult to describe obvious flaws.

Model Evaluation: This study introduces MPBench, a method for comprehensively evaluating the ability of AI models to distinguish between AI-generated images and real images using large datasets.

Model Performance Variation: Model performance varies greatly depending on the characteristics of the training and validation datasets, highlighting the importance of diverse datasets to improve accuracy.

Best Model Performance: The ConvNext-S model trained using dataset set D was found to be the most effective model for detecting fake images, but still had a 13% failure rate.

Advances in Image Generation Models: Advanced text-to-image synthesis methods outperform previous GAN-based models in terms of image fidelity and diversity.

Challenges for AI Algorithms in Fake Image Detection: Current AI algorithms still face significant challenges in false image detection, as evidenced by a fairly high false positive rate.

- I was very inspired by this paper, especially the way it compares the perceptual differences between humans and miracles.

### Seeing is Believing: Exploring Perceptual Differences in DeepFake Videos

Human visual and cognitive properties: Humans naturally tend to focus on facial features and other salient visual elements when visually recognising and processing information. Facial features such as eyes, nose, mouth, as well as expressions are often key factors for humans to recognise and understand images, especially to determine the identity and emotions of people. Therefore, when detecting DeepFake videos, users naturally focus on these areas to look for possible inconsistencies.

Limitations of DeepFake generation technology: although DeepFake technology has made great strides in mimicking and replacing facial features, there are still some technical limitations. For example, unnatural traces may appear in details such as the edges of the hair and the alignment of the eyes or lips. These limitations lead to visual inconsistencies that become important clues for detecting DeepFake.

Experimental data and user feedback: the research methods in the paper include user surveys and analysis of eye-tracking data. Through these methods, the authors were able to collect data on the areas that users naturally focus on when watching videos. The user feedback and eye-tracking data revealed the specific areas they tended to focus on when detecting DeepFake.

COMPARISON WITH EXISTING LITERATURE: The existing literature on human visual perception and DeepFake detection also provides theoretical support for the selection of these visual cues. Previous research has shown that when making visual truthfulness judgements, people pay particular attention to areas that are considered key factors in the expression of identity and emotion in everyday experience.

- These underlying visual cues used in this article were informative for my research.
