# Task 1: Language Translation Tool

A Streamlit web app that translates text between 100+ languages.

## Features
- User interface with text box + source/target language selectors (Auto Detect supported)
- Uses the Google Translate API via `deep-translator` (no API key needed)
- Translated text displayed clearly on screen
- **Optional extras:** Copy-to-clipboard button and text-to-speech (gTTS)

## Setup
```bash
python -m venv venv
venv\Scripts\activate        # Windows  (Linux/Mac: source venv/bin/activate)
pip install -r requirements.txt
```

## Run
```bash
streamlit run app.py
```
Internet connection is required (Google Translate + gTTS are online services).

## Using the official Google Cloud Translation API instead
Replace the `translate()` function in `app.py` with a call to `google.cloud.translate_v2.Client().translate(...)`
after setting `GOOGLE_APPLICATION_CREDENTIALS`.
