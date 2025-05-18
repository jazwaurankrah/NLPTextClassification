📄README.md

# Autocorrect Models for Natural Language Processing

This project was developed for **CS-4742 (Natural Language Processing)** at Kennesaw State University by:
**Jazwaur A., Spencer F., Nicholas H., and Cassidy S.**

Our goal was to research and compare various approaches to autocorrection in text applications using natural language models. We implemented and tested multiple techniques including:

- **Levenshtein Distance**
- **Keyboard Proximity Correction**
- **Contextual BERT**
- **Chebyshev-based BERT**
- **BART Transformer Model**

---

## 🔍 Project Overview

Autocorrection is a critical function in NLP applications such as messaging, virtual assistants, and search engines. This project explores:

- How edit distance and keyboard-based techniques can serve as baselines
- How transformer models (BERT, BART) can enhance contextual predictions
- Quantitative and qualitative comparisons across correction methods

---

## 📁 Directory Structure
project-autocorrect/
├── .gitattributes
├── .gitignore
├── README.md
├── src/
│   ├── autocorrect/
│   │   ├── BART.py
│   │   ├── BERT.py
│   │   ├── ChebyshevBERT.py
│   │   ├── LevenshteinBERT.py
│   │   ├── keyboard_approach.py
│   ├── dataset/
│   │   ├── data_transform.py
│   │   ├── original_DailyDialog_train.txt
│   │   ├── train.csv
│   │   ├── train.txt
│   │   ├── train(OLD).csv


---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/jazwaurankrah/project-autocorrect.git
   cd project-autocorrect/src
   
2. Install dependencies (create a virtual environment first if needed):
  pip install -r requirements.txt

3. Run any of the model scripts:
   python autocorrect/BERT.py


| Model                  | Technique                        | Description                                                  |
| ---------------------- | -------------------------------- | ------------------------------------------------------------ |
| `LevenshteinBERT.py`   | Edit Distance + BERT             | Suggests corrections using word distance and BERT embeddings |
| `ChebyshevBERT.py`     | QWERTY Chebyshev Distance + BERT | Uses spatial key distances and semantic context              |
| `keyboard_approach.py` | Keyboard-based heuristics        | Classic autocorrect logic using proximity                    |
| `BERT.py`              | Pure Transformer (BERT)          | Context-aware suggestions                                    |
| `BART.py`              | Transformer-based Seq2Seq        | End-to-end autocorrect via generative modeling               |

📊 Dataset
We used the DailyDialog dataset for training and evaluation.

License: CC BY-NC-SA 4.0

Format: CSV and plain text

📌 Contributors
Jazwaur Ankrah
Spencer F.
Nicholas H.
Cassidy S.

📜 License
This repository is for educational use only. Dataset license: CC BY-NC-SA 4.0

