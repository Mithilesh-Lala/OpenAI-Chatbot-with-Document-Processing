# OpenAI Chatbot with Document Processing

This project implements a chatbot using OpenAI's GPT-3.5-turbo model, with the ability to process and reference uploaded documents. The chatbot can understand and respond to queries based on the content of uploaded PDF, DOCX, Excel, JSON, or TXT files.

## Features

- Integration with OpenAI's GPT-3.5-turbo model for natural language processing
- Document upload and processing (PDF, DOCX, Excel, JSON, TXT)
- Text embedding and semantic search using FAISS
- Interactive chat interface built with Streamlit

## Prerequisites

- Python 3.7+
- OpenAI API key

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/Mithilesh-Lala/OpenAI-Chatbot-with-Document-Processing.git
   cd project directory 
   ```

2. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

3. Set up your OpenAI API key:
   - Open the `app.py` file
   - Replace  with your actual OpenAI API key

## Usage

1. Run the Streamlit app:
   ```
   streamlit run app.py
   ```

2. Open your web browser and go to the URL provided by Streamlit (usually `http://localhost:8501`).

3. Upload documents using the sidebar on the left.

4. Start chatting with the bot in the main interface.

## How it works

1. The app allows users to upload various document types.
2. Uploaded documents are processed and their content is embedded using a sentence transformer model.
3. Embeddings are stored in a FAISS index for efficient similarity search.
4. When a user asks a question, the app searches for relevant context in the uploaded documents.
5. The OpenAI GPT-3.5-turbo model generates a response based on the user's question and the relevant context.

## Security Note

Be cautious with your OpenAI API key. The current setup includes the API key directly in the code, which is not recommended for production use. For deployment, consider using environment variables or a secure key management system.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.


