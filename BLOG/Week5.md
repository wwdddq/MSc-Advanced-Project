# Week5
In this week's meeting with my mentor, I brought up an issue I discovered last week.

Also, I noticed a comment on GitHub while searching for related content this week.

- https://github.com/NVlabs/stylegan3/issues/180

This comment pointed out that different datasets and models result in different output scores from the StyleGAN discriminator, with higher scores indicating that the image is real and lower scores indicating that the image is a forgery.

After a discussion with my tutor, I decided to select a dataset with a larger number of data comparisons and try to find some patterns in it.

I chose the MetFaces dataset because most of the previous research was based on FFHQ face detection, but I wanted to go for artistic images to explore the difference between human and machine perception. One more thing is that MetFaces is portraits of people in real paintings, and this dataset is also officially released by Nvidia, which has some advantages in standard type.

During the analysis, I generated 100 synthetic images of portrait paintings of people using the StyleGAN3 pre-trained model based on Metfaces and numbered them as seed0001-0100.Similarly, I randomly selected 100 real images of portrait paintings of people from the metfaces dataset and numbered them as MF1-100.Subsequently, I used a discriminative model on these 200 images one by one using the discriminator and recorded the results.

I ranked the data from lowest to highest and the results can be seen in the link below. (Colours marked in the graph are the images selected as experimental samples)
- https://github.com/wwdddq/MSc-Advanced-Project/blob/main/StyleGAN3-D/data-D.pdf

I processed the scores for the 200 valid data points and the results show an average score of approximately -1.34, ranging from a low of -5.24 to a high of 3.31. It is worth noting that 82% of the scores are negative, indicating that whilst the majority tends to be negative, there is still a large portion of the overall distribution of scores that are below zero.

This leads to the conclusion that, despite the discrepancy between the discriminator's output scores and its underlying theory, these scores exhibit discernible patterns in individual datasets. Specifically, in the model based on the MetFaces dataset, lower discriminator (D) output scores indicate a higher likelihood of generating an image, and vice versa.

Using the theoretical framework of score thresholding in computational metrics, I established a score threshold (the median score of the D output of these 200 images) to distinguish between real and generated images in this dataset. Thus, in my experimental setup, images with scores higher than -1.6163 were categorised as real images, while those with scores lower than -1.6163 were regarded as forgeries.

I extracted 20 images from the table. These 20 images were 10 originally real and 10 originally generated respectively. out of 10 real images, five were considered fake by the machine. And five of the 10 generated images were also images that the machine thought were real.

At the end of the week, I ran a short questionnaire with these 20 images, but people fed back that there were a bit too many images. So I further randomly selected 10 more images from these 20 images and the results are below.

![MSc-Advanced-Project](https://github.com/wwdddq/MSc-Advanced-Project/blob/main/BLOG/img/paper_img.001.jpeg)
