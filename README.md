# Intelligent-Document-Automation-Building-a-Smart-OCR-Bot

## Project Description
This project explores Intelligent Document Processing (IDP) techniques using two datasets: the SROIEv2 dataset for receipt information extraction and a resume dataset for converting PDF resumes to text. The project demonstrates steps for document pre-processing (grayscale conversion, noise reduction, binarization, and skew correction) using OpenCV, text extraction using Tesseract OCR, and information extraction from receipts using a generative AI model. It also includes steps for converting PDF documents to text using `pdfminer.six`. The goal is to showcase a basic IDP pipeline for handling semi-structured documents like receipts and unstructured documents like resumes.

## Tech Stack
* **Python:** The primary programming language used for the analysis and model building.
* **kagglehub:** Used for downloading datasets from Kaggle.
* **os:** Used for interacting with the operating system, including file and directory operations.
* **cv2 (OpenCV):** Used for image pre-processing techniques like grayscale conversion, noise reduction, binarization, and skew correction.
* **matplotlib:** Used for displaying images.
* **numpy:** Used for numerical operations, particularly with image data.
* **pytesseract:** A Python wrapper for Google's Tesseract OCR engine, used for text extraction from images.
* **PIL (Pillow):** Used for opening and handling image files, required by pytesseract.
* **google-generativeai:** The Google AI SDK for interacting with generative models for information extraction.
* **google.colab.userdata:** Used for securely accessing API keys in Google Colab.
* **json:** Used for working with JSON data, particularly for loading ground truth and saving extracted information.
* **time:** Used for timing operations.
* **pdfminer.six:** Used for converting PDF files to text.
* **io (StringIO):** Used as a text buffer for PDF to text conversion.

## How to Run
1. **Open the notebook in Google Colab:** Upload or open the notebook file (.ipynb) in your Google Colab environment.
2. **Install dependencies:** Ensure you have the necessary libraries installed. If running in a new Colab environment, you can install them using pip (refer to the requirements.txt file generated earlier).
3. **Provide API Key:** Add your Google AI API key to the Colab secrets manager named `GOOGLE_API_KEY`.
4. **Ensure PDF files are in the correct path:** If you are working with the resume PDF conversion part, ensure your `BPO_data_pdf` folder is located at `/content/BPO_data_pdf` as specified in the notebook.
5. **Run all cells:** Execute all the code cells in the notebook sequentially from top to bottom. This will perform the dataset download (for SROIEv2), image pre-processing, text extraction (Tesseract), information extraction (Gemini), and PDF to text conversion.

## Screencasts

**1. PDF to Text Conversion**

<img width="455" height="492" alt="image" src="https://github.com/user-attachments/assets/73754cd1-1176-4a74-99ee-f67733c217a9" />

**2. PDF to Text Conversion Image**

<img width="787" height="516" alt="image" src="https://github.com/user-attachments/assets/cce94bf5-67d7-478c-81b6-c070177fda2a" />


