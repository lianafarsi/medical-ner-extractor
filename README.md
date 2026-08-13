# Medical NER Extractor (BioBERT)

An advanced Natural Language Processing (NLP) pipeline designed to extract crucial biomedical entities—such as drugs, dosages, and medical conditions—from raw clinical transcriptions using fine-tuned transformer models.

## 🚀 Project Overview
In the digital health and healthtech sectors, extracting structured data from unstructured or messy clinical texts is critical for modern electronic health record (EHR) systems. This project leverages **BioBERT** via Hugging Face `transformers` to automatically parse and recognize medical entities with high precision, converting unstructured notes into clean, structured dataframes ready for clinical downstream tasks.

## 🛠️ Tech Stack
* **Python** (Core programming language)
* **Hugging Face Transformers** (For state-of-the-art BioBERT token classification)
* **PyTorch** (Deep learning backend)
* **Pandas & NumPy** (Data structuring and manipulation)
* **Regex** (Text preprocessing and noise reduction)


Engineering Best Practices & Safety Standards
Modular Architecture: Strict separation of concerns (SoC) dividing preprocessing logic, model inference, and execution pipelines.

Confidence Thresholding: Implements rigorous score filters to discard low-confidence model predictions, ensuring clinical data reliability and safety-critical compliance.

Data Hygiene & Robustness: Automated handling of missing dataset values (NaN), structural duplicate removal, and dynamic path management to prevent runtime failures.

💡 Future Enhancements
Integration with relational databases (PostgreSQL) for direct EHR ingestion.

Fine-tuning BioBERT on custom domain-specific clinical datasets.

Building a lightweight REST API wrapper using FastAPI for real-time inference.
