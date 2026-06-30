# Customer Review Sentiment Analysis using DistilBERT
An implementation of a customer review sentiment analysis pipeline using DistilBERT and traditional NLP techniques. The project was customized with improved documentation, analysis, and model evaluation
## Dataset

The project utilizes the Amazon Fine Food Reviews dataset from Kaggle, containing over 500,000 customer reviews for multi-class sentiment classification.. The dataset comes from a Kaggle competition. It can be downloaded from <a href="https://www.kaggle.com/snap/amazon-fine-food-reviews/download" > here </a>(254MB).

## Task

This is a multi-class classification. Reviews should be classified into three classes <b>Negative</b>, <b>Positive</b>, <b>Neutral</b>.

## Used approaches

- Simple vectorization approaches: CountVectorizer and Tf-idf with Scikit-learn.
- Different Pretrained Word Embeddings: Glove, Word2Vec and FastText with Gensim.
- Different visualization approaches: PCA, t-SNE
- Bert embeddings (DistilBERT) with Transformers - Hugging Face.
- Fine-tuned Bert with pyTorch.

## Results

| Method                                   | F1 macro avg. |
| ---------------------------------------- | :-----------: |
| Glove embeddings + SGD                   |     0.46      |
| DistilBERT embeddings + SGD              |     0.566     |
| DistilBERT embeddings + Logistic + stack |     0.69      |
| DistliBERT Fine-tuned                    |     0.75      |
