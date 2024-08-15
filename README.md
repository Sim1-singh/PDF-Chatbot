
# PDF Chatbot Maker

This repository contains the code and resources used for creating a chatbot that can answer questions based on the content of PDF documents. The chatbot utilizes advanced Natural Language Processing (NLP) techniques to understand and respond to user queries.

## Overview

The PDF Chatbot Maker project is designed to:

- Upload and parse PDF documents
- Extract and process text from PDFs
- Utilize NLP models to generate responses based on the extracted text
- Deploy the chatbot for interactive querying

## Technologies Used

- **Python**: Main programming language
- **Flask**: Web framework for the API
- **PyMuPDF (Fitz)**: Library to extract text from PDF files
- **Spacy**: NLP library for text processing
- **HuggingFace Transformers**: Pre-trained transformer models
- **Pandas**: Data manipulation and analysis
- **Numpy**: Numerical computations
- **Google Colab**: For running and testing notebooks

## Project Outline

1. **Upload and Parse PDF Documents**  
   **Objective:** Allow users to upload PDF files and extract text content.  
   **Tools:** PyMuPDF (Fitz)
   
2. **Text Extraction and Preprocessing**  
   **Objective:** Extract text from PDFs and preprocess for NLP tasks.  
   **Tools:** Spacy, Pandas, Numpy
   
3. **Question Answering Using NLP Models**  
   **Objective:** Use pre-trained transformer models to answer questions based on the extracted text.  
   **Tools:** HuggingFace Transformers
   
4. **Deploying the Chatbot**  
   **Objective:** Deploy the chatbot using Flask for interactive querying.  
   **Tools:** Flask

## Getting Started

### Installation

Clone this repository:

```bash
git clone https://github.com/your-username/pdf-chatbot-maker.git
cd pdf-chatbot-maker
```

Install required libraries:

```bash
pip install -r requirements.txt
```

### Running the Application

Run the Flask application:

```bash
python app.py
```

### Using the Chatbot

Once the application is running, you can interact with the chatbot via the web interface. Upload a PDF document and start asking questions based on its content.

### Endpoints

#### Upload PDF

- **Endpoint:** `/upload`
- **Method:** `POST`
- **Description:** Upload a PDF document to be processed by the chatbot.
- **Request Body:**
  - `file`: The PDF file to be uploaded.
- **Response:**
  - `200 OK`: PDF uploaded and processed successfully.
  - `400 Bad Request`: Invalid file format or upload error.

#### Ask Question

- **Endpoint:** `/ask`
- **Method:** `POST`
- **Description:** Ask a question based on the content of the uploaded PDF.
- **Request Body:**
  - `question`: The question to be asked.
- **Response:**
  - `200 OK`: Successful response with the answer.
  - `400 Bad Request`: Invalid question format or processing error.

## Examples

Check the `/notebooks` directory for example notebooks demonstrating text extraction, preprocessing, and question-answering tasks.

## Contributing

Contributions are welcome! If you have any suggestions or improvements, feel free to open an issue or submit a pull request.

---

Feel free to customize the URLs, project descriptions, and other specific details as per your project requirements.
