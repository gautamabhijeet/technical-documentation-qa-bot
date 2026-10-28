# Closed-Domain Technical Documentation QA Bot

A question-answering system that helps students find information in technical manuals by uploading a PDF and asking questions in natural language.

## Features

- Upload technical PDF documents.
- Extract text using PyMuPDF.
- Retrieve relevant passages using TF-IDF and cosine similarity.
- Display brief answers, key points, and source-page references.
- Gradio-based user interface.
- Fine-tuned RoBERTa-base extractive question-answering model trained on a subset of SQuAD 2.0.

## Technologies Used

- Python
- Google Colab
- PyTorch
- Hugging Face Transformers and Datasets
- Scikit-learn
- PyMuPDF
- Gradio

## Current Implementation Status

The current chatbot uses TF-IDF retrieval and sentence selection. RoBERTa was fine-tuned separately and still needs to be integrated into the chatbot's final inference pipeline.

## Dataset

SQuAD 2.0: https://huggingface.co/datasets/rajpurkar/squad_v2

## How to Run

1. Open the notebook in Google Colab.
2. Install the required Python packages.
3. Load the dataset and train the QA model, or load saved model weights when available.
4. Run the notebook cells in order.
5. Upload a technical PDF and ask a question through the Gradio interface.

## Future Improvements

- Integrate the fine-tuned RoBERTa model into the chatbot.
- Evaluate answer quality using Exact Match and token-level F1.
- Improve handling of unanswerable questions.
- Add OCR support for scanned PDFs.

## Author

Abhijeet Kumar Gautam  
B.Tech Computer Science
