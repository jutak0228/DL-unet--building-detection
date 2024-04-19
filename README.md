# DL-unet-building-detection
Object detection for building through UNet algorithm

## U-Net
U-Net is a semantic segmentation method proposed in U-Net: Convolutional Networks for Biomedical Image Segmentation presented at MICCAI (Medical Image Computing and Computer-Assisted Intervention) 2015. Semantic Segmentation is a method proposed in MICCAI (Medical Image Computing and Computer-Assisted Intervention) 2015.

Semantic Segmentation is a deep learning method that labels each pixel in an image. As the name implies, U-Net has a U-shaped network structure.

U-Net does not have a total coupling layer, but is a network composed of convolutional layers. U-Net has an almost symmetric Encoder-Decoder structure, where the down-sampled feature maps are up-sampled by the Decoder through pooling of the Encoder. U-Net introduces concatenation of the feature maps output at each layer of the Encoder to the corresponding feature maps at each layer of the Decoder, which is called a skip connection.

In this project, we will use deep learning to extract buildings from satellite images. The procedure is as follows:

- (1) Preparation of dataset
- (2) Learning of U-Net
- (3) Evaluation of U-Net

## Approach
- Step 1. First, install the AWS Command Line Interface (AWS CLI) via pip in order to download data from the SpaceNet dataset.
- Step 2. Next, we will prepare for training. First, we will map the images to the location information of the buildings for learning.
- Step 3. Segmentation is performed on the learned U-Net using satellite images from the U-Net evaluation test data.
