## LLM and RAG-based Invoice Data Retrieval

This project implements a Python-based solution for extracting and analyzing data from PDF invoices using Large Language Models (LLM) and Retrieval-Augmented Generation (RAG).

### Features

1. **PDF text extraction and preprocessing**: The project uses the `PyPDFLoader` from the `langchain_community` library to extract text content from PDF invoices.

2. **LLM integration for intelligent data extraction**: The project integrates the `ChatGoogleGenerativeAI` model from the `langchain_google_genai` library to interpret and extract key information from the invoice text.

3. **RAG implementation for enhanced accuracy**: The project implements a RAG-based approach, where a knowledge base is created using the `FAISS` vector store from the `langchain_community` library. This knowledge base is used to retrieve relevant information to enhance the accuracy of the data extraction.

4. **User-prompt based information retrieval**: The project provides a user-friendly interface that allows users to input queries, and the system responds with the relevant invoice details.

### Objectives

1. **Process PDF invoices and extract text content**: The project aims to efficiently process PDF invoices and extract the text content for further analysis.

2. **Utilize LLM to interpret and extract key information**: The project leverages the capabilities of Large Language Models to interpret the invoice text and extract relevant information.

3. **Implement RAG to improve extraction accuracy**: The project incorporates a Retrieval-Augmented Generation approach to enhance the accuracy of the data extraction by utilizing a knowledge base.

4. **Provide a user-friendly interface for data retrieval based on prompts**: The project offers a user-friendly interface where users can input queries, and the system retrieves the relevant invoice details.

### Implementation

1. **PDF Processing**: The project uses the `PyPDFLoader` from the `langchain_community` library to extract and preprocess the text content from the PDF invoices.

2. **LLM Integration**: The project connects to the `ChatGoogleGenerativeAI` model from the `langchain_google_genai` library to interpret and extract key information from the invoice text.

3. **RAG Implementation**: The project creates a knowledge base using the `FAISS` vector store from the `langchain_community` library. This knowledge base is then used to retrieve relevant information to enhance the accuracy of the data extraction.

4. **User-prompt based information retrieval**: The project provides a user-friendly interface where users can input queries, and the system responds with the relevant invoice details using the LLM and RAG-based approach.

### Requirements

- Python 3.x
- Required Python libraries:
  - `langchain_community`
  - `langchain_text_splitters`
  - `langchain_google_genai`
  - `langchain.chains`
  - `langchain.chains.combine_documents`
  - `langchain_core.prompts`
  - `google.generativeai`
  - `langchain_community.vectorstores`

### Usage

1. Set up the Google API key in the `os.environ` variable.
2. Load the PDF invoices using the `PyPDFLoader` and create a FAISS vector store for the invoice data and the knowledge base.
3. Implement the `llm_ans` function to handle user queries and provide the relevant invoice details.
4. Run the interactive loop to accept user input and display the corresponding invoice information.

### Future Improvements

- Enhance the user interface for a more seamless experience.
- Incorporate additional data sources beyond PDF invoices.
- Explore advanced techniques for improving the accuracy of the data extraction.
- Implement the ability to save and retrieve previous user queries and responses.
