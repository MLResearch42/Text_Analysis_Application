# Natural Language Processing Tool

## Introduction/Overview

This application is a Natural Language Processing (NLP) tool built with Streamlit. It provides a user-friendly interface for various text analysis tasks. The target users for this application include anyone who needs to perform text analysis, from students and researchers to business professionals.

## Features

This tool offers a range of NLP features:

*   **Basic Text Analysis:** Provides simple descriptive statistics about your text, including document count, word count, unique word count, average word length, and generates a word cloud.
*   **Named Entity Recognition (NER):** Identifies and categorizes named entities in text, such as persons, organizations, and locations.
*   **Text Classification:** Classifies text into predefined categories. This feature utilizes the Hugging Face API for pre-trained models.
*   **Text Summarization:** Generates concise summaries of longer texts. This feature utilizes the Hugging Face API for pre-trained models.
*   **Topic Modeling:** Discovers abstract topics within a collection of documents.
*   **Document Clustering:** Groups similar documents together. Some clustering models may utilize the Hugging Face API.

## Input Methods

The application supports two main input methods:

*   **Text Area:** Users can directly paste or type text into a designated text area for analysis.
*   **CSV Upload:** Users can upload a CSV file containing text data. The application will provide an example format for the CSV file to ensure proper processing.

## Technologies Used

The following technologies and libraries are used in this project:

*   Streamlit
*   Pandas
*   Spacy
*   Textacy
*   KeyBERT
*   Scikit-learn
*   Plotly Express
*   WordCloud
*   UMAP
*   Cluestar
*   Hugging Face API

## Getting Started

To get started with this application, follow these steps:

1.  **Dependencies:** Install the required dependencies by running the following command in your terminal:
    ```bash
    pip install -r requirements.txt
    ```
2.  **Running the app:** Once the dependencies are installed, you can run the application using Streamlit:
    ```bash
    streamlit run Conduit_Application.py
    ```
3.  **Hugging Face API Key:** Certain features, such as Text Classification and Text Summarization, require a Hugging Face API key. You need to configure this key via Streamlit secrets. Create a file named `.streamlit/secrets.toml` in your project directory and add your API key as follows:
    ```toml
    api_key = "YOUR_HUGGING_FACE_API_KEY"
    ```
    The application will then access this key using `st.secrets["api_key"]`.

## License

This project is licensed under the terms of the LICENSE file.

## Contributing
Contributions are welcome! Please feel free to submit a pull request or open an issue.
