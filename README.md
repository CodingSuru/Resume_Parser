# Resume Parser

## Overview
This project is a **Resume Parsing System** built in **Google Colab** to extract and process key information from resumes. It leverages **Machine Learning (ML) models**, **Natural Language Processing (NLP)**, and predefined libraries to identify structured data from resumes in **PDF and DOCX** formats. The extracted data is stored in an **Excel sheet** for further analysis.

## Features 🚀
- **File Handling:**
  - Supports **PDF** and **DOCX** resume files.
  - Reads files directly from the **`/content/`** directory.
  
- **Data Extraction & Preprocessing:**
  - Extracts raw text from uploaded resumes.
  - Cleans and formats extracted text for analysis.
  
- **Named Entity Recognition (NER) with Hugging Face Models:**
  - Identifies key details like **Name, Father’s Name, Date of Birth, Gender, Phone Number, Education, Experience, and Key Skills**.
  - Uses a hybrid model combining **pre-trained NER models** and **custom-trained models**.

- **Key Skills Matching:**
  - Uses a predefined dataset for extracting **soft skills, technical skills, and programming languages**.
  - Leaves the field blank if no match is found.

- **Education & Experience Extraction:**
  - Extracts **university name, degree, and time period**.
  - Uses an alternative approach when regex-based extraction fails.

- **User Corrections & Data Labeling:**
  - Allows users to correct misidentified labels.
  - Saves corrections and applies them in subsequent extractions.

- **Excel Storage & Structured Output:**
  - Stores parsed data in an **Excel file (`SampleResumeParsing.xlsx`)**.
  - Ensures structured and indexed data output.

## Workflow 📌
1. **Upload Resumes** → Place resume files in **`/content/`**.
2. **Run Google Colab Notebook** → Extract and process data.
3. **User Corrections** → Adjust incorrect labels if needed.
4. **Save & Export Data** → Outputs structured data to an Excel sheet.

## Dependencies 🔧
Ensure the following Python libraries are installed in Google Colab:
```python
!pip install pdfplumber python-docx pandas openpyxl transformers
```

## Future Enhancements ✨
- Integrate **FastAPI** for a web-based API service.
- Add **more datasets** for improved accuracy in skill and education extraction.
- Improve **multi-language support** for parsing non-English resumes.

## License 📜
This project is licensed under the **MIT License**.

