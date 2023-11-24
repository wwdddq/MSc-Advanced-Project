# Week2
This week was spent deepening some initial ideas and learning about technology

## Tech
- https://levelup.gitconnected.com/training-a-stylegan3-in-colab-gan-create-nft-6dd119774644
- https://blog.paperspace.com/stylegan3-gradient-notebooks/
- Tried to run StyleGAN3, but it didn't work!

## Literatures
Looked at some literature

### Learning to See: You Are What You See 

Paper brief .

This paper describes a visual tool for exploring bias in artificial neural networks and provides mechanisms for manipulating real-world representations of specific training. The tool explores and manipulates these representations in real time and reflects on the relationship between artificial neural networks and human-constructed meaning with a specific creative perspective.

Background: The aim of this study is to use convolutional artificial neural networks as a reflection of our own self-affirming cognitive biases, demonstrating the importance of training data for model prediction by exposing and amplifying learning biases in artificial neural networks.

Past Programme: Past research approaches have not provided real-time, interactive systems for creative expression and have lacked attention to the potential of deep learning systems as tools or instruments for human-computer collaboration.

Thesis Motivation: The motivation for this research is to enable real-time, interactive systems for creative expression by creating visual tools and enabling humans to have continuous, meaningful control over the generated deep neural networks. By using deep learning techniques, the authors hope to explore the potential of deep learning in the field of visual tools and fill the gaps in current research.

Methods.

a. Theoretical Background.

The authors developed a vision tool called "Learning to See" to explore bias in artificial neural networks. The tool uses artificial neural networks to predict real-time camera inputs, enabling real-time exploration and manipulation of representations. The authors used the tool to create interactive installations and video works. They emphasise the importance of continuous and meaningful human control when developing generative deep neural networks for creative expression.

b. Technical Track.

The authors used a pix2pix-based network architecture for pairwise image transformation. They modified this architecture to produce higher resolution images and allow real-time manipulation of parameters. Unlike traditional pix2pix, they provide only the target image for training and use preprocessing transformations to compute the input image on-the-fly. They also used data augmentation during training to encourage the network to generalise rather than memorise data. The network was trained with a batch size of 4 for 500,000 iterations.

Results.

a. Detailed Experimental Setup.

The methodology described by the authors involves training a neural network to reconstruct realistic images from fuzzy, abstract, grey input images. The network is trained using a variety of operators with randomly varying parameters, such as scaling the target image to a random size between 100% and 130% of the desired image size, random cropping, horizontal and/or vertical flipping, converting to greyscale images, downsampling and upsampling using filtering, and applying random brightness and contrast adjustments. The network learns from large image datasets, allowing it to capture rich representations and details across the entire dataset. During inference, the camera input is preprocessed into a blurry, abstract, grey image using the same preprocessing map and the learned features are used to reconstruct a realistic image.

b. Detailed experimental results.

The method differs from neural style migration in that it produces a predictive model rather than optimising the output image. This makes real-time processing possible. The method also differs from newer style migration methods that use multiple reference style images because it combines knowledge from the entire dataset and does not require manual blending of weights. The authors believe that deep learning has significant potential in a variety of areas, including helping to produce creative output in a real-time continuous manner. They also emphasise the importance of understanding the impact of training data distribution on neural network predictions. In addition, they emphasise the need to be sensitive to possible biases in artificial neural networks and human perspectives.

### Trust It or Not: Effects of Machine-Learning Warnings in Helping Individuals Mitigate Misinformation

**Key Insights**:
Effects of Warnings on Fake News Detection: Fact-checking warnings improve the detection rate of fake news compared to machine-learning warnings. Machine learning graph warnings improve the sensitivity of distinguishing fake news from real news, but do not necessarily improve trust.

Computational detection of fake news: Computational approaches focus on analysing textual and multimodal features for fake news detection.

Signal Detection Theory (SDT) Application***: SDT was used to understand individuals' reactions to fake news detection, measuring their sensitivity and bias.

Machine Learning Warning Experiments: Two experiments were conducted to assess the impact of machine learning warnings on individuals' willingness to recognise, detect, and share fake and real news.

Sharing decisions: Participants were generally wary of sharing news and were more likely to share fake news than real news.

Impact of warnings: Fact-checking warnings influenced participants' decisions when news sources were included, but disappeared when news sources were excluded.

### The role of artificial intelligence in disinformation

The gist:
The role of artificial intelligence in disinformation: artificial intelligence systems play an important role in both the creation of realistic disinformation content and the dissemination of disinformation.

Deep forgery: AI technologies, especially deep learning and generalised arithmetic networks (GANs), facilitate the creation of deep forgeries that greatly affect the authenticity of content.

Dissemination techniques: AI-powered micro-locations and social bots effectively disseminate disinformation and manipulate online discourse and public opinion.

Ethical implications: the use of AI in disinformation raises ethical issues that challenge human dignity, autonomy, democracy and peace.

Detection techniques: Various AI techniques have been developed to detect disinformation, but their effectiveness is limited by the large number of labelled datasets required and the biases in these datasets.

Challenges in defining disinformation: Distinguishing between misinformation and disinformation is complex, as the intent of the sharer is a key factor.

Transparency and Interpretability: AI systems lack clarity and transparency in policing content, which can lead to over-censorship of content.

Risk of over-censorship: detection of false information by AI systems may lead to over-censorship of false positives and false negatives, affecting freedom of expression.

### Explaining and Harnessing Adversarial Examples

Synopsis: Discusses the finding that several machine learning models, including state-of-the-art neural networks, are vulnerable to adversarial examples. The main reason for this vulnerability is proposed to be the linear nature of these models.

RELATED WORK: Reviews previous research demonstrating various properties of neural networks and their vulnerability to adversarial examples. Explore the limitations of existing models in terms of their vulnerability.

Linear explanations for adversarial examples: explain in detail why linear models, despite their simplicity, are vulnerable to adversarial examples. Discusses how higher dimensional spaces and linearity contribute to this vulnerability.

Linear perturbations in non-linear models: explores the hypothesis that neural networks are too linear to resist linear adversarial perturbations. Discusses the design of neural networks and their inherent linearity.

Adversarial training and weight decay for linear models: compare adversarial training and weight decay in the context of logistic regression. Analyses how adversarial examples are generated and their implications for simple linear models.

Adversarial training for deep networks: explores the potential of adversarial training to improve the robustness of deep neural networks. Discusses the effectiveness of this approach in enhancing the model against adversarial perturbations.

Different types of model capacity: examine how adversarial instances challenge our intuitions about high-dimensional spaces and model capacity. Explore the resistance of different models (e.g. RBF networks) to adversarial examples.

Generalisation of adversarial examples: investigate why adversarial examples generalise across different models. Propose an explanation for this phenomenon based on the linear nature of the models.

Alternative hypotheses: consider and refute alternative hypotheses about the existence of adversarial examples. Discuss the potential role of generative training and model ensembles in resisting adversarial examples.

Summary and Discussion: summarise the key findings and observations of this paper. Discuss the implications of these findings for the design and training of machine learning models.

## Project Progress.

Initial project direction after meeting with mentor

"Criteria by which a human judges the authenticity of an image, versus a machine"

Using GAN's own mechanisms to represent the subject of misrepresentation - generators and discriminators

Data counted by GAN discriminators - how to judge the authenticity of generated images

Hands-on experiments - human subject study - how a human generates an image to judge the veracity of the generated image

Comparing human given representations or answers with machine computed data (data given by d), what are the differences - Perceptual differences

Thematic analysis - commonalities leading to ideas for future discussion

