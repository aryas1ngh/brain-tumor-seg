## Brain Tumor Segmentation using 3D U-Net

This repository contains code for brain tumor segmentation using a 3D U-Net architecture. The model is trained on magnetic resonance imaging (MRI) data with different modalities, including T1, T1-CE, T2, and FLAIR. The segmentation task involves identifying the tumor region in the brain scans. The dataset used is BraTS Challenge 2020, organized by Perelmann Med School, UPenn.

Kaggle dataset link (train + val) : [link](https://www.kaggle.com/datasets/awsaf49/brats20-dataset-training-validation)
BraTS Challenge : [link](https://www.med.upenn.edu/cbica/brats/)


1. Clone the repo:
```git clone https://github.com/aryas1ngh/brain-tumor-seg.git```

2. Download the MRI data into the specified directory ```'/bt_data/'```. You can modify the data path in the code if needed. Store the training and validation data in ```/train/``` and ```/val/``` respectively.

3. Execute the Jupyter notebook ```bt_seg_colab.ipynb``` in a compatible environment like Google Colab. Make sure to mount your Google Drive to access the data.

4. The notebook includes sections for data exploration, preprocessing, model architecture, training, and evaluation.

5. After training, the model will be saved as bt_seg.hdf5.

6. To test the trained model on a specific image, load the image and its corresponding mask using the provided function ```test_model```. Update the file paths accordingly.

7. View the training history and performance using the provided visualization functions.
