# Week3
Still reading the literature this week and discussing the code section with my tutor. Successfully solved the problem with the help of my mentor and ran out of D data. Next step is to try testing with other datasets.

## Tech
See StyeGAN3-D folder for details

## Literatures

### Detecting Fake News With Machine Learning

INTRODUCTION: Discusses the prevalence of fake news in the digital age and its potential harms, such as misleading the public and creating political divisions. Introduces current approaches to tackling fake news, such as manual vetting and blacklisting of unreliable sources, and the limitations of these approaches.

BACKGROUND: Provide an overview of the machine learning approach used in the study, highlighting its potential for detecting fake news through language pattern analysis. Compare the approach to related fields such as spam detection and stance detection in news articles.

METHODS: Details the dataset used from Kaggle, which contains both real and fake news sets. The data cleaning and vectorisation process is explained, including techniques such as CountVectorizer, TF-IDF Vectorizer and One-Hot representation.

Applied Classifiers: discusses the application of various classifiers such as Polynomial Naive Bayes, Passive Aggressive Algorithms, and Long Short-Term Memory (LSTM) models. The specific features and processes of each classifier are presented.

RESULTS: Present the results of applying these classifiers, including accuracy rates and confusion matrices. Compare the effectiveness of the different classifiers in identifying fake news.

CONCLUSION: Summarises the research findings that various machine learning algorithms are effective in detecting fake news. Future research directions such as testing more models and applying the framework to different platforms are proposed.

### GAN-generated Faces Detection: A Survey and New Perspectives

INTRODUCTION: Discusses the development of GAN and its application in generating highly realistic faces that pose challenges for fake face detection. The social issues and negative impacts of GAN generated faces in various scenarios such as fake social media accounts are discussed.

GAN Generation of Highly Lifelike Faces: a brief overview of the mainstream methods for generating high-quality faces using different GAN models.

GAN-Face Detection Methods
   - Deep Learning Based Approaches: Examines the use of deep neural networks to discriminate fake faces.
   - Physics-Based Approaches: Discusses methods for recognising GAN faces by checking the inconsistency of physical world representations.
   - Physiological-based methods: Explore methods for detecting synthetic faces based on biological and physiological inconsistencies.
   - Human Visual Performance: Analyse the effectiveness of human perception in recognising GAN-generated faces.

Datasets and Performance Evaluation: Survey of popular datasets and key evaluation metrics used in GAN face detection research.

Related Surveys: Review other surveys related to GAN face detection and related areas such as deformed face and manipulated face detection.

Future Directions: Discusses the expected development of GAN models and the continued need for effective detection methods, taking into account challenges such as adversarial attacks and data imbalance.

Conclusion: summarises recent advances in GAN face detection, highlighting the importance of the field and the need for continued research.

### Discriminator Synthesis: On reusing the other half of Generative Adversarial Networks

Introduction: Introduces the concept of GANs and their impact on art and computer vision. Focuses on the generator component of GANs, while discriminators are often neglected after training.

Discriminator Dreaming: presents the new idea of using features learnt by the discriminator to modify and generate images, called "discriminator dreaming". The inspiration and theoretical foundations of this approach are described in detail, citing previous research in GAN and art applications.

METHODOLOGY AND IMPLEMENTATION: Explains the technical process of "Discriminator Dreaming", including the extraction of intermediate features from the discriminator of StyleGAN2. Discuss practical applications, such as using the method for style transfer and image projection.

EXPERIMENTAL RESULTS: Presents preliminary results using various pre-trained models and discriminator layers. Includes visual examples demonstrating the effect of the method on different images and resolutions.

Limitations and future work: discusses the current limitations of the algorithm, such as slow synthesis speed and the potential need for further refinement. Potential areas for future research and improvement are suggested.

Ethical Considerations and Acknowledgements: discusses the intended artistic uses of the method and the ethical implications of using pre-trained models.

### Amplifying The Uncanny

INTRODUCTION: Addresses the rise of deep fakes and the controversy surrounding them, particularly their use in areas such as pornography and the creation of false online identities.

BACKGROUND: Discusses machine learning, GANs and their use in deep fakes and art creation. Introduces the concept of fine-tuned GANs and highlights the potential of discriminator networks in generating novel artistic output.

Inverting the objective function: explains the process of inverting the GAN objective function, with a particular focus on optimising the generator to produce images classified as fake by the discriminator.

Maximising Likelihood: discusses the theoretical implications of maximising the likelihood of data in a GAN and its artistic potential.

Divergence, Convergence, and Collapse: describes the stages of the fine-tuning process and its effects on the generated images, leading to varying degrees of spooky effects.

Examining Peak Mystery: explores specific iterations of the model that demonstrate the most obvious weirdness.

Explore different states: discuss the variations in the results of the fine-tuning process at different stages of model training.

Conclusion: summarise the findings and reflect on the artistic and perceptual implications of the work.

- Information related to the Discriminator

- **Role of the discriminator**: in a traditional GAN, the discriminator is optimised to classify real data as real and generated data as fake, while the generator tries to trick the discriminator.
- **Fine-tuning GAN**: the paper highlights the potential of discriminator networks in art creation. By freezing the weights of the discriminators and using them in conjunction with the generators, the paper explores novel outputs that are significantly different from images generated by typical GANs.
- **Reverse Objective Function**: instead of optimising the generator to produce realistic images, the generator is fine-tuned to produce images that the discriminator classifies as false. This approach produces a range of artistic outputs that amplify the mysterious nature of machine-generated images.

