# Gemini Text Analysis App

This application allows users to upload a PDF document, extract text using OCR, and analyze the extracted text using Google's Gemini API for generative AI. It is designed for scenarios such as resume reviews and tailored content generation.

## Features

- PDF Upload: Users can upload PDF files for processing.
- Text Extraction: Extracts text from the uploaded PDF using `pdfplumber`.
- AI Analysis: Sends extracted text and user input to the Gemini API for advanced text analysis.
- Streamlit Interface: A user-friendly web application interface built with Streamlit.

## Requirements

### Libraries
- `streamlit`
- `Pillow`
- `google-generativeai`
- `pdfplumber`
- `python-dotenv`

### Environment Variables
Create a `.env` file in the project root and define the following:
```
GEMINI_API_KEY=your_gemini_api_key_here
```

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/ocr-gemini-app.git
   cd ocr-gemini-app
   ```

2. Set up a virtual environment and activate it:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Create a `.env` file and add your Gemini API key.

## Usage

1. Run the application:
   ```bash
   streamlit run app.py
   ```

2. Open the URL provided in the terminal (e.g., `http://localhost:8501`).

3. Upload a PDF document and provide a custom prompt in the text input field.

4. Click "Submit" to process the text and display the AI analysis.

## File Structure
```
ocr-gemini-app/
├── app.py          # Main application script
├── requirements.txt # List of dependencies
├── .env            # Environment variables (ignored by git)
├── README.md       # Project documentation
```

## Notes

- Ensure your API key has the necessary permissions for the Gemini API.
