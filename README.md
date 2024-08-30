# CareerAI RAG System

**CareerAI-RAG-System** is an AI-powered prototype that provides personalized skill recommendations and career advice based on user queries about specific job roles. This system leverages a combination of retrieval and generative models to deliver accurate and insightful responses tailored to individual user needs.

## Features

- **Retrieval Augmented Generation (RAG):** Combines document retrieval with generative models to provide contextually relevant career guidance.
- **Document Embedding:** Utilizes Sentence Transformers to generate document embeddings for precise retrieval.
- **Vector Database Integration:** Supports retrieval using vector databases like Elasticsearch with ElastiKNN, Faiss, or Pinecone.
- **Generative Models:** Implements cutting-edge generative models such as Phi-3 - Mini 4k Instruct, Llama 3 - 8B Instruct, Gemma - 2B Instruct, or Mistral - 7B Instruct.
- **User Authentication:** Ensures secure access and personalized user experience.
- **Chat Memory Storage:** Remembers previous interactions to provide coherent and continuous conversations.
- **Simple UI:** User-friendly interface for seamless interaction with the system.

## How It Works

The application follows these steps to provide responses to your questions:

1. **PDF Loading:** The app reads multiple PDF documents and extracts their text content.

2. **Text Chunking:** The extracted text is divided into smaller chunks that can be processed effectively.

3. **Language Model:** The application utilizes a language model to generate vector representations (embeddings) of the text chunks.

4. **Similarity Matching:** When you ask a question, the app compares it with the text chunks and identifies the most semantically similar ones.

5. **Response Generation:** The selected chunks are passed to the language model, which generates a response based on the relevant content of the PDFs.

## Dependencies and Installation

1. Clone the repository to your local machine.
   ```bash
   git clone https://github.com/Islam-hady9/CareerAI-RAG-System.git
   cd CareerAI-RAG-System
   ```

3. Install the required dependencies by running the following command:
   ```
   pip install -r requirements.txt
   ```

4. Obtain an API key from OpenAI and add it to the `.env` file in the project directory.
   ```commandline
   OPENAI_API_KEY=your_secrit_api_key
   ```

## Usage

To use the MultiPDF Chat App, follow these steps:

1. Ensure that you have installed the required dependencies and added the OpenAI API key to the `.env` file.

2. Run the `main.py` file using the Streamlit CLI. Execute the following command:
   ```
   streamlit run app.py
   ```

3. The application will launch in your default web browser, displaying the user interface.

4. Load multiple PDF documents into the app by following the provided instructions.

5. Ask questions in natural language about the loaded PDFs using the chat interface.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
