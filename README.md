# RAG-Mistral7b
RAG (Retrievel Augmented Generation) implementation using the **Mistral-7B-Instruct-v0.1**

## Project Description
This repository contains the implementation of the Retrieval Augmented Generation (RAG) model, using the newly released Mistral-7B-Instruct-v0.1 as the Language Model, SentenceTransformers for embedding, and llama-index for data ingestion, vectorization, and storage. The model has been implemented in a Google Colab notebook, optimized for a v100 instance.

The implementation focuses on querying data from Amazon’s Annual Report for the fiscal year ended December 31, 2022. This enables the extraction of insightful information and knowledge encapsulated in the fiscal documents.

## Contents
- `RAG_testing_mistral7b.ipynb` : The main Google Colab notebook containing the entire implementation and execution details.

## Prerequisites
- Google Colab with v100 instance.
- Knowledge on RAG, SentenceTransformers, and Mistral 7B models.
- Access token for HuggingFace (read)

## Quick Start
1. Clone the repository:
   ```shell
   git clone <repository_url>
   ```
2. Open the `RAG_testing_mistral7b.ipynb` notebook in Google Colab.
3. Set up the environment with the necessary libraries and dependencies.
4. Create a new folder called "data" and store the Amazon 10k repport in it.
5. Run the notebook cells in sequence.

## Implementation Details
### 1. **Mistral 7B Model (LLM)**
   This implementation utilizes Mistral 7B as the Large Language Model to generate human-like, coherent responses based on the retrieved documents.

### 2. **SentenceTransformers (Embedding Model)**
   SentenceTransformers is used to create embeddings for the sentences, enabling efficient and semantic similarity search among them. **all-mpnet-base-v2** pretrained model was used as it had the best performance. 

### 3. **llama-index (Data Ingestion, Vectorization, and Storage)**
   llama-index is employed for ingesting and vectorizing the dataset and for storing the vectorized representations of the data.

### 4. **Data Source**
   The data queried in this implementation is sourced from Amazon’s Annual Report for the fiscal year ended December 31, 2022. 

## Usage
Follow the instructions in the `RAG_testing_mistral7b.ipynb` notebook to run the cells and execute the implementation on Google Colab.

## License
This project is licensed under the MIT License.

## Acknowledgments
- The entire team at Mistral for the powerful language model.
- SentenceTransformers for the efficient embedding model.
- llama-index for data ingestion and vectorization.
- Amazon for the annual report data.

## Contact
For any queries or discussions related to this implementation, feel free to raise an issue in this GitHub repository.
