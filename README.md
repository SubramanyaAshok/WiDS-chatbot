# WiDS 5.0 – Human-like Conversational Chatbot

This repository contains the final project developed as part of WIDS 5.0.
The goal of this project is to improve human-like conversational responses by
fine-tuning a pretrained DialoGPT model.

## Overview
The project focuses on building a conversational chatbot that produces more
natural, coherent, and human-like responses. Improvements were achieved through
feature engineering, model upgrades, hyperparameter tuning, and controlled text
generation strategies.

## Dataset
The project uses the 'Cornell Movie-Dialogue Corpus'.
Due to size and licensing considerations, the dataset files
  ('movie_lines.txt', `movie_conversations.txt') are not included in this repository.

## Model
- Base Model: DialoGPT-medium
- Architecture: Transformer (decoder-only)
- Training Objective: Causal Language Modeling

## Improvements
- Speaker-role based feature engineering (User:` / `Bot:)
- Model upgrade from DialoGPT-small to DialoGPT-medium
- Hyperparameter tuning (epochs, batch size, sequence length)
- Controlled response generation using temperature scaling, top-p sampling,
  and repetition penalty
- Response length control for improved conversational quality



**Repository Structure**
monologue_wids_final.ipynb
app.py
requirements.txt
README.md

---

## Streamlit Deployment
A simple Streamlit-based web application is provided to interact with the
fine-tuned chatbot. The app loads the trained model and generates responses
in real time.

 To run locally:
```bash
pip install -r requirements.txt
streamlit run app.py


## Note :
-Trained model weights are not included in this repository due to size constraints.
-If GitHub preview shows the notebook as invalid, please download it and open
 it using Colab or Jupyter Notebook.




