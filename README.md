## Brain Tumor Segmentation using 3D U-Net

This repository contains code for brain tumor segmentation using a 3D U-Net architecture. The model is trained on magnetic resonance imaging (MRI) data with different modalities, including T1, T1-CE, T2, and FLAIR. The segmentation task involves identifying the tumor region in the brain scans. The dataset used is BraTS Challenge 2020, organized by Perelmann Med School, UPenn.

- Kaggle dataset link (train + val) : [link](https://www.kaggle.com/datasets/awsaf49/brats20-dataset-training-validation)
- BraTS Challenge : [link](https://www.med.upenn.edu/cbica/brats/)


1. Clone the repo:
```git clone https://github.com/aryas1ngh/brain-tumor-seg.git```

2.  Install the requirements:
```pip install -r requirements.txt```

3. Download the MRI data into the specified directory ```'/bt_data/'```. You can modify the data path in the code if needed. Store the training and validation data in ```/train/``` and ```/val/``` respectively.

4. Execute the Jupyter notebook ```bt_seg_colab.ipynb``` in a compatible environment like Google Colab. Make sure to mount your Google Drive to access the data.

5. The notebook includes sections for data exploration, preprocessing, model architecture, training, and evaluation.

6. After training, the model will be saved as ```bt_seg.hdf5```.

7. To test the trained model on a specific image, load the image and its corresponding mask using the provided function ```test_model```. Update the file paths accordingly.

8. View the training history and performance using the provided visualization functions.



### Files
- ```bt_seg_colab.ipynb```: Jupyter notebook containing the code for data processing, model training, and evaluation.
- ```README.md```: Brief overview and usage instructions.
- ```sample-brain-images.png```: Sample scans of T1, T1-CE, T2 and FLAIR modality with tumor mask.
- ```unet_arch.png```: Model architecture diagram.


### Acknowledgments
- The U-Net architecture used in this project is adapted from the original paper: [U-Net: Convolutional Networks for Biomedical Image Segmentation.](https://arxiv.org/abs/1505.04597)
- Data used in this project can be obtained from the [BraTS challenge](https://www.med.upenn.edu/cbica/brats/).
