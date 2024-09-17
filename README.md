# Vectorize the data

To train a classifier that will predict whether articles come from a fake news source (e.g., `Infowars`) or a quality news outlet (e.g., `bbc`). In other words, I want to predict `source` based on linguistic variations in the articles.

To arrive at a model that will do just that, I transform 'text' to 'features'. By defining different vectorizers, with the following options:
- `count` vs. `tfidf` vectorizers
- with/ without pruning
- with/ without stopword removal

# Fit a Classifier - Compare Metrics
I implemented a few simple supervised model: **MultinomialNB** and **LogisticRegression** to predict the `media outlet source` ('Infowars', 'BBC', 'The Guardian') using linguistic variations in the articles.

I also tested a combination of pre-processing steps + vectorizer to determine one with the best results. **CountVectorizer** gives the best overall metrics as compared to **TfidVectorizer**
