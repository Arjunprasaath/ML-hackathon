# PDF Analysis with LLM

## Overview

This project leverages the power of OpenAI's GPT models to analyze the contents of PDF files, providing detailed insights and enabling user interaction through a conversational interface. It includes a Gradio-based web application that lets users upload PDF files, process their contents, and query the extracted data interactively.

## Features

- **PDF to Image Conversion:**  
  Converts PDF pages into images for analysis.

- **Detailed Content Analysis:**  
  Processes PDF images using an OpenAI GPT model to generate detailed, accurate textual descriptions.

- **Interactive Chat with LLM:**  
  Allows users to ask specific questions about the analyzed PDF content.

- **Efficient Processing:**  
  Caches analysis results to avoid redundant processing of previously uploaded PDFs.

- **Web-Based Interface:**  
  User-friendly Gradio interface for seamless interaction.

## Prerequisites

- Python 3.7 or later
- OpenAI API key (required for GPT model integration)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/pdf-analysis-llm.git
   cd pdf-analysis-llm
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set your OpenAI API key:
   Open the script and replace `your_openai_api_key` with your OpenAI API key.

4. Run the application:
   ```bash
   python app.py
   ```

## Usage

- **Upload PDF:**  
  Drag and drop or select a PDF file through the provided upload button.

- **Automatic Analysis:**  
  The application processes the uploaded PDF and generates detailed textual descriptions for its contents.

- **Query the Analysis:**  
  Enter specific questions about the PDF content in the chat interface, and receive answers powered by the OpenAI model.

## File Caching

Processed PDF analyses are saved as text files in a directory named `KD`. This allows faster interaction with previously analyzed PDFs.

## Example Workflow

1. Upload a soccer game analysis PDF.
2. The application extracts images from the PDF and analyzes the content using OpenAI's model.
3. Enter a query like, "What are the key highlights of the game?" to get a summarized answer based on the extracted data.


## Dependencies

- **gradio:** For building the web interface.
- **openai:** For GPT model interaction.
- **pymupdf:** For PDF to image conversion.
- **Pillow:** For image processing.
- **tqdm:** For progress visualization.

## Known Limitations

- **Image-Based PDFs:** PDFs with embedded images but no text may lead to incomplete or imprecise analysis.
- **Processing Time:** Large PDFs with many pages can take longer to process.

## Future Enhancements

- Make the KD more stronger by using bigger models.
- Can implement Graph RAG for answering question.
- Can make the 