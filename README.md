# 🧠 Text Extraction from Legal PDFs using BERT and Rule-Based Methods

This project focuses on extracting key information from legal or structured PDF documents using a combination of **BERT-based Question Answering**, **rule-based methods**, and **fallback extraction from PDF text**. It's designed to ensure that at least 400 relevant tokens are extracted per document, in an intelligent and robust way.

---

## 📌 Project Objectives

- Automate information extraction from documents (like legal allegations).
- Ensure high-quality extraction using:
  1. BERT QA-based extraction.
  2. Rule-based pattern extraction.
  3. Full-text fallback extraction from PDFs if needed.

---

## 🧰 Tools & Libraries Used

- **Python**
- **Google Colab** (with Google Drive integration)
- **Transformers (Hugging Face)** – for BERT models
- **PyMuPDF / fitz** – for PDF reading
- **re** – for pattern matching
- **NLTK** – for basic text processing

---

## 🚀 How It Works

1. **Mount Google Drive**  
   Connect your Drive so the notebook can access your files.

2. **Install Required Libraries**  
   Automatically installs all necessary Python packages.

3. **Text Extraction Pipeline**
   - **Step 1:** Try extracting content using a BERT Question Answering model.
   - **Step 2:** If Step 1 returns fewer than 400 tokens, apply rule-based extraction with regex patterns.
   - **Step 3:** If both steps return insufficient content, fallback to extracting relevant text directly from the PDF document.

4. **Final Output**  
   The result is a text file (or string) with the extracted content, optimized for relevance and length.

---

## 📝 How To Use

1. Open the notebook in **Google Colab**.
2. Mount your Google Drive when prompted.
3. Place your PDF documents in the appropriate Drive folder.
4. Run the notebook cells in order.
5. Retrieve the extracted output from the specified directory or variable.

---

## 📁 Folder Structure

```
project-root/
│
├── Your PDFs/
│   └── file1.pdf
│   └── file2.pdf
│
├── Extracted/
│   └── file1_output.txt
│
├── PJT2_Final.ipynb
```

---

## 🤖 Model Details

- The BERT model used is likely a pre-trained QA model like `bert-large-uncased-whole-word-masking-finetuned-squad`.
- It’s capable of answering questions and finding relevant spans in the input text.

---

## 💡 Notes for Beginners

- No deep knowledge of machine learning is needed to use this notebook.
- It's ideal for people looking to automate document analysis or content filtering.
- All installation and file-handling steps are covered within the notebook.

---

## 📬 Questions or Feedback?

Feel free to reach out via issues or pull requests if you’d like to contribute or need help!
