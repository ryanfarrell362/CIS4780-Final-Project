# CIS4780-Final-Project

To run the project, simply execute the codeblocks in the Jupyter Notebook in order
The codeblocks and their functionality are detailed below

- Install required library
- Declare imports and hyperparameters
- Load and preprocess CIFAR10 dataset
- Define generator model
- Define discriminator model
- Train models
- Save generator model
- Load generator model and create a batch of images (Mostly test block, can be skipped)
- Load generator model and generate 50k images (This will generate the set of images required to calculate a FID score)
- Save real CIFAR10 images in preparation of FID score calculation
- Calculate FID score
- Install required libraries for DDPM FID score
- Load DDPM model
- Save DDPM generated images
- Calculate DDPM FID score

Tweakable variables:

nEpochs - Default: 100, will determine how long training takes
nSnapshots - Default: 100, will determine how often snapshots of the generator model are taken (Every n epochs)
epochModel - Default 100, determines which pretrained model will be loaded to generate images

Of the pretrained models included in our repo, generator_epochs_100.pth is recommended to use for all purposes