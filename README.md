# News_Research_Bot

This project demonstrates the creation of an end-to-end research tool that allows users to input news article URLs and ask questions to retrieve answers from the provided articles using Language Learning and Streamlit.

## Features

- **Document Loaders**: Load text data from different sources (e.g., URLs, CSV files)
- **Text Splitting**: Divide large text into smaller chunks using CharacterTextSplitter or RecursiveCharacterTextSplitter
- **Vector Databases**: Store embeddings of text chunks in a vector database (e.g., faiss)
- **Retrieval QA with Source Chain**: Retrieve relevant text chunks from the Vector Database based on a user's question and form a prompt for LLM, which then generates the final answer.

## Setup and Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/news-research-bot.git
   cd news-research-bot
   ```

2. **Install Required Packages**:
   Make sure you have Python installed (version 3.7+ recommended). Install the required packages using `requirements.txt`.
   ```bash
   pip install -r requirements.txt
   ```

3. **API Configuration**:
-  **OpenAI API**: Ensure you have API access for retrieving text chunkss.
-  Create an `.env` file in the root directory and add your API keys:
   ```bash
   OPENAI_API_KEY='enter your openapi key here'
   ```

4. **Run the Application**:
   Launch the Streamlit app by running the following command:
   ```bash
   streamlit run main.py
   ```
