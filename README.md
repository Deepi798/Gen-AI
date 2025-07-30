# 🎶 BTS Lyrics Analyzer (Google Colab Version)

A simple Natural Language Processing (NLP) tool built in **Google Colab** to analyze the lyrics of BTS songs. It allows you to:

- Upload a CSV file of BTS songs
- Choose a song from a list
- View the lyrics
- Generate a summary
- Get a simplified explanation of the song's meaning

---

## 📌 Features

- 📂 Upload your own `bts (1).csv` file
- 🎧 Choose any BTS song from the dataset
- 📜 Display the song’s lyrics (first 1000 characters)
- 📝 Summarize lyrics using `facebook/bart-large-cnn`
- 🔍 Explain meaning in simple English using `gpt2`

---

## 📁 Dataset Format

Your CSV file (`bts (1).csv`) must contain the following columns:

| eng_track_title | lyrics                 |
|------------------|-------------------------|
| Dynamite         | 'Cause I, I'm in the stars tonight... |
| Butter           | Smooth like butter...   |

Place this file in the same directory as your notebook or upload it using Colab.

---

## ▶️ How to Run in Google Colab

1. Open this project in [Google Colab](https://colab.research.google.com/).
2. Upload your dataset:

```python
from google.colab import files
uploaded = files.upload()


