# Handwritten Text Extraction Using OCR

This project implements an Optical Character Recognition (OCR) pipeline to extract handwritten text from images and PDF documents. The pipeline uses Tesseract OCR with the `pytesseract` library, along with image preprocessing techniques to improve text accuracy. The project is developed in Python and runs in Google Colab.

## Features

- **Image Preprocessing:** Converts images to grayscale and applies binary thresholding to enhance text visibility.
- **OCR Processing:** Utilizes Tesseract OCR to extract handwritten text from images and PDF pages.
- **PDF Support:** Converts PDF pages to images before performing OCR.
- **Data Visualization:** Includes visualization of processed images and extracted text using Matplotlib.
- **Colab Integration:** Provides a Colab notebook for easy setup and execution.

## Technologies

- **Programming Language:** Python
- **Libraries:** Tesseract OCR, `pytesseract`, OpenCV, PIL, Matplotlib, `pdf2image`
- **Platform:** Google Colab

## Installation and Usage

1. **Install Required Packages:**

   ```bash
   !apt-get install -y poppler-utils
   !apt-get install -y tesseract-ocr
   !pip install pytesseract
   !pip install opencv-python-headless
   !pip install pdf2image
   ```

Set Up Tesseract Path:

2. **Ensure the path for Tesseract OCR is set in your script. For Google Colab, it is typically:**


```bash
pytesseract.pytesseract.tesseract_cmd = '/usr/bin/tesseract'
Upload Files:
```
Use the file upload dialog in Google Colab to upload images and PDF documents.

Run Preprocessing and OCR:

The script will automatically process uploaded files:

For PDFs, each page is converted to an image, preprocessed, and then OCR is applied.
For images, preprocessing is applied directly, followed by OCR.
View Results:

Processed images and extracted text will be displayed in the Colab notebook. Visualization of binary images and the extracted text will be shown.

Example
Here's a snippet of how to use the provided Colab notebook:

python
```
# Install dependencies
!apt-get install -y poppler-utils
!apt-get install -y tesseract-ocr
!pip install pytesseract
!pip install opencv-python-headless
!pip install pdf2image

# Upload files
uploaded = files.upload()

# Process files
# Code for processing and OCR extraction here
```
Colab Notebook
Access the interactive Colab notebook [here](https://colab.research.google.com/drive/10YUJvhUh6Fp5Ndx9BYsaHJL3aViIeM2V#scrollTo=loaeYYVrg4VJ).


Contributing
Contributions are welcome! Please open an issue or submit a pull request to contribute.

License
This project is licensed under the Apache License 2.0. See the LICENSE file for details.

