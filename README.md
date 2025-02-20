# 📄 PDF Summarization Using Gemini LLM

## 🚀 Overview

This project implements **automated text summarization** for PDF documents using **Google Vertex AI's Gemini-Pro Model**. It extracts text from PDF files, generates summaries for each page, and then creates a final concise summary using **LLM-powered summarization techniques**.

## 📌 Features

- ✅ **Extracts text** from PDF documents.
- ✅ **Summarizes each page** individually using Gemini LLM.
- ✅ **Combines summaries** into a final, concise summary.
- ✅ **Handles rate limits** with `ratelimit` and `backoff`.
- ✅ **Supports large documents** efficiently.

## 📂 Project Structure

```
text-summarization/
│── pdf_summarization/   # This folder contains the PDF Summarization project
│   ├── summarize_pdf.py  # Main script for summarizing PDFs
│   ├── mlops_summary.txt # Sample summary output
│   ├── requirements.txt  # Python dependencies
│   ├── README.md         # Project documentation (this file)
```

## 🛠️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/text-summarization.git
cd text-summarization/pdf_summarization
```

### 2️⃣ Create a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # On Mac/Linux
venv\Scripts\activate  # On Windows
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

## 🚀 How to Use

### **Summarizing a PDF**

```bash
python summarize_pdf.py --pdf_file path/to/your.pdf
```

### **Example Output**

```plaintext
📜 Extracted Summaries from PDF:
📄 Page 1 Summary: A guide to MLOps, a framework for continuous delivery and automation of ML.
📄 Page 2 Summary: This document presents a comprehensive overview of MLOps lifecycle and capabilities.
...
📌 Final Summary: A structured overview of MLOps best practices and deployment strategies.
```

## 🧠 How It Works

1. **Reads a PDF file** and extracts text from each page.
2. **Generates a summary per page** using Google’s **Gemini-Pro model**.
3. **Applies the MapReduce technique** to merge summaries into a final concise summary.
4. **Handles API rate limits** using `ratelimit` and `backoff`.

## ⚡ Technologies Used

- **Python 3.8+**
- **PyPDF2** for PDF text extraction
- **Vertex AI (Gemini LLM)** for text summarization
- **TQDM** for progress visualization
- **Google Cloud SDK** for authentication
- **Rate Limiting & Backoff** for API stability

## 🏗️ Future Improvements

- 🔹 Add **GUI/Web Interface** using Streamlit
- 🔹 Support **multi-language summarization**
- 🔹 Implement **topic-based summarization**

## 📜 License

This project is **MIT Licensed**. Feel free to use and modify it.

---

🚀 **Contributions are welcome!** If you improve this project, submit a Pull Request. 💡


