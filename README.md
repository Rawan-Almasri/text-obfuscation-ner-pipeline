#  Privacy-Preserving Text Obfuscation using Named Entity Recognition

##  Project Overview

This project focuses on building an intelligent text obfuscation system that detects and anonymizes sensitive information from text documents.

The system uses a **Named Entity Recognition (NER)** model (NuNerZero) to identify entities such as:
- Person
- Organization
- Location
- Country

These entities are then replaced with masked values (e.g., `****`) to ensure privacy preservation.

---

##  Objective

The main goal of this project is to:
- Automatically detect sensitive entities in text
- Replace them with anonymized placeholders
- Preserve the structure and meaning of the original text
- Generate a cleaned and privacy-safe output file

---

##  Methodology

The system is built as a structured pipeline consisting of multiple functions:

### 1. File Loading
The system reads input files (e.g., `.txt`, `.docx`) from a predefined storage location.

### 2. Text Extraction
The content of the file is extracted and converted into raw text for processing.

### 3. Entity Definition
Users define the types of entities to be detected, such as:
- Person
- Organization
- Location
- Country

---

### 4. Named Entity Recognition Model
A pretrained NuNerZero model is used to detect entities within the text.

---

### 5. Entity Extraction
The model is applied to extract relevant entities based on the defined labels.

---

### 6. Text Anonymization
Detected entities are replaced with masked tokens (e.g., `****`) to anonymize sensitive information.

---

### 7. Output Generation
The anonymized text is saved as a new file while preserving the original format of the input document.

---

##  Pipeline Workflow

The full system follows this sequence:

1. Load file  
2. Read content  
3. Define entity types  
4. Run NER model  
5. Extract entities  
6. Anonymize text  
7. Save output file  

---

##  Key Features

- Supports multiple file types  
- Uses transformer-based NER model  
- Customizable entity detection  
- Privacy-preserving text processing  
- Automated pipeline execution  

---

##  Use Case

This system can be used in:
- Data anonymization
- Privacy protection in documents
- Sensitive information removal
- Academic text processing
- Legal or medical text preprocessing

---

##  Outcome

The system successfully transforms raw text into a privacy-safe version by automatically detecting and masking sensitive entities while maintaining readability.

---

