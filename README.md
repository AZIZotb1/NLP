# Natural Language Processing Labs

A collection of Jupyter notebooks covering core Natural Language Processing techniques, from text
pre-processing and n-gram language models to word embeddings, neural networks, transformers and attention.

## Contents

| Lab | Topic | Highlights |
|---|---|---|
| [Lab01](Lab01) | Introduction to NLP | Text data formats, loading and exploring the IMDB 50K reviews dataset |
| [Lab02](Lab02) | Text Pre-processing & Regular Expressions | Tokenization, stemming, lemmatization, stop words, hashtag analysis with regex |
| [Lab03](Lab03) | N-Grams | Bigram language model, tweet generation, probabilities and perplexity |
| [Lab04](Lab04) | Classification & Evaluation | Sentiment analysis with TF-IDF and Naive Bayes, classification report, confusion matrix |
| [Lab05](Lab05) | Text Representation | TF-IDF, cosine similarity, skip-gram Word2Vec |
| [Lab06](Lab06) | Deep Learning for NLP | Review classification with PyTorch neural networks on TF-IDF and Word2Vec features |
| [Lab07](Lab07) | Large Language Models | Encoder-only, encoder–decoder and decoder-only transformers (DistilBERT, FLAN-T5, DistilGPT-2) |
| [Lab08](Lab08) | Part-of-Speech Tagging | NLTK and spaCy POS tagging, ambiguity, dependency visualization |
| [Lab09](Lab09) | Named Entity Recognition | spaCy NER, rule-based entity matching, training a custom NER model |
| [Lab10](Lab10) | Machine Translation | LSTM encoder–decoder for English → French translation, BLEU evaluation |
| [Lab11](Lab11) | Attention | RNN with attention for question answering, attention-weight visualization |

## Requirements

- Python 3.12
- `numpy`, `pandas`, `scikit-learn`, `matplotlib`
- `nltk`, `spacy` (with `en_core_web_sm`), `gensim`, `emoji`
- `torch`, `tensorflow`, `transformers`, `sentencepiece`
- `kagglehub`

```bash
pip install numpy pandas scikit-learn matplotlib nltk spacy gensim emoji torch tensorflow transformers sentencepiece kagglehub
python -m spacy download en_core_web_sm
```

The notebooks also run on Google Colab.

## Datasets

Most datasets are downloaded automatically from Kaggle with `kagglehub` when the notebooks run.
Labs 5, 6 and 11 read local files from a `dataset/` folder inside the lab directory:

| Lab | File |
|---|---|
| Lab05 | `dataset/simpsons_script_lines.csv` |
| Lab06 | `dataset/07-yelp-dataset.txt` |
| Lab11 | `dataset/Lab_11_QnA_Dataset.csv` |
