# PDF → Markdown Pipeline

Browser-based tool for converting PDF documents to Markdown format with OCR support.

**Live:** https://ocr-ssilv.de/

## Features

- **PDF Upload** - Drag & drop or select PDF files directly in the browser
- **OCR Support** - Extract text from scanned/image-only PDFs using Tesseract.js
- **Markdown Export** - Convert PDFs to clean, structured Markdown
- **Image Support** - Extract and embed images from PDF documents
- **Math Rendering** - MathJax support for mathematical expressions (LaTeX)
- **Word Export** - Export documents as Word (.docx) format
- **PWA Ready** - Works offline with service worker caching

## Tech Stack

- **Frontend:** Vanilla JavaScript (ES6+), HTML5, CSS3
- **PDF Processing:** pdf.js (Mozilla)
- **OCR:** Tesseract.js
- **Math:** MathJax 3
- **Word Export:** html-docx.js, JSZip
- **Canvas:** Fabric.js

## Getting Started

### Online

Simply visit https://ocr-ssilv.de/ and upload a PDF file.

### Local Development

```bash
# Clone the repository
git clone https://github.com/erichrueger-ssilv/marker-ocr.git
cd marker-ocr

# Serve with any static file server
python3 -m http.server 8000
# or
npx serve .
```

Then open http://localhost:8000 in your browser.

## Project Structure

```
├── index.html          # Main application
├── app.js              # Core application logic
├── styles.css          # Main styles
├── update-version.py   # Version/badge updater
├── lib/                # Third-party libraries
│   ├── pdf.min.js          # PDF.js
│   ├── pdf.worker.min.js   # PDF.js worker
│   ├── tesseract.min.js    # Tesseract.js OCR
│   ├── mathjax/            # MathJax
│   └── ...
└── manifest.json       # PWA manifest
```

## Usage

1. Open the application in your browser
2. Upload a PDF file via drag & drop or file picker
3. Wait for the document to be processed
4. Edit or copy the resulting Markdown
5. Optionally export as Word document

## Version History

- **v2.41** - Latest update from Kasserver
- **v2.40** - Initial release

## License

MIT License
