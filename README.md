# **TraCR TMF**

This repository contains a set of modular notebooks exploring different approaches to applying Large Language Models (LLMs) for cybersecurity threat intelligence, with a focus on Retrieval-Augmented Generation (RAG), In-Context Learning (ICL), and Vector Store Indexing techniques.

## **Overview**

With the rise of sophisticated cyber threats, traditional data processing pipelines often fail to capture the complex and multimodal nature of cyber incident data. This project presents a comparative and complementary approach using LLM-powered pipelines to enhance cyber threat detection, classification, and reporting—especially for transportation systems and critical infrastructure.

The repository consists of three main components:

* **RAG Pipeline (`RAG.ipynb`)**: Implements a retrieval-augmented generation pipeline that integrates external threat knowledge bases with LLMs to generate context-aware responses.

* **In-Context Learning (`ICL.ipynb`)**: Demonstrates few-shot learning capabilities of LLMs using representative threat incident examples without the need for fine-tuning.

* **Vector Store Indexing (`Vector_Store_Index.ipynb`)**: Constructs a vector-based search index using embedding models to enable semantic similarity search and efficient retrieval of cyber incident reports.

---

## **Repository Structure**

`├── RAG.ipynb       # Retrieval-Augmented Generation pipeline with custom prompt engineering`  
`├── ICL.ipynb       # In-Context Learning setup with multi-shot examples`  
`├── Vector_Store_Index.ipynb   # Vector index construction and semantic search utilities`  
`└── README.md                  # Project documentation`

---

## **Key Features**

* ✅ **Multimodal Data Processing**: Handles textual and tabular cyber incident data.

* ✅ **Retrieval-Augmented Intelligence**: Combines LLM generative reasoning with relevant external knowledge retrieval.

* ✅ **Few-Shot and Zero-Shot Classification**: Uses ICL methods for flexible threat classification with minimal supervision.

* ✅ **Vector-Based Semantic Search**: Embeds and indexes incidents for fast and accurate similarity search.

* ✅ **OpenAI API Ready**: Easily configurable with OpenAI models like GPT-4 and OpenAI Embeddings.

---

## **Getting Started**

### **Prerequisites**

* Python 3.9+

* OpenAI Python SDK (`openai`)

* FAISS or Chroma for vector indexing

* Other standard Python libraries (`pandas`, `numpy`, `tqdm`, etc.)

You can install dependencies using:

`pip install -r requirements.txt`

### **Usage**

Each notebook can be executed independently. Example order of execution:

1. Run `Vector_Store_Index.ipynb` to generate the vector index from your cyber incident dataset.

2. Use `RAG.ipynb` to build a retrieval pipeline combining LLM with vector-based search.

3. Explore `ICL.ipynb` for few-shot experiments using domain-specific cyber incident examples.

---

## **Use Cases**

* Cyber threat intelligence analysis

* Incident classification for transportation sectors

* Knowledge augmentation for cybersecurity reports

* Rapid prototyping of LLM-powered cybersecurity tools

---

## **Acknowledgements**

This work is based upon the work supported by the National Center for Transportation Cybersecurity and Resiliency (TraCR) (a U.S. Department of Transportation National University Transportation Center) headquartered at Clemson University, Clemson, South Carolina, USA. Any opinions, findings, conclusions, and recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of TraCR, and the U.S. Government assumes no liability for the contents or use thereof.

---

## **License**

---

