# AskGPT Document Generator

AskGPT Document Generator is a Flask-based web application that utilizes OpenAI's GPT-3 API to generate question-and-answer pairs. The application allows users to submit a question, get a response from GPT-3, and generate a downloadable Word document (in `.docx` format) containing the questions and corresponding answers. The app also supports downloading chat logs as a Word document.

## Features

- Users can ask questions through a simple web interface.
- Questions are processed using OpenAI's GPT-3 to generate thoughtful answers.
- Generated Q&A pairs are stored in a Word document.
- Users can download the generated chat logs or Q&A pairs in `.docx` format.
  
## Prerequisites

Make sure you have the following installed:

- Python 3.x
- Flask
- Python-docx library for handling `.docx` file creation
- OpenAI API key for GPT-3 access

## Installation

1. Clone the repository:

   git clone https://github.com/ikhan9985/askgpt-document-generator.git
   cd askgpt-doc-generator

Create a virtual environment (optional but recommended):

python3 -m venv venv
source venv/bin/activate  # On Windows, use venv\Scripts\activate

Install dependencies.

Set up your OpenAI API key:

Open the app.py file and replace the placeholder YOUR API KEY with your actual OpenAI API key.

openai.api_key = "YOUR API KEY"

Usage
Start the Flask server:

python app.py
Open your browser and navigate to:

http://127.0.0.1:5000/

Enter your question in the web form and submit. You will get an AI-generated answer from GPT-3.

You can download the generated Q&A pairs as a .docx document by clicking the "Download Answers" button.

Endpoints
/ - Main page with the question form.
/get_answer - Endpoint for processing the question and fetching the GPT-3 response.
/download_answers - Endpoint for downloading the generated Word document with chat logs.

Template (HTML)
The index.html file is located in the templates directory. You can modify the front-end as per your design needs.

The project uses the following Python libraries:

Flask: A lightweight WSGI web application framework.
python-docx: A Python library for creating and updating .docx files.
openai: OpenAI API for GPT-3 access.
To install dependencies, run:

pip install Flask python-docx openai
Alternatively, you can install all the dependencies using the requirements.txt file:

Author
Muhammad Imran
