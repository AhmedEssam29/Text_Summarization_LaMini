# Document Summarization App using Language Model


## Overview
This Document Summarization App is built using Streamlit, Langchain, and Hugging Face's T5 Transformer model for summarization. The app allows users to upload PDF documents, which are then preprocessed and summarized by a language model. This tool is particularly useful for extracting key information from lengthy documents quickly and efficiently.

## Features
- **PDF Upload and Display**: Upload any PDF document to view it directly within the app.
- **Document Summarization**: Summarize content from the PDF file using a fine-tuned T5 model.
- **Interactive UI**: User-friendly interface built with Streamlit.

## Requirements
- Python 3.7+
- [Streamlit](https://streamlit.io/)
- [Hugging Face Transformers](https://huggingface.co/transformers/)
- [Langchain](https://langchain.com/)

## Setup Instructions
### 1. **Clone the repository** and navigate to the project folder.
### 2. **Install the dependencies**:
   ```bash
   pip install streamlit langchain transformers torch
   ```

### 3. Download and prepare the model:

- The project uses the LaMini-Flan-T5-248M model. It will be downloaded automatically when running the app.

### Run the App
   ```bash
streamlit run app.py
   ```

## Code Explanation
The app is structured in three main parts:

1. **Model and Tokenizer Initialization:** The T5 model and tokenizer are initialized and loaded.

2. **File Preprocessing:** The PDF is loaded, text is extracted, and then split into manageable chunks for summarization.
3. **Summarization Pipeline:** Summarizes the text chunks and outputs a summary to the UI.

## File Structure

**app.py:** The main application file containing all the code.

**README.md:** This README file with instructions.

**data/:** Folder where uploaded files are temporarily stored.
## Usage
**Upload a PDF:** Drag and drop your PDF file into the uploader.

**View PDF:** The uploaded file will display on the left side of the screen.

**Summarize:** Click the "Summarize" button to generate a summary on the right side of the screen.

## Screenshot

To view the app interface, see the image below:
![alt text](https://github.com/AhmedEssam29/Text_Summarization_LaMini/blob/main/Program.png?raw=true)



## Notes
- Make sure your environment supports GPU for faster processing if you’re working with larger documents.
- The model can handle documents of reasonable length, but for very large documents, you may need to adjust chunk sizes for optimal performance.

## vbnet

   ```bash

In this example:
- Make sure to replace `app.py` with the actual name of your app script if it differs.
- The image link is set to an absolute path; for sharing, you’d usually place the image within the repository and use a relative path like `![Program Interface](./Program.png)`
```





