# PROJECT TITLE:
## Interactive-Document-Q-A-with-Python-RAG-CLI

Clearly explain how to install Python, clone the repo, set up environment, install dependencies, and run the CLI commands (--upload and --ask).

### CLI usage:
Describe how to use the command line interface with examples, e.g.:

bash
Copy
Edit
python main.py --upload sample.txt
python main.py --ask "What is Python?"
Architecture overview:
Briefly explain the main components of your RAG system:

### Ingestion: Upload and chunk documents

### Retrieval: Find relevant document chunks based on the question

### Generation: Use an LLM to generate answers from retrieved chunks

# Limitations:

Limited document formats supported (txt, md)

Accuracy depends on LLM and retrieval quality

May not handle very large documents efficiently

No GUI, CLI only

# 2. Design Choices
Document why and how you selected key parts of your system:

Tech stack:
Python, argparse for CLI, custom modules for ingestion, retrieval, and generation, and external APIs/libraries for embeddings and language model integration

LLM selection:
This project uses Cohere’s "command-r-plus" for generation and "embed-english-v3.0" for embeddings, chosen for their strong language understanding, easy API use, and cost-effectiveness in RAG systems.

Chunking strategy:
Documents are split into fixed-size text chunks to improve retrieval and make embedding more efficient.

Embedding strategy:
This project uses Cohere’s embed-english-v3.0 model to convert text chunks into vector embeddings. These embeddings are stored in a vector database and used to retrieve the most relevant chunks based on semantic similarity to the user's query.
### Setup steps:
Clearly explain how to install Python, clone the repo, set up environment, install dependencies, and run the CLI commands (--upload and --ask).

### CLI usage:
Describe how to use the command line interface with examples, e.g.:

bash
Copy
Edit
python main.py --upload sample.txt
python main.py --ask "What is Python?"
Architecture overview:
Briefly explain the main components of your RAG system:

### Ingestion: Upload and chunk documents

### Retrieval: Find relevant document chunks based on the question

### Generation: Use an LLM to generate answers from retrieved chunks

# Limitations:

Limited document formats supported (txt, md)

Accuracy depends on LLM and retrieval quality

May not handle very large documents efficiently

No GUI, CLI only



Embedding strategy:
This project uses Cohere’s embed-english-v3.0 model to convert text chunks into vector embeddings. These embeddings are stored in a vector database and used to retrieve the most relevant chunks based on semantic similarity to the user's query.
