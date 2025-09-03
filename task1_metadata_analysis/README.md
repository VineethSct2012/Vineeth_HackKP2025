# Task 1 – Metadata Analysis

##  Description
The Metadata Analysis module extracts both technical metadata and textual content from an image.
It combines EXIF data extraction, OCR (Optical Character Recognition), and language detection into a unified pipeline.
This task is useful for forensic analysis of images, as it reveals hidden metadata (e.g., camera model, timestamps, geo-coordinates) and extracts embedded text (e.g., receipts, documents, or signs in photos).

##  How to Run
Run the script from the task folder:

cd task1_metadata_analysis/code

python metadata_analysis.py ../sample_input/sample1.jpg

Task 1: Metadata Analysis
 

Features

    Extract EXIF metadata (camera model, timestamp, orientation, ISO, focal length, etc.)
    Detect geo-location (GPS coordinates) if available in EXIF
    Run OCR using Tesseract to extract text from the image
    Detect language of extracted text automatically
    Save analysis report as a Word document (.docx) for investigators

Tech Stack Used

    Python 3.12

Libraries:

    exifread → Read image EXIF metadata

    pytesseract → OCR using Google Tesseract (AI-powered LSTM model)

    Pillow → Image loading & preprocessing

    langdetect → Detect language of OCR text

    python-docx → Generate investigation reports in Word format

Installation

Make sure you have the dependencies installed:

pip install -r requirements.txt


Additionally, install Tesseract OCR (required for text extraction):



After installation, ensure tesseract is in your system PATH:

tesseract --version

Usage

Run the script from the task folder:

cd task1_metadata_analysis/code
python metadata_analysis.py ../sample_input/sample1.jpg

Output

Prints EXIF metadata, OCR text, and detected language in the terminal.

Saves a structured Word report in ../sample_output/ with:

Image filename

Extracted EXIF metadata

OCR extracted text

Detected language

Example Report Snippet
File: sample1.jpg

EXIF Metadata:
- Camera: OnePlus Nord CE4
- Date Taken: 2025-07-28 21:55:16
- ISO: 1000
- Exposure: 1/50

OCR Extracted Text:
"Invoice No: 748
  Water & Beverage - 430.00
  Chicken Kebab - 795.00"

Detected Language:
English (en)