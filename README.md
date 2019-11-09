# RiverGAN
Using Generative Adversarial Networks (GANs) to Develop Realistic River Satellite Imagery - **Akshat Gautam**

The RiverGAN was trained using a logic similar to PyTorch's original DCGAN (Deep Convolutional Generative Adversarial Network). The generator takes in a latent vector (z) of size 100, and outputs a 64x64x3 (RGB) image, while the discriminator takes in a 3-channeled 64x64 image and outputs a probability of the passed-in image being a satellite river or not, using the Sigmoid function, which yields a value from 0 to 1.

In this repository, there are two main notebook files:
- **River Image GAN (IPYNB)**: This Jupyter notebook contains the code for training the model, as well as the architectures for both the generator and discriminator networks. 
- **River From GAN (IPYNB)**: This Jupyter notebook takes the weights of the generator and discriminator, trained from the River Image GAN notebook, and has a script to utilize those weights to generate random river images of size 64x64. 

The data for this project was customly sampled from the Google Earth Engine program, and 1000+ images were snapshotted. Then, around 8-9 transforms were applied to each of these images in the data augmentation process, and the DCGAN was trained on around 10K+ images.


The weights for the generator and discriminator ('river_generator.pth' and 'river_discriminator', respectively) are too large to upload on GitHub. **Please e-mail me for any inquiries you may have regarding the full dataset, GAN weights, or training process.**
