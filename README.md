## RAG System for Resume with LLAMA

This is a lightweight Retrieval-Augmented Generation (RAG) system built using open-source tools. It allows you to query your PDF resume using natural language and get contextual answers powered by a local LLaMA model.


## LLaMA Model Setup

This project uses the [LLaMA 2 7B Chat GGUF model](https://huggingface.co/TheBloke/LLaMA-2-7B-Chat-GGUF).

### Download Instructions

1. Go to [TheBloke/LLaMA-2-7B-Chat-GGUF](https://huggingface.co/TheBloke/LLaMA-2-7B-Chat-GGUF).
2. Download the file: `llama-2-7b-chat.Q4_K_M.gguf` (or any quantized variant).
3. Place the file in the desired location.


### Note
1. This model file is not included in the repo due to its size.
2. Resume pdf file is not included in the repo. Please utilize your own resume/pdf.


## Features

-  Query PDFs like resumes using natural language
-  Local vector store using FAISS
-  LLaMA 2 (7B) model via `llama-cpp-python`
-  No OpenAI or API keys required
-  Modular and easily extensible

## Tech Stack

| Component | Library/Tool |
|----------|---------------|
| PDF Reader | LangChain + PyPDF |
| Embeddings | Sentence Transformers |
| Vector Store | FAISS |
| LLM | `llama-cpp-python` |
| Framework | LangChain |


## Requirements

See [requirements.txt](requirements.txt)

## Usage

### 1. Install Dependencies

```bash
pip install -r requirements.txt