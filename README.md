# josa-corpus
Jopara (Guarani-dominant mixed with Spanish) sentiment analysis corpus.

## Corpora

We created two Corpora: balanced and unbalanced. The balanced (1526) was created from the unbalanced (3941).

### TweetIDs

Tweet IDs, the content can rehydrate (i.e. request the full Tweet) using the Twitter APIs. See [Redistribution of Twitter content](https://developer.twitter.com/en/developer-terms/more-on-restricted-use-cases).
Consider [hydrated](https://catalog.docnow.io/datasets/20210506-jopara-guarani-dominant-mixed-with-spanish-sentiment-analysis-corpus/) them back into full datasets using a **Hydrator** (e.g., [DocNow](https://catalog.docnow.io/)).

Go to [Harvard Dataverse repository](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/GLDX14). [](https://catalog.docnow.io/datasets/20210506-jopara-guarani-dominant-mixed-with-spanish-sentiment-analysis-corpus/).

### Tweets downloader

If you are curious and want to know how we download these particular tweets, go to this [GitHub repository](https://github.com/mmaguero/guarani-tweets) (see also [tweets-downloader repository](https://github.com/mmaguero/tweets-downloader)).

## Baselines

### Traditional machine learning

(Complement) Naïve Bayes and SVMs for unbalanced datasets.

Go to [GitHub repository](https://github.com/mmaguero/textcat-josa).

### Neural-Networs text-classifiers

BiLSTM-CNN, CNN-BiLSTM char-word-embeddings, also pre-trained non-contextualized representations (Spanish, Guarani, and Multilingual): FastText’s word and BPEmb’s subword vectors.

Go to [Google Colab notebook](https://colab.research.google.com/drive/1egleuWnjo6qomFk_6eZvb3pI3FLi0WsZ?usp=sharing).

### Pre-trained language models (BERT-based)

Fine-tuning: Spanish BERT (BETO), Multilingual BERT (102 languages) and XLM (15 languages) (none of the language models used
considered Guarani during pre-training).

Go to [Google Colab notebook](https://colab.research.google.com/drive/1eHnF1GsMScHXAldl0VJ2-usdkhfdO7X_?usp=sharing).

## How do I cite this work?

Please, cite this paper [On the logistical difficulties and findings of Jopara Sentiment Analysis](https://aclanthology.org/2021.calcs-1.12/):

Marvin Agüero-Torales, David Vilares, and Antonio López-Herrera. 2021. On the logistical difficulties and findings of Jopara Sentiment Analysis. In Proceedings of the *CALCS 2021 (co-located with NAACL 2021)* [Fifth Workshop on Computational Approaches to Linguistic Code Switching](https://code-switching.github.io/2021), pages 95–102, Online. Association for Computational Linguistics.

```
@inproceedings{aguero-torales-etal-2021-logistical,
    title = "On the logistical difficulties and findings of Jopara Sentiment Analysis",
    author = {Ag{\"u}ero-Torales, Marvin  and
      Vilares, David  and
      L{\'o}pez-Herrera, Antonio},
    booktitle = "Proceedings of the Fifth Workshop on Computational Approaches to Linguistic Code-Switching",
    month = jun,
    year = "2021",
    address = "Online",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2021.calcs-1.12",
    doi = "10.18653/v1/2021.calcs-1.12",
    pages = "95--102",
    abstract = "This paper addresses the problem of sentiment analysis for Jopara, a code-switching language between Guarani and Spanish. We first collect a corpus of Guarani-dominant tweets and discuss on the difficulties of finding quality data for even relatively easy-to-annotate tasks, such as sentiment analysis. Then, we train a set of neural models, including pre-trained language models, and explore whether they perform better than traditional machine learning ones in this low-resource setup. Transformer architectures obtain the best results, despite not considering Guarani during pre-training, but traditional machine learning models perform close due to the low-resource nature of the problem.",
}

```
