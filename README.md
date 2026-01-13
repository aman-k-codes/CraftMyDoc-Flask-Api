# 📄 Document & Image Processing API (Flask)

A multi-utility REST API built using **Flask** that provides image and document
processing features such as background removal, image enhancement, OCR,
PDF conversion, and Word generation.

This project demonstrates backend API development combined with
computer vision and ML-based tools.

---

## 🚀 Features

- 🖼️ Image background removal (using `rembg`)
- 🔍 Image enhancement with **Real-ESRGAN**
- 🧾 Image to Text (OCR using Tesseract)
- 📄 PDF to HTML conversion
- 📄 PDF to Word (DOCX)
- 🖼️ Image to Word conversion
- RESTful API endpoints with file uploads

---

## 🛠 Tech Stack

- **Backend:** Flask (Python)
- **Image Processing:** Pillow, rembg
- **ML / CV:** Real-ESRGAN, PyTorch
- **OCR:** Tesseract OCR
- **Document Processing:** pdf2docx, PyMuPDF
- **Utilities:** UUID, IO streams

---

## 📂 Project Structure
├── app.py
├── pdf_files/
├── html_con/
├── doc_files/
├── word_files/
├── requirements.txt
└── README.md

## 🔌 API Endpoints

| Method | Endpoint | Description |
|------|--------|------------|
| GET | `/api` | Health check |
| POST | `/api/remove-bg` | Remove image background |
| POST | `/api/enhance-photo` | Enhance image using Real-ESRGAN |
| POST | `/api/image-to-text` | Extract text from image |
| POST | `/api/pdf-to-html` | Convert PDF to HTML |
| POST | `/api/pdf-to-word` | Convert PDF to Word |
| POST | `/api/image-to-word` | Convert image to Word |

## ▶️ How to Run Locally

### 1️⃣ Clone the repository
```bash
git clone https://github.com/aman-k-codes/<repo-name>.git
cd <repo-name>

python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate

pip install -r requirements.txt

python app.py

http://127.0.0.1:5000
