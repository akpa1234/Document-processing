# Document-processing
# RAG System with Pinecone

## Overview

This project implements a Retrieval-Augmented Generation (RAG) system using Pinecone for vector indexing and OpenAI's GPT-3.5 for generating answers. The system allows users to query a Pinecone index with their questions and retrieve relevant context to generate answers using GPT-3.5.

## Features

- **Pinecone Indexing**: Manages vector-based indexing for efficient retrieval of relevant context.
- **Sentence Transformers**: Generates embeddings for queries and context using pre-trained models.
- **OpenAI GPT-3.5**: Provides advanced natural language understanding and generation to answer questions based on the retrieved context.
- **Streamlit Interface**: Provides a user-friendly web interface for interacting with the system.

## Prerequisites

Before running the app, ensure you have the following:

- Python 3.6 or higher
- API keys for Pinecone and OpenAI

## Installation

1. **Clone the repository:**

    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2. **Create and activate a virtual environment:**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install the required packages:**

    ```bash
    pip install -r requirements.txt
    ```

4. **Set up environment variables:**

    Create a `.env` file in the root of the project directory and add your API keys:

    ```dotenv
    PINECONE_API_KEY=<your-pinecone-api-key>
    OPENAI_API_KEY=<your-openai-api-key>
    ```

## Usage

1. **Run the Streamlit app:**

    ```bash
    streamlit run app.py
    ```

2. **Open your browser and navigate to:**

    ```
    http://localhost:8501
    ```

3. **Interact with the app:**

    - Enter your question in the text input field.
    - Click the "Get Answer" button to receive an answer based on the context retrieved from Pinecone and processed by GPT-3.5.

## Code Overview

- `app.py`: Main Streamlit application script.
- `requirements.txt`: Lists all required Python packages.
- `.env`: Contains API keys for Pinecone and OpenAI.

## Troubleshooting

- **API Key Issues**: Ensure your API keys are correctly set in the `.env` file.
- **Dependencies**: Make sure all required packages are installed by checking `requirements.txt`.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or feedback, please contact [your-email@example.com].

