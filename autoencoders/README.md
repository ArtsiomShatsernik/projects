## Implementation of Convolutional Autoencoder with PyTorch
This project implements a convolutional autoencoder designed to work with images of size 128x128 and three channels (RGB). The autoencoder compresses (encodes) images into a latent space representation of size 512 and then reconstructs (decodes) the images back to their original size.

The project uses the LFW (Labeled Faces in the Wild) dataset, specifically the lfw-deepfunneled subset for aligned face images and the lfw_attributes.txt file for attribute metadata.
Using the metadata, image transformations were applied, such as adding or removing smiles and glasses from the photos.

Best loss function on validation (MSE): 0.0011.

The architectural modifications that can be used to improve the model:
- VAE (Variational Autoencoder) - using probabilistic distributions in the latent space can make the model more stable and improve the quality of generated images by allowing more variety in the outputs.
- CAE (Conditional Autoencoder) - adding extra input data, like metadata or specific attributes, can help guide the image generation based on certain conditions (for example, adding or removing glasses or smiles).
