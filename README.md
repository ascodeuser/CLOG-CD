## CLOG-CD: Curriculum Learning based on Oscillating Granularity of Class Decomposed Medical Image Classification


## Introduction

We introduced the CLOG-CD model to improve the generalisation of medical image classification and address overlapping class distributions. This approach combines an anti-curriculum learning strategy with class decomposition at different levels of granularity. The model starts training at the highest granularity level, where the maximum number of sub-classes is present, and gradually fine-tunes the learned knowledge to lower levels. Here, the class decomposition method helps the model first learn specific features by simplifying the dataset’s complex structure, defining clear boundaries between classes, and then moving gradually to the generic features. This makes it easier for the model to understand relationships between examples and reduces the impact of overlapping class distributions.

The model was evaluated on four different imbalanced medical image datasets, such as Chest X-ray (CXR), brain tumour, digital knee X-ray, and histopathology colorectal cancer (CRC), using two pre-trained networks, ResNet-50 and DenseNet-121, as the backbone for CLOG-CD. 

The results with ResNet-50 show that CLOG-CD has the ability to improve classification performance with an accuracy of 96.08% for the CXR dataset, 96.91% for the brain tumour dataset, 79.76% for the digital knee x-ray, and 99.17% for the CRC dataset, compared to other training strategies. In addition, with DenseNet-121, CLOG-CD
has achieved 94.86%, 94.63%, 76.19%, and 99.45% for CXR, brain tumour, digital knee x-ray, and CRC datasets, respectively.

### Datasets Used
CURVETE has been evaluated on three distinct medical image datasets:
1. **Chest x-ray Dataset**. [here](https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database)
2. **Brain Tumor Dataset**. [here](https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection)
3. **Digital Knee X-ray Dataset**. [here](https://data.mendeley.com/datasets/t9ndx37v5h/1)
4. **Colorectal cancer Dataset**. [here]( https://zenodo.org/records/1214456#.YxQp63ZBxPZ)

### Requirements
To run this project, you'll need the following dependencies:
- **Python**: 3.8
- **TensorFlow**: Version 2.13
- Other required libraries: 
  - `NumPy`
  - `Matplotlib`
  - `scikit-learn`
  - `OpenCV`

 ## Model Overview
 
<p align="center">
  <img src="https://github.com/ascodeuser/CLOG-CD/raw/main/images/CLOG-CD_Model.png" alt="Model Figure" width="600"/>
</p>

### Citation
If you use this code or method in your research, please cite the following paper:

**CLOG-CD: Curriculum Learning based on Oscillating Granularity of Class Decomposed Medical Image Classification." Manuscript submitted for publication, IEEE Transactions on Emerging Topics in Computing, 2023.**

*Asmaa Abbas, Mohamed Medhat Gaber, and Mohammed M. Abdelsamea*


