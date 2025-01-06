# U-Net for Street Scene Segmentation (CamVid Dataset)

## Project Overview
This project explores the use of the U-Net architecture for semantic segmentation on the CamVid dataset, a collection of street video frames. U-Net, originally proposed for biomedical image segmentation, is adapted here to tackle real-world urban scene understanding. This work aims to improve segmentation accuracy and experiment with architectural enhancements such as attention mechanisms.

## Dataset
The [CamVid dataset](http://mi.eng.cam.ac.uk/research/projects/VideoRec/CamVid/) consists of labeled frames extracted from driving videos. It is widely used for benchmarking segmentation models in urban environments. The dataset includes:
- **Input**: RGB images of urban street scenes.
- **Labels**: Pixel-wise annotations for 32 semantic classes (e.g., road, building, pedestrian, sky), with some classes being heavily imbalanced.

The dataset is particularly relevant for applications like autonomous driving, urban planning, and real-time traffic monitoring.

## Model Architecture
The project utilizes the U-Net architecture, a fully convolutional neural network designed for segmentation tasks. Key features include:
- **Encoder-Decoder Structure**: Captures high-level context and restores spatial resolution for pixel-wise predictions.
- **Skip Connections**: Preserve spatial information by connecting encoder and decoder layers.


## Training Details
- **Framework**: PyTorch
- **Optimization**: Adam optimizer with learning rate schedulers to ensure convergence.
- **Challenges**:
  - Imbalanced class distribution
  - Tuning hyperparameters for optimal performance


## References
- **Original U-Net Paper**: ["U-Net: Convolutional Networks for Biomedical Image Segmentation"](https://arxiv.org/abs/1505.04597) by Olaf Ronneberger, Philipp Fischer, and Thomas Brox.
- **CamVid Dataset**: [Dataset Description and Access](http://mi.eng.cam.ac.uk/research/projects/VideoRec/CamVid/)
