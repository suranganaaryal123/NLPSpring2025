# 1. System Requirements

Before running the app, ensure you have:
Python 3.9+
pip installed
Tesseract OCR installed (required for image-based PDF extraction)
Google Gemini API key

# 2. Install Tesseract OCR (Required)
Windows
Download installer:
https://github.com/UB-Mannheim/tesseract/wiki

After installation, add this to your PATH (if installer didn’t add it):
C:\Program Files\Tesseract-OCR

Mac
brew install tesseract

Linux (Debian/Ubuntu)
sudo apt install tesseract-ocr

# 3. Clone the Repository
Clone this repository.

# 4. Create & Activate Virtual Environment
Windows:
python -m venv venv
venv\Scripts\activate

macOS / Linux:
python3 -m venv venv
source venv/bin/activate

# 5. Install Python Dependencies
pip install -r requirements.txt

# 6. Set Up Your Google Gemini API Key

This app requires a Gemini API key.
Insert your api key in the .env file 
GOOGLE_API_KEY=your_api_key_here


You can generate an API key here:
https://ai.google.dev/gemini-api/docs/api-keys

# 7. Configure Poppler (Required for PDF Images)
Windows:
Download Poppler:
https://github.com/oschwartz10612/poppler-windows/releases/

Extract and add poppler/bin to PATH.

Mac:
brew install poppler

Linux:
sudo apt install poppler-utils

# 8. Run the Application

Inside the project directory:
streamlit run app.py
