# Vineeth_HackKP2025
Hackthon Project of Vineeth M , for HackKP25 , vineethsct2012@gmail.com , AI team , Cyber Security Engineer/ Analyst @ Union Bank of India
# HacKP 2025 

##  Author
- Name: Vineeth M
- Email: vineethsct2012@gmail.com
- Team/Institution : AI Team / Union Bank of India

##  Hackathon Tasks & Integration
All eight hackathon tasks have both **individual modules** and are **integrated into a unified Investigator Web Tool**.

###  Task Modules
- [Task 1: Image Metadata Analysis](./task1_metadata_analysis)
- [Task 2: Indoor/Outdoor Classifier](./task2_indoor_outdoor_classifier)
- [Task 3: Search Images with Text](./task3_search_images_text)
- [Task 4: Search Images with Image](./task4_search_images_image)
- [Task 5: Object Segmentation & Cropping](./task5_object_segmentation)
- [Task 6: Image Similarity Scoring](./task6_similarity_scoring)
- [Task 7: Search Objects with Image Query](./task7_search_objects_image_query)
- [Task 8: Investigator Web Tool (Integrated)](./task8_investigator_web_tool)

###  Integrated Product
The Investigator Web Tool features:
- Bilingual support (English & Malayalam)
- AI modules with pfi3 LLM, RAG, MCP
- Functional requirements: Trace an Object, Take It Down, Grapnel 2.0

##  Setup Instructions
```bash
# create environment
python3 -m venv venv && source venv/bin/activate

# install dependencies
pip install -r requirements.txt

# 1. Clone repo
git clone https://github.com/VineethSct2012/Vineeth_HackKP2025.git
cd Vineeth_HackKP2025

# 2. Create Python environment
python3 -m venv venv
source venv/bin/activate    # On Windows use: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run Task 1 (example)
python task1_metadata_analysis/code/run.py --input task1_metadata_analysis/sample_input/test.jpg --output task1_metadata_analysis/sample_output/report.json

⚠️ Note: For OCR features (English + Malayalam), please install Tesseract OCR engine:
- Linux: sudo apt-get install tesseract-ocr tesseract-ocr-mal
- Windows: Download from https://github.com/UB-Mannheim/tesseract/wiki
