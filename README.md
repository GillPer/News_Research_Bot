# News_Research_Bot

This project is an end-to-end research tool that enables users to input URLs of news articles and ask targeted questions, retrieving precise answers from the provided articles. Built using Language Learning Models (LLM) and Streamlit, this tool is ideal for researchers and analysts who need quick insights from a large volume of news articles. 

## Features

- **Automated Content Loading**: Pulls text from various sources, such as URLs and CSV files.
- **Efficient Text Splitting**: Divides large text bodies into manageable chunks, improving processing and retrieval efficiency.
- **Vector Database**: Embeds and stores text chunks in a vector database (FAISS) for quick retrieval.
- **Question-Answering**: Leverages Retrieval QA with Source Chain to find relevant text chunks, generate responses, and cite sources.

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

3. **Set Up OpenAI API Key**:
-  **OpenAI API**: Ensure you have API access for retrieving text chunkss.
-  To use the OpenAI LLMs, store your API key in a `.env` file.
   ```bash
   OPENAI_API_KEY='enter your openapi key here'
   ```

4. **Run the Application**:
   Launch the Streamlit app by running the following command:
   ```bash
   streamlit run main.py
   ```
## Project Workflow

1. **Input News URLs**: Enter up to three news article URLs in the sidebar.
2. **Data Loading and Processing**: Click "Process URLs" to load and split data into text chunks.
3. **Embedding Storage**: FAISS stores embeddings of the text chunks for easy retrieval.
4. **Query and Answer**: Enter your question in the input box to retrieve relevant answers along with sources.
