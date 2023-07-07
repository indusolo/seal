# SEAL
### Data Generation With Structure Enforcing Adversarial Learning
### This paper is accepted for presentation at International Conference on Image Processing 2023 (ICIP23)
#### Pytorch code, datasets and implementation details are shared here
The hardware and software setup for the experiments are as follows:
* CPU - Intel® Xeon® CPU E5-2630 v4 2.20 GHz
* GPU - Nvidia Quadro RTX 8000, GPU memory - 48 GB, CUDA cores - 4608, python version 3.10.4
* NumPy version 1.22.4
* pytorch version 1.12.1
* torchvision version 0.13.1
* sklearn version 1.1.2. 
The parameter selection is as follows: 
* latent space dimension is selected between 32 to 64
* learning rate is chosen between 0.0002 to 0.0015
* activation functions used are ReLU, leaky ReLU and sigmoid
* the encoder-decoder has 2 hidden layers
* cGAN generator, discriminator has 3 hidden layers
* MLP classifier has a three layer architecture 
* $\lambda_{struct}, \lambda_{1,..,3}$ are set as 0.5, 1.0 respectively
## Datasets 
Datasets used in the experiments are shared in the dataset folder
- Wafer Dataset - 52x52 single channel images, 10 classes
- Imbalanced train dataset
- Imbalanced and balanced test dataset
- KMNIST Dataset - 28x28 single channel images, 10 classes
- Imbalanced train dataset
- Imbalanced and balanced test dataset

![alt text] (http://localhost:8080/files/SRGAN/Waferfiles/Genimages_E2ECGAN_64LD3.png)
- http://localhost:8080/files/SRGAN/Waferfiles/Genimages_E2ECGAN_64LD1.png
