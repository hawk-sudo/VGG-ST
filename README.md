# VGG-ST-RW-ROP-Classification
<p align="justify">
VGG-ST: A VGG-Swin Transformer-Based Model for RW-ROP Disease Diagnosis.
</p>
Project Status: [Completed]

### Objective
<p align="justify">
This project aims to detect Referral-Warranted Retinopathy of Prematurity (RW-ROP) using retinal images.
</p>

### Partner
<p align="justify">
Xinwei Luo, Songlin Zhao, Yong Chen, Gui-shuang Ying, Lifang He
</p>

### Methods Used
* Deep Learning
* Machine Learning
* VGG19
* Swin Transformer V2

### Technologies
* Python
* Jupyter
* Numpy
* OpenCV
* Pytorch

### Needs of this project
* Data Augmentation
* Data Processing
* Deep Learning Modeling
* Evaluation and Reporting

### Project Description
* CLAHE to enhance the image feature.
* Labeling image data according to the class (Normal or RW-ROP).
* Dividing data into train, test, and validation data.
* ROSE oversampling to generate the minority class (RW-ROP) images to handle class imbalance issues in the trainset.
* Data augmentation to increase the number of images for training.
* Data preparation includes changing images to arrays, resizing, and normalizing.
* Implementing VGG-ST to classify Retinal images.
* Train models and provide evaluation reports.

### Getting Started
1. Prepare the Pytorch >=2.0 version and Python >=3.6. Download and install this repo.
```
git clone https://github.com/hawk-sudo/VGG-ST.git
```
2. Move to this repo and install the environment.
```
conda env create -f rop.yaml
conda env create -f datapreprocess.yaml
```
Datapreprocess env is used for Data preparation. rop env is used for VGG-ST training and testing. 
3. Organizing the dataset. The dataset should be organized into the following format. We do not provide the dataset for privacy reasons.
```
root_directory/
├── class1/
│   ├── img1.jpg
│   ├── img2.png
│   ├── ...
├── class2/
│   ├── img1.jpg
│   ├── img2.png
│   ├── ...
├── class3/
│   ├── img1.jpg
│   ├── img2.png
│   ├── ...
└── ...

```
4. Launch the Jupyter Notebook and change the param according to your settings. First use the Data Preprocessing file to process the data, and then use VGGA-ST_Train and VGGA-ST_Test to train and test VGG-ST.

### Acknowledgements
This codebase is built based on the (https://github.com/huggingface/pytorch-image-models) and (https://github.com/Cadene/pretrained-models.pytorch.) Thank you!
