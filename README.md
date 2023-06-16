# Image-Segmentation-Detectron2-Acne-Pimple
This repository contains a Python project for image segmentation using the Detectron2 framework. The project focuses on detecting and marking acne and pimple regions in facial images. The dataset consists of 250+ images collected from various online sources and Kaggle datasets. 

Dataset

The dataset used for training and testing the model consists of face images collected from various sources, including the internet and Kaggle datasets. A total of 250+ images containing acne and pimple regions were gathered for this project. To annotate the data, the VGG Annotator tool was employed, allowing the marking of acne and pimple regions in each image. The annotations were saved in JSON format.

Dataset Structure
The dataset folder should have the following structure:

dataset/
    ├── train/
    │   ├── image1.jpg
    │   ├── image2.jpg
    │   ├── ...
    │   └── train_annotations.json
    └── test/
        ├── image1.jpg
        ├── image2.jpg
        ├── ...
        └── test_annotations.json

The train folder contains training images, and the test folder contains testing images. The train_annotations.json file stores the JSON annotations for the training data, while the test_annotations.json file stores the JSON annotations for the testing data. Ensure that the JSON file names match in both folders.

Installation
Clone this repository:

git clone https://github.com/TarunChintu/Image-segmentation-Detectron2-Acne-Pimple.git
cd your-repo

Install the required dependencies:

Training
Open the train_model.py script and modify the configuration parameters as needed. You can adjust the batch size, learning rate, number of iterations, etc.
Run the training script:
The trained model and training logs will be saved in the output directory.

Inference
Open the test_model.py script and modify the path to the trained model in the cfg.MODEL.WEIGHTS variable.
Run the inference script:
The script will load the trained model and perform inference on the test images.
The resulting segmented images will be displayed.

Feel free to modify and adapt the code according to your specific requirements. Remember to update the paths, file names, and configurations as necessary. 


Note: The code provided in this README assumes that you have the necessary image data and annotations in the expected format. Ensure that the dataset folders, image files, and annotation files are properly organized and named before running the code.

