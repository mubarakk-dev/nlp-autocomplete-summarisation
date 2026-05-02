# NLP Pipeline: Sentence Autocomplete and Summarisation

This project implements an end-to-end Natural Language Processing (NLP) pipeline that combines text generation and summarisation into a single workflow.

The system takes a partial input paragraph, generates a continuation using a language model, and then produces a concise summary of the generated text.

---

## 🚀 Features

- Sentence autocomplete using GPT-2  
- Text summarisation using BART  
- End-to-end pipeline integration  
- Evaluation using ROUGE metrics  
- Interactive interface using Gradio  

---

## 🧠 How It Works

The system follows a sequential pipeline:

1. **Input** – User provides a partial text prompt  
2. **Generation** – GPT-2 generates a continuation  
3. **Summarisation** – BART summarises the generated text  
4. **Output** – Completed text and summary are displayed  

This design demonstrates how multiple NLP components can be integrated into a unified system.

---

## 📊 Dataset

- CNN/DailyMail dataset  
- Contains news articles and human-written summaries  
- Used for both generation prompts and evaluation  

---

## ⚙️ Tech Stack

- Python  
- Hugging Face Transformers  
- PyTorch  
- Hugging Face Datasets  
- Evaluate (ROUGE)  
- Pandas  
- Gradio  

---

## 📈 Results

The system was evaluated using ROUGE metrics:

- ROUGE-1: 0.23  
- ROUGE-2: 0.07  
- ROUGE-L: 0.17  

These results show that the model captures key information but struggles with precise phrasing and structure.

---

## ⚠️ Key Insights

### 1. Error Propagation
The summarisation stage depends on generated text.  
Errors introduced during generation directly affect the final summary.

### 2. Domain Sensitivity
The system performs well on structured, news-style input but produces weaker results on creative or ambiguous text.

### 3. Pretrained Model Limitations
The models were not fine-tuned for this task, which limits performance and domain adaptation.

---

## 🖥️ Example

**Input:**
> A leading renewable energy company has unveiled plans to expand its operations...

**Output:**
- Generated continuation (GPT-2)  
- Summary (BART)  

---

## 📌 Notes

This project demonstrates:
- Integration of transformer models  
- Practical NLP pipeline design  
- Trade-offs between performance and simplicity  

---

## 📎 Future Work

- Fine-tuning models on domain-specific data  
- Training models from scratch  
- Using semantic evaluation metrics (e.g. BERTScore)  
- Improving factual consistency in generation  

---

## 👨‍💻 Author

Developed as part of an NLP project.
