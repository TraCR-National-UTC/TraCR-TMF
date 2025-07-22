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

* ✅ **Fine-Tuning Pipeline**: Leverages transfer learning on ModernBERT for multi-label classification of MITRE ATT&CK techniques in transportation CPS data flows, enhancing performance through supervised learning.

---

## **Project Structure**
The project is organized into folders for data, notebooks by approach, and supporting files. The `data/` folder contains the dataset used across notebooks and k-fold splits , particularly for supervised learning. Notebooks are mapped to their respective folders as follows:

* `in_context_learning/`: Contains `ICL.ipynb` for in-context learning experiments.
* `rag/`: Contains RAG.ipynb and `Vector_Store_Index.ipynb` for RAG and vector indexing.
* `supervised_learning/`: Contains `Fine_Tuning.ipynb` for model fine-tuning and `ARC_IT_dataset_evaluation.ipynb` for evaluation on the ARC-IT dataset.

Additionally, trained model checkpoints from the 5-fold cross-validation fine-tuning process are available as a zip file hosted on Amazon S3: [model_ckpt_kfold.zip](https://tracr-tmf-models.s3.us-east-2.amazonaws.com/model_ckpt_kfold.zip). These can be downloaded and used for inference or further evaluatoin in the `ARC_IT_dataset_evaluation.ipynb` notebook within the supervised learning folder.

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

