# SIH-23-ZT6 :: PolyIndicTrans: A Python Based Multilingual Multi-format Document Translator
PolyIndicTrans is a Flask application designed to translate multi-format documents. It takes input as the file location, the language of the content, and the language to which the file needs to be translated. The application supports various file formats including presentations (pptx), PDFs, .txt files, .docx files, and images.

The application processes the file based on its extension. For text-based files, it reads the content, translates it, and produces the output. For images, it uses Tesseract OCR to read the content, translates it, and outputs the result.

The application currently uses deep_translator’s Google_translator library for translation, which requires an internet connection. However, we plan to switch to AI4Bharat’s Translation models, which are pretrained machine learning models capable of translating up to 11 Indian languages.

In the future, we aim to use OCR to identify text paragraphs in documents, translate them, and replace the original text with the translated version in the document itself. This will allow us to maintain the original formatting of the document, including images, footers, etc. We also plan to build our own OCR models to handle Indian languages, reducing dependency on Tesseract’s OCR and ensuring better security and control over the model configuration.

This project is developed to compete in SMART INDIA HACKATHON 2023.

## Installation Guide:
We recommend creating a new environment in Anaconda Prompt and installing all the required libraries. Use the following commands:

```
conda create --name sih23zt6 python=3.11.5 pip
conda activate sih23zt6
cd /path/to/the/clone/of/the/repository
pip install -r requirements.txt
```
Replace "sih23zt6" with your desired environment name, and navigate to the GitHub repository to install the required libraries.

Run the application by executing the Python File at flask_application -> Test_Flask -> Test_Flask.py

### NOTE:
If you encounter any errors while building wheel for any library, you might need to install Microsoft Visual C++ 14.0 or greater. Please visit the following link to install it: Microsoft Visual C++ Build Tools

## Sources:
[https://pypi.org/project/pytesseract/](https://pypi.org/project/pytesseract/)

[2022.ai4bharat.org/translation](https://2022.ai4bharat.org/models)
