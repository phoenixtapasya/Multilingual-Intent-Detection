# Multilingual Intent Detection with XLM-RoBERTa on the MASSIVE Dataset

This project tackles the complex challenge of **multilingual intent detection** using state-of-the-art **transformer-based models**, with a focus on the **MASSIVE dataset** — a benchmark for multilingual spoken language understanding (SLU) that spans **51 languages** and **60 intent classes**.

## 🔍 Project Overview

We fine-tuned the **XLM-RoBERTa Base** model, known for its robust cross-lingual representations, to classify **English utterances** by intent. The dataset was preprocessed and filtered to include **5,000 English utterances**, ensuring a clean and representative training sample.

Training leveraged **Hugging Face’s `Trainer` API**, optimized with the following strategies:

- **Attention-based tokenization**
- **Max-length truncation** (64 tokens)
- **Dynamic padding** for memory-efficient batch processing
- **AdamW optimizer** with linear learning rate scheduling

---

## 📊 Performance Metrics

| Metric                  | Value               |
|-------------------------|---------------------|
| **Accuracy**            | 86%                 |
| **Weighted F1-score**   | 0.855               |
| **Evaluation Loss**     | 0.606               |
| **Eval Throughput**     | ~487 samples/sec    |
| **Training Throughput** | ~92 samples/sec     |
| **Total Training FLOPs**| 493.6 trillion      |
| **Avg. Training Loss**  | 0.787               |

---

## ⚙️ Key Highlights

- 🚀 **Efficient training pipeline** with excellent scalability and throughput  
- 🧠 **High linguistic generalization** via multilingual pretraining  
- 🎯 **Task-specific fine-tuning** for improved domain accuracy  
- 🔉 Suitable for multilingual digital assistants, voice interfaces, and smart automation

---

## 📁 Dataset

- **MASSIVE** (Multilingual Amazon SLU)  
  - 51 languages  
  - 60 intent classes  
  - Source: [https://huggingface.co/datasets/amazon_massive](https://huggingface.co/datasets/amazon_massive)

---

## 🛠️ Tech Stack

- **Transformers**: [Hugging Face Transformers](https://huggingface.co/transformers)
- **Model**: XLM-RoBERTa Base
- **Trainer API**: Hugging Face `transformers.Trainer`
- **Preprocessing**: Tokenizers, truncation, and dynamic padding
- **Frameworks**: PyTorch, Datasets, Accelerate

---

## 📌 Conclusion

This project offers a robust and computationally efficient backbone for intent classification in multilingual settings. By combining the **cross-lingual power of XLM-RoBERTa** with **fine-tuned task performance**, it sets a solid foundation for building scalable and accurate natural language understanding systems.

