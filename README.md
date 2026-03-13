# VocEd — Cytology Segmentation Course

Applied deep learning for cytology image segmentation.
**Goal:** Predict the nucleus-to-cytoplasm (N/C) ratio using convolutional neural networks.

## Labs

| # | Notebook | Topic | Open in Colab |
|---|---|---|---|
| 01 | Exploratory Segmentation | Grayscale thresholding, Dice score | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/emilsar/VocEd/blob/main/01_exploratory_segmentation.ipynb) |
| 02 | Bayesian Optimisation | Auto-search for best thresholds, train/test split | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/emilsar/VocEd/blob/main/02_bayesian_optimisation.ipynb) |
| 03 | Image Processing | Denoising, morphological opening/closing | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/emilsar/VocEd/blob/main/03_image_processing.ipynb) |
| 04 | Pixel Classifiers | k-NN on RGB colour vectors | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/emilsar/VocEd/blob/main/04_pixel_classifiers.ipynb) |
| 05 | Convolutions & CNN | Manual convolution, minimal PyTorch CNN | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/emilsar/VocEd/blob/main/05_convolutions.ipynb) |
| 06 | U-Net | Encoder-decoder with skip connections | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/emilsar/VocEd/blob/main/06_unet.ipynb) |
| 07 | N/C Ratio Pipeline | End-to-end clinical evaluation | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/emilsar/VocEd/blob/main/07_nc_ratio_pipeline.ipynb) |

## Dataset

`imagedata/X/` — 200 RGB images, shape `(3, 256, 256)`, float32 `[0, 1]`
`imagedata/y/` — 200 segmentation masks, shape `(256, 256)`, labels: `0` background · `1` cytoplasm · `2` nucleus

## Textbook

Course textbook: [cvmath.club](https://cvmath.club/)
