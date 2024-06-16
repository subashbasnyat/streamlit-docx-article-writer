## Overview
The Article Writer is a Streamlit application that allows users to generate articles on any topic. Users can specify a keyword, choose a writing style, and set the desired word count for the article. The generated article can then be downloaded as a .docx file.

## Features
- Keyword Input: Users can input a keyword for the article's topic.
- Writing Style Selection: Users can choose from various writing styles such as "Academic", "Business", "Sarcastic", "Casual", "Funny".
- Word Count Slider: Users can select the word count for the article, ranging from 300 to 1000 words.
- Article Generation: The app generates the article based on the provided inputs.
- Downloadable Output: The generated article can be downloaded as a .docx file.

## Technologies Used
- Streamlit: Used for building the web interface.
- LangChain: Utilized for generating the article content using language models.
- python-docx: Used for creating and saving .docx files.
- Pydantic: For data validation and settings management.
- Loguru: For logging information and debugging purposes.

## Prerequisites
Ensure you have the following installed:

- Python 3.7 or higher
- Required Python packages listed in requirements.txt

## Installation
- Clone the repository:
    ```
    git clone https://github.com/subashbasnyat/streamit-docx-article-writer.git
    cd streamit-docx-article-writer
    ```
- Install the required packages:
    ```
    pip install -r requirements.txt
    ```

- You can setup local OLLAMA instance from [here](https://github.com/ollama/ollama).
- You can use NVIDIA API key to use `mistralai/mixtral-8x7b-instruct-v0.1` model by referencing [this documentation](https://python.langchain.com/v0.2/docs/integrations/chat/nvidia_ai_endpoints/) 
    - Set up NVIDIA API Key: Replace the XXXXXXXX in the `os.environ["NVIDIA_API_KEY"]` line with your actual NVIDIA API key.

## Usage
- Run the Streamlit app:
    ```
    streamlit run app.py
    ```

## Interact with the app:

- Enter a keyword for the article topic.
- Select a writing style from the dropdown.
- Adjust the word count using the slider.
- Click the "Generate Article" button to generate the article.
- Once the article is generated, you can download it as a .docx file by clicking the "Click here to download (docx)" button.

