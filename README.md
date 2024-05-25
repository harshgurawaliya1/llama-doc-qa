
This repository hosts a Streamlit application designed for efficient question-answering over a collection of documents. The application uses the following components:

- **Llama 3 by Groq** for natural language processing.
- **Google Generative AI Embeddings** for embedding generation.
- **FAISS** for vector similarity search.
- **PyPDFDirectoryLoader** for loading PDF documents.

### Features
- **Document Embedding**: Load and preprocess PDF documents, splitting them into manageable chunks.
- **Question Answering**: Input queries to retrieve and process relevant document sections using Llama 3.
- **Similarity Search**: Display document chunks most relevant to the query for better insight.

### Installation
1. Clone the repository:
    ```sh
    git clone https://github.com/harshgurawaliya1/llama-doc-qa.git
    cd llama-doc-qa
    ```
2. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```
3. Set up your environment variables:
    ```sh
    cp .env.example .env
    ```
    Fill in your API keys in the `.env` file.

### Usage
1. Start the Streamlit app:
    ```sh
    streamlit run app.py
    ```
2. Open your web browser and navigate to `http://localhost:8501`.
3. Upload your PDF documents to the `./us_census` directory.
4. Click "Documents Embedding" to prepare the vector store.
5. Enter your question in the text input and retrieve answers along with relevant document chunks.

### License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

### Contributing
Contributions are welcome! Please fork the repository and create a pull request with your changes.
