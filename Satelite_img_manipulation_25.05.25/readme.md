Satelite Image Processing Using Deep Learning

This project provides a Python script for processing images in a Google Colab environment, specifically for resizing and cropping images from a dataset. It is designed for neural research applications, such as preparing medical imaging data (e.g., COVID-19 scans) for machine learning tasks.

Table of Contents

Project Description
Key Features
Installation Guide
Technologies Used

Project Description
Satelite Image Processing Using Deep Learning project automates the resizing and cropping of images stored in Google Drive using Google Colab. It processes images from a specified dataset directory, resizes them to a uniform size (e.g., 224x224 pixels), and applies cropping for specific regions of interest. 

Key Features

1. Image Resizing: Resizes images to a uniform size (e.g., 224x224 or 300x350 pixels) for consistency in neural network input.
2. Image Cropping: Crops specific regions of images (e.g., [60:400, 30:250]) for focused analysis.
3. Batch Processing: Processes multiple images in a dataset directory automatically.
4. Google Drive Integration: Mounts Google Drive to access and save images seamlessly in Colab.
5. Error Handling: Skips invalid images and logs processing status for each file.

Installation Guide
To run this project locally or in Google Colab, follow these steps:

1. Set Up Google Colab:
2. Open Google Colab.
3. Upload the provided .ipynb file or create a new notebook.
4. Mount Google Drive:
Run the following code to mount your Google Drive:from google.colab import drive
drive.mount('/content/drive')
5. Follow the authentication prompt to grant access.

Prepare Dataset:

Place your images in a Google Drive directory (e.g., /content/drive/MyDrive/Dataset_images).
Ensure images are in .png, .jpg, or .jpeg format.

Run the Script:

Copy and paste the provided code into the Colab notebook.
Update the input_dir and output_dir paths to match your Google Drive structure.
Execute the cells to resize and crop images.

Check Output:

Resized images are saved in the specified output_dir (e.g., /content/drive/MyDrive/Resized_Dataset_images).
Cropped images are saved in the specified cropping output_dir (e.g., /content/drive/MyDrive/Cropped_Dataset_images).


Technologies Used

1. Python: Core programming language (version 3.x).
2. OpenCV (cv2): For image reading, resizing, and cropping.
3. NumPy: For handling image arrays and dimensions.
4. Google Colab: Cloud-based environment for running the script.
5. Google Drive: For storing and accessing image datasets.
