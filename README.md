# DSC-210-Final-Project

## Project Description
This repository contains code for the final project of DSC 210: Linear Algebra at UCSD, Fall 2023. The project is about topic modeling in NLP, and we implemented Latent Semantic Analysis (LSA), Non-negative Matrix Factorization (NMF), and BERTopic. We also implemented some basic classifiers and transformer-based classifiers for comparison.

Instructed by Professor [Lily Weng](https://lilywenglab.github.io/)

## Project Report

The project report can be found [here](https://sweet-vole-3e7.notion.site/Topic-Modeling-in-NLP-A-Linear-Algebra-Perspective-06f1c1fc34b24b429f9a4064510267b4).

## Project Structure/Contents

### Data

We use AG News dataset for our project, which can be downloaded on 🤗 HuggingFace [here](https://huggingface.co/datasets/ag_news).

### Code and Notebooks

- `requirements.txt`: Python dependencies, using `pip install -r requirements.txt` to install.
- `notebooks/text_preprocessing.ipynb`: Notebook for text preprocessing; following the steps in the notebook will save the preprocessed text to `./data` folder.
- `notebooks/lsa.ipynb`: Notebook for running Latent Semantic Analysis (LSA).
- `notebooks/lda.ipynb`: Notebook for running Latent Dirichlet Allocation (LDA); 
    > p.s. the LDA is not included in our final report.
- `notebooks/nmf.ipynb`: Notebook for running Non-negative Matrix Factorization (NMF).
- `notebooks/bertopic.ipynb`: Notebook for running BERTopic.
- `notebooks/basic_classifier.ipynb`: Notebook for running some basic classifiers, e.g., Logistic Regression(LR), Support Vector Machine(SVM), Naive Bayes(NB), and Neural Network(NN).
- `notebooks/transformer_classifier.ipynb`: Notebook for running some transformer-based classifiers, e.g., BERT, RoBERTa, DART.
    > p.s. the transformer-based classifiers are fine-tuned on 1 A100 GPU (80GB), for GPUs with less memory, you may need to reduce the batch size.
