# RiverGAN
Using Generative Adversarial Networks (GANs) to Develop Realistic River Satellite Imagery

The RiverGAN was trained using a logic similar to PyTorch's original DCGAN (Deep Convolutional Generative Adversarial Network). The generator takes in a latent vector (z) of size 100, and outputs a 64x64x3 (RGB) image, while the discriminator takes in a 3-channeled 64x64 image and outputs a probability of the passed-in image being a satellite river or not, using the Sigmoid function, which yields a value from 0 to 1.

In this repository, there are two main notebook files:
- River Image GAN (IPYNB): This Jupyter notebook contains the code for training the model, as well as the architectures for both the generator and discriminator networks. 
- River From GAN (IPYNB): This Jupyter notebook takes the weights of the generator and discriminator, trained from the River Image GAN notebook, and has a script to utilize those weights to generate random river images of size 64x64. 
