# Image Colorization using GANs

This is my deep learning project in which we performed image colorization on B/W images using GANs.



## Motivation
- Recolorizing and restoring old photos is a painstaking process when done manually through some old editing software.
- One solution to this problem is using GANs for recolorizing and restoring of old projects.
- Colorizing black and white images with deep learning has become an impressive showcase for the real-world application of neural networks in our lives.
## Design
- GANs include 2 major components:
1. Generator
2. Discriminator
## Design
- GANs include 2 major components:
1. Generator
2. Discriminator
## Methodology
Dataset: Our dataset will consist of 3000 RGB images from various domains (mountains, forests, cities, etc..). We will convert these RGB images to grayscale which will act as labels for our model.

1. For a single step, we ran the generator once and the discriminator twice.
2. For the discriminator, maximizing its loss would mean classifying generated images accurately as well as producing a good probability (closer to 1.0) for images from the dataset.
3. The generator, by minimizing its loss, improves itself to such an extent that it can fool the discriminator. Fooling the discriminator means that the discriminator will produce probabilities (closer to 1.0) even for generated images.
4. We'll train the discriminator in such a manner that it will output probabilities closer to 1.0 for real images (from our dataset) and output probabilities closer 0.0 for images coming from the generator.
5. If the discriminator is "smart" enough, it will output probabilities closer to 1.0 for real images (coming from our dataset). So, we are training our generator to forge such realistic images which will make the discriminator output probabilities closer to 1.0 even when the images are forged (not from our dataset, but from the generator.
## Future Work
- By using this project, we can convert old b/w photo of our grandparents into colorized photo making that picture more memorable.
- We also aim to carry our work further by colorizing the videos too.
- Lastly, we want our model to be deployed on web platform, so that it is accessible for users worldwide.
