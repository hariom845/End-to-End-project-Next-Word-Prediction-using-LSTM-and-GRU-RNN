# Next Word Prediction using LSTM & GRU RNN  
*(End-to-End Project)*

---

## 📌 Project Overview

This project is about predicting the next word in a sequence using deep learning techniques.  
It uses **LSTM** and **GRU** recurrent neural networks, with data preparation, training, and an application component to demonstrate predictions.  

---

## 🚀 Features

- Data preprocessing using a large text corpus (e.g. *Hamlet*)  
- Tokenization and sequence generation  
- Training two different RNN architectures: LSTM and GRU  
- Saved trained models (`.h5` files) and tokenizer pickles  
- A simple `app.py` to interactively generate next-word predictions  
- Experiment notebook to try different parameters  

---

## 📂 Project Structure

├── app.py # Script for interacting/generating predictions

├── experiment.ipynb # Notebook for experimentation (parameter tuning etc.)

├── hamlet.txt # Sample text corpus

├── next_word_Gru.h5 # Saved GRU model

├── requirement.txt # Required Python packages

├── tokenizer.pickle # Tokenizer object for sequence generation

└── .gitignore # Files/folders to be ignored in version control

---

## ⚙️ Getting Started

### 1️⃣ Prerequisites

- Python 3.7+  
- Packages in `requirement.txt` (like TensorFlow or Keras, etc.)  

### 2️⃣ Installation

# Clone this repo
git clone https://github.com/hariom845/End-to-End-project-Next-Word-Prediction-using-LSTM-and-GRU-RNN.git
cd End-to-End-project-Next-Word-Prediction-using-LSTM-and-GRU-RNN

# (Optional) set up virtual environment
python3 -m venv venv
source venv/bin/activate

# Install requirements
pip install -r requirement.txt

# To train models (if you want to retrain)

You can use the notebook experiment.ipynb, or write a script to:
- load corpus (e.g. hamlet.txt)
- tokenize text and generate sequences
- build and train either LSTM or GRU model
- save modelo .h5 and tokenizer
(Note: The GRU model is already saved as next_word_Gru.h5.)

# To run interactive prediction via app.py
You’ll be prompted (or have inputs) to enter a sequence of words, and the model will predict the next word using the trained tokenizer and model.

# 🧪 Testing / Experiments

- Check experiment.ipynb for different architectures / parameters and their results.
- You can test the model’s predictions with various input text sequences to observe how well it generalizes.

🔮 Future Improvements

- Support for saving & using the LSTM model similarly to the GRU model
- More text corpora (e.g. different genres, languages) to make model more robust
- Hyperparameter tuning (layers, dropout, sequence length)
- Deploy the model as a web API or UI for easier use
- Add evaluation metrics (perplexity, BLEU, etc.)
