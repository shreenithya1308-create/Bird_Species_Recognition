# PS-37: Bird Species Recognition Using Deep Learning

## Project Overview
This project implements a deep learning-based bird species recognition system using transfer learning with ResNet-18. It evaluates classification using original bird images and bounding-box-cropped images from the CUB-200-2011 dataset.

## Objectives
- Classify bird images into 200 species.
- Apply transfer learning using a pretrained ResNet-18 model.
- Compare original-image and cropped-image classification performance.
- Evaluate the models using accuracy, precision, recall, and F1-score.

## Dataset
**CUB-200-2011 (Caltech-UCSD Birds-200-2011)**

- Total images: 11,788
- Number of species: 200
- Official training images: 5,994
- Official test images: 5,794

The dataset is not included in this repository. Obtain it from an authorized source and follow its applicable terms of use.

## Methodology
1. Load and prepare the dataset and labels.
2. Resize images to 224 × 224 pixels.
3. Normalize images using ImageNet statistics.
4. Fine-tune a pretrained ResNet-18 model.
5. Train and evaluate original-image and cropped-image models.
6. Compare classification metrics.

## Results

| Metric | Original Images | Cropped Images |
|---|---:|---:|
| Accuracy | 65.98% | 76.49% |
| Macro Precision | 67.70% | 77.91% |
| Macro Recall | 66.27% | 76.60% |
| Macro F1-score | 65.77% | 76.21% |

The cropped-image pipeline achieved an accuracy improvement of **10.51 percentage points** in this experiment. The two experiments used different learning-rate schedules, so this improvement cannot be attributed to cropping alone.

## Tools and Technologies
- Python
- PyTorch
- Torchvision
- Google Colab
- ResNet-18
- CUB-200-2011 dataset

## Repository Contents
- Jupyter Notebook: implementation and evaluation
- Project report: methodology, experiments, and findings
- Result images: performance charts and prediction examples, if included

## How to Run
1. Open the notebook in Google Colab.
2. Download and extract the CUB-200-2011 dataset.
3. Update the dataset path to match your environment.
4. Install any missing dependencies.
5. Run the notebook cells in order.

## Conclusion
The project demonstrates the use of transfer learning for fine-grained bird species recognition. In the conducted experiments, the cropped-image pipeline achieved better classification metrics than the original-image pipeline.

## Author
Nithya  Shree M
SRM Institute of Science and Technology, Tiruchirappalli  
Academic Year: 2026–2027
