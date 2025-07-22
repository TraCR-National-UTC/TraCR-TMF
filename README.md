# **TraCR TMF**

This repository contains a set of modular notebooks exploring different approaches to applying Large Language Models (LLMs) for cybersecurity threat intelligence, with a focus on Retrieval-Augmented Generation (RAG), In-Context Learning (ICL), Vector Store Indexing, and Supervised Learning techniques.

## **Overview**

With the rise of sophisticated cyber threats, traditional data processing pipelines often fail to capture the complex and multimodal nature of cyber incident data. This project presents a comparative and complementary approach using LLM-powered pipelines to enhance cyber threat detection, classification, and reporting—especially for transportation systems and critical infrastructure.

The repository consists of four main components:

* **RAG Pipeline (`RAG.ipynb`)**: Implements a retrieval-augmented generation pipeline that integrates external threat knowledge bases with LLMs to generate context-aware responses.

* **In-Context Learning (`ICL.ipynb`)**: Demonstrates few-shot learning capabilities of LLMs using representative threat incident examples without the need for fine-tuning.

* **Vector Store Indexing (`Vector_Store_Index.ipynb`)**: Constructs a vector-based search index using embedding models to enable semantic similarity search and efficient retrieval of cyber incident reports.

* **Supervised Learning (`Fine_Tuning.ipynb`)**: Fine-tunes a pre-treained ModernBERT model for multi-label classification to identify relevant MITRE ATT&CK techniques in transportation CPS data flows.

---

## **Key Features**

* ✅ **Retrieval-Augmented Intelligence**: Combines LLM generative reasoning with relevant external knowledge retrieval.

* ✅ **Few-Shot and Zero-Shot Classification**: Uses ICL methods for flexible threat classification with minimal supervision.

* ✅ **Vector-Based Semantic Search**: Embeds and indexes incidents for fast and accurate similarity search.

* ✅ **OpenAI API Ready**: Easily configurable with OpenAI models like GPT-4 and OpenAI Embeddings.

* ✅ **Supervised Fine-Tuning Pipeline**: Leverages transfer learning on ModernBERT for multi-label classification of MITRE ATT&CK techniques in transportation CPS data flows, enhancing performance through supervised learning with ground-truth labels.

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

2. Run `RAG.ipynb` to build a retrieval pipeline combining LLM with vector-based search.

3. Run `ICL.ipynb` for few-shot experiments using domain-specific cyber incident examples.

4. Run `Fine_Tuning.ipynb` and `ARC_IT_dataset_evaluation.ipynb` to train the ModernBERT model via supervised fine-tuning and evaluate its performance on the ARC-IT dataset.

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

https://tracr-tmf-models.s3.us-east-2.amazonaws.com/model_ckpt_kfold.zip

