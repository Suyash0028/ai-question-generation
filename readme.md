# AI-Powered Question Generation from Text  

## 📌 Overview
This project focuses on automatically generating questions from a given text passage using deep learning models. The goal is to leverage pre-trained Transformer models (T5 and BART) to generate relevant questions, helping improve educational tools and assessment systems.

## 🧠 Models Used
- **T5 (Text-to-Text Transfer Transformer)**  
- **BART (Bidirectional and Auto-Regressive Transformer)**

## 📁 Dataset
- Dataset used: `train.csv` (accessed from Google Drive)
- It includes two main columns: `context` and `question`
- Sampled **10,000** rows for training and evaluation

## ⚙️ Setup Instructions

### 1. Mount Google Drive
To access the dataset:
```python
from google.colab import drive
drive.mount('/content/drive')
```

### 2. Install Required Libraries

```bash
!pip install datasets
!pip install nltk rouge-score
```

### 3. Import Python Libraries

* `pandas`, `numpy`, `torch`
* `transformers` for T5 and BART
* `nltk` and `rouge_score` for evaluation
* `sklearn` for data splitting and metrics
* `matplotlib`, `seaborn` for visualization

## 🧪 Preprocessing

Each context is transformed into a prompt for generation:

```python
input_text = f"generate question: {context}"
```

## 🧮 Evaluation Metrics

The performance of the models was evaluated using:

* **BLEU Score**
* **ROUGE Score**
* **Precision, Recall, F1 Score**

## 🚀 How to Run

1. Open the notebook in Google Colab.
2. Mount your Google Drive and ensure the correct path to `train.csv`.
3. Select T5 or BART for training and testing.
4. Evaluate the model and visualize results using metrics and plots.

## 📊 Output

* Generated questions from input context
* Model performance comparison (T5 vs BART)
* Visual analysis of scores

## 🤝 Acknowledgements

Thanks to HuggingFace Transformers and Google Colab for their powerful tools and platforms.# question-generation-project
