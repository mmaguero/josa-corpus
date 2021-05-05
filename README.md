# josa-corpus
Jopara (Guarani-dominant mixed with Spanish) sentiment analysis corpus.

## Corpora

We created two Corpora: balanced and unbalanced. The balanced (1526) was created from the unbalanced (3941).

### TweetIDs

Tweet IDs, which the content can rehydrate (i.e. request the full Tweet) using the Twitter APIs. See [Redistribution of Twitter content](https://developer.twitter.com/en/developer-terms/more-on-restricted-use-cases).

[Harvard Dataverse repository](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/GLDX14).

## Baselines

### Traditional machine learning

(Complement) Naïve Bayes and SVMs for unbalanced datasets.

[GitHub repository](https://github.com/mmaguero/textcat-josa).

### Neural-Networs text-classifiers

BiLSTM-CNN, CNN-BiLSTM char-word-embeddings, also pre-trained non-contextualized representations (Spanish, Guarani, and Multilingual): FastText’s word and BPEmb’s subword vectors.

[Google Colab notebook](https://colab.research.google.com/drive/1egleuWnjo6qomFk_6eZvb3pI3FLi0WsZ?usp=sharing).

### Pre-trained language models (BERT-based)

Fine-tuning: Spanish BERT (BETO), Multilingual BERT (102 languages) and XLM (15 languages) (none of the language models used
considered Guarani during pre-training).

[Google Colab notebook](https://colab.research.google.com/drive/1eHnF1GsMScHXAldl0VJ2-usdkhfdO7X_?usp=sharing).

## How do I cite this work?

Please, cite this paper [On the logistical difficulties and findings of Jopara Sentiment Analysis](https://code-switching.github.io/2021):

Marvin M. Agüero-Torales, David Vilares, Antonio G. López-Herrera (2021). On the logistical difficulties and findings of Jopara Sentiment Analysis. In Proceedings on *CALCS 2021 (co-located with NAACL 2021) - Fifth Workshop on Computational Approaches to Linguistic Code Switching*, to appear (June).

```
BibTeX format pending
```
