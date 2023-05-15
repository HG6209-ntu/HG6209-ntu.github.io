---
title: 'HG2051 (AY22/23) Project 2: Group assignment'
---

##   Introduction

This project constitutes 30% of your final grade for HG2051. Please work on the
final program in groups of 2-3 and report together.

- The goal of this assignment is to demonstrate your programming and
problem-solving abilities through teamwork. If your team has an idea for
another project that you would like to do instead, talk to me for approval.

- This project involves text classification using machine learning tools. As
with the individual project, your team will be required to submit data, output,
and annotated code along with a short writeup that describes your goals,
process, and results. Your code will be assessed based on its functionality and
simplicity.

## Project 2: Text classification

Text classification is a general term for automatically identifying properties
of a text based on its linguistic content. For this project you will develop a
program that classifies short texts based on their polarity/sentiment (positive,
negative, neutral), improving on existing tools.

NLTK has an in-built sentiment analyzer  that determines polarity of a short
text (like a sentence). You can use it like this:

```python
>>> from nltk.sentiment import SentimentIntensityAnalyzer
>>> sia = SentimentIntensityAnalyzer()
>>> sia.polarity_scores("Wow, this tool is incredibly powerful!")
{'neg': 0.0, 'neu': 0.358, 'pos': 0.642, 'compound': 0.8012}
```

The `polarity_scores` function returns 3 values which correspond to the
percentage likelihood that the text is negative, neutral, or positive. The
`compound` score is a value between `1` (positive) and `-1` (negative). You can
use these scores to track/evaluate polarity of short texts. However, the
'vanilla' classifier can be made better with a bit of effort.

1. Make sure you have downloaded the NLTK `movie_reviews` corpus
(`nltk.corpus.movie_reviews`), as this will be the set of data that
you will use for training and testing the classifier. Each of the reviews in
this corpus has already been classified as positive or negative, which allows
us to see how well the NLTK sentiment analyzer works, i.e. with the following
code:

```python
import nltk
from nltk.sentiment import SentimentIntensityAnalyzer
from statistics import mean
from random import shuffle

sia = SentimentIntensityAnalyzer()

def is_positive(review_id: str) -> bool:
    """True if the average of all sentence compound scores is positive."""
    text = nltk.corpus.movie_reviews.raw(review_id)
    scores = [
        sia.polarity_scores(sentence)["compound"]
        for sentence in nltk.sent_tokenize(text)
    ]
    return mean(scores) > 0

positive_review_ids = nltk.corpus.movie_reviews.fileids(categories=["pos"])
negative_review_ids = nltk.corpus.movie_reviews.fileids(categories=["neg"])
all_review_ids = positive_review_ids + negative_review_ids

shuffle(all_review_ids)
correct = 0
for review_id in all_review_ids:
  if is_positive(review_id):
    if review_id in positive_review_ids:
      correct += 1
  else:
    if review_id in negative_review_ids:
      correct += 1

print(F"{correct / len(all_review_ids):.2%} correct")
```

```python
64.00% correct
```

2. Create a list of 'positive' words and 'negative' words based on ratings
of short texts. You can either use the same NLTK corpus of movie reviews or
another that you can find online. Once you have sorted and filtered the words,
perhaps via frequency distributions, write a function that uses these words in
conjunction with the NLTK sentiment analyzer to classify the movie reviews and
improve on the score. This process is known as feature selection/engineering -
try to think of and implement other "features" that you can identify in the
text which might improve your classification. Some ideas can be found [here](https://realpython.com/python-nltk-sentiment-analysis/).

3. Once you have determined the features that you want to extract from the
text, write a function that automatically extracts these features from the text
as a dictionary. Then use the function to create a list of tuples, where the
first item of the tuple is the dictionary of features and the second item is the
category ("pos" or "neg") of the review, i.e.:

```python
features = [
            (extract_features(nltk.corpus.movie_reviews.raw(review)), "pos")
            for review in nltk.corpus.movie_reviews.fileids(categories=["pos"])
            ]
features.extend([
            (extract_features(nltk.corpus.movie_reviews.raw(review)), "neg")
            for review in nltk.corpus.movie_reviews.fileids(categories=["neg"])
            ])
```

> Finally, split the dataset for training and validation to see how/whether your
features improve classification using, i.e. the Naive Bayes classification
algorithm in NLTK. It is important that whatever classifier you use, the
training data is kept separate from the testing/validation set, otherwise you
are simply letting the model "memorize" inputs (overfitting) and it will not
generalize well to other datasets. It is common in machine learning to use an
80/20 or 90/10 split with larger datasets, but for illustration and due to the
small size of the `movie_reviews` corpus we will train on a quarter of the
dataset and predict on the remainder of the dataset.

```python
>>> # Use 1/4 of the set for training
>>> train_count = len(features) // 4
>>> shuffle(features)
>>> classifier = nltk.NaiveBayesClassifier.train(features[:train_count])
>>> classifier.show_most_informative_features(10)
>>> nltk.classify.accuracy(classifier, features[train_count:])
```

4. This code is simply a starting point for exploration. What other
features can you think of and implement to improve accuracy? How does the
accuracy improve with different splits? Try to implement other classifiers and
see how they perform on this dataset. Are there other lexical resources/corpora
within NLTK or from other sources that can improve your results? What is the
best accuracy you can get?

5. With your group, write a roughly 5-page paper (no longer than 10 pages)
describing your goals, data, process, and results. This paper should include
relevant linguistic information and citations for your sources. Submit the
paper as a PDF along with your annotated/commented Python code in a Github
repository. The PDF should also be submitted via TurnItIn.
