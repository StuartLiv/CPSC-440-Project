# CPSC 440 Final Project - Autoencoder for Emergent Super-resolution
Joan Weng, Stuart Livingstone, & Ziven Anderson

## File Structure
### `datasets` 
The `datasets` directory contains various formatted image datasets we created based on the Kaggle image sources below. The actual dataset used in all our research is `medset_multisize`. This dataset contains a directory called `color` containing original 256 x 256 color images from the Kaggle dataset, randomly re-ordered and numbered from 1 to 12000. The directory called `gray` contains the same images with the same numbering scheme where image j in `gray` is a decolorized version of image j in `color`. There are also directories `gray128`, `gray64`, and `gray32` containing these same numbered grayscale images downsampled to 128 x 128, 64 x 64, and 32 x 32 respectively.

### `image-preprocessing`
This directory contains a series of Jupyter notebooks that were run offline on the raw Kaggle datasets to generate the formatted datasets as described above.

### `models`
This directory contains Jupyter notebooks which were used to train our various models. Pytorch model parameters are also stored in this directory. To train or use specific models, we recommend clicking the "Open in Colab" button at the top of each notebook.

## Dataset Sources
smallset: https://www.kaggle.com/datasets/theblackmamba31/landscape-image-colorization
medset: https://www.kaggle.com/datasets/ankit1743/skyview-an-aerial-landscape-dataset (resizing, decolorization, and organization done by us)
largeset: all images from smallset, plus all images from medset (resizing, decolorization, and organization done by us)
