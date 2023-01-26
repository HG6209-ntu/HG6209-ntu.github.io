---
title: Language and the Computer (AY22-23)
instructor:
  - name: Hiram Ring
    email: hiram.ring@ntu.edu.sg
date: "Thursdays, 12:30-15:20"
location: >
  [TR+65](https://maps.ntu.edu.sg/#/ntu/d386ffa80e4e46f286d17f08/poi/details/5b919a593c90401d8723f308) (SS1-B1-03, South Spine)

abstract: >
  Traditionally linguistic analysis was done largely by hand, but
  computer-based methods and tools are becoming increasingly widely
  used in contemporary research. This course provides an introduction
  to skills and resources that can assist the linguist in performing
  fast, flexible, and accurate quantitative analyses. Students will
  learn a programming language (Python) along with techniques for
  processing human language data. No previous programming experience
  is required: we will teach you the basics of programming and
  computational linguistics along with some good software engineering
  practices.

schedule:
  - week: 1
    date: 12 Jan
    topic: What is Computational Linguistics? Why do it? Why use Python?
    url: week1.html

  - week: 2
    date: 19 Jan
    topic: Basic Types and Data Structures; Using Python to Count Things; Lists
    url: week2.html
    notes: "[PyT 3.1](https://docs.python.org/3/tutorial/introduction.html#using-python-as-a-calculator); [NLTK 1](https://www.nltk.org/book/ch01.html)"

  - week: 3
    date: 26 Jan
    topic: Assignment, Expressions, and Control; Strings
    url: week3.html
    notes: "[PyT 3.2](https://docs.python.org/3/tutorial/introduction.html#first-steps-towards-programming), [4](https://docs.python.org/3/tutorial/controlflow.html); [NLTK 4.1](http://www.nltk.org/book/ch02.html#wordlist-corpora)"

  - week: 4
    date: 02 Feb
    topic: Text Corpora and Conditional Frequencies
    url: week4.html
    notes: "[DIP 2.2](https://diveintopython3.problemsolving.io/native-datatypes.html#booleans),
    [2.8](https://diveintopython3.problemsolving.io/native-datatypes.html#none); [PyT 5.3](https://docs.python.org/3/tutorial/datastructures.html#tuples-and-sequences),
    [5.5](https://docs.python.org/3/tutorial/datastructures.html#dictionaries); [NLTK 2.1](http://www.nltk.org/book/ch02.html#accessing-text-corpora), [2.2](http://www.nltk.org/book/ch02.html#conditional-frequency-distributions)"
    # notes: "[notebook](static/week4-practice.ipynb)"

  - week: 5
    date: 09 Feb
    topic: Lexical Resources and WordNet
    # url: week5.html
    notes: "[NLTK 2.4](http://www.nltk.org/book/ch02.html#lexical-resources), [2.5](http://www.nltk.org/book/ch02.html#wordnet),
    ([How To](http://www.nltk.org/howto/wordnet.html))"
    # notes: "[notebook](static/week5-practice.ipynb)"

  - week: 6
    date: 16 Feb
    topic: Processing Raw Text
    # url: week6.html

  - week: 7
    date: 23 Feb
    topic: Mid-review; Working with Software Projects
    # url: week7.html

  - week: --
    date: 02 Mar
    topic: Recess
    cancelled: true

  - week: 8
    date: 09 Mar
    topic: Regular Expressions
    # url: week8.html
    notes: Project 1 due

  - week: 9
    date: 16 Mar
    topic: N-Grams and Collocations
    # url: week9.html

  - week: 10
    date: 23 Mar
    topic: Part-of-speech Tagging
    # url: week10.html

  - week: 11
    date: 30 Mar
    topic: Classification
    # url: week11.html

  - week: 12
    date: 06 Apr
    topic: Exploring Software Libraries
    # url: week12.html

  - week: 13
    date: 13 Apr
    topic: Review
    # url: week13.html
    notes: Project 2 due
---

## Course Pages

- [Environment Setup](environment-setup.html) -- instructions for setting up your computer for HG2051
- [Using Visual Studio Code](using-vscode.html) -- how to get, complete, and submit assignments
- [Glossary](glossary.html) -- definitions of some technical terms

## Grading Criteria

This course is graded with continuous assessment as follows:

- Homework (autograded)
- Project 1 -- 30%
- Project 2 -- 30%
- Mid-term Quiz -- 15%
- Final Quiz -- 15%
- Participation -- 10%

You may also get 1--5% extra credit (not exceeding 100% in the course)
by submitting a contribution (e.g., code or documentation) to an
open-source project. Contact me for details.

## Resources

- Python -- <https://www.python.org/>
  - The Python Tutorial (official docs) -- <https://docs.python.org/3/tutorial/>
  - The Python Standard Library (official docs) -- <https://docs.python.org/3/library/index.html>
  - Learn Python in 10 Minutes (quick guide) -- <https://www.stavros.io/tutorials/python/>
  - Dive Into Python 3 (free ebook) -- <https://diveintopython3.problemsolving.io/>
- Git -- <https://git-scm.com/>
  - Official documentation (manuals, cheat sheets, videos) -- <https://git-scm.com/doc>
- GitHub -- <https://github.com/>
  - GitHub Guides -- <https://guides.github.com/>
- Visual Studio Code -- <https://code.visualstudio.com/>
  - Documentation -- <https://code.visualstudio.com/docs>
  - Using Python in VS Code -- <https://code.visualstudio.com/docs/python/python-tutorial>
  - Working with Jupyter Notebooks in Visual Studio Code -- <https://code.visualstudio.com/docs/python/jupyter-support>
- NLTK -- <http://www.nltk.org/>
  - Natural Language Processing with Python (free ebook) -- <http://www.nltk.org/book/>
- StackOverflow (popular programming Q&A site)-- <https://stackoverflow.com/>

## Acknowledgments

The majority of the content for this course has been borrowed (with
permission) from Michael Wayne Goodman and Francis Bond, who taught
previous years:

- Michael Wayne Goodman:
  [2019](http://compling.hss.ntu.edu.sg/courses/hg2051/),
  [2020](https://ntu-hg2051.github.io/)
- Francis Bond:
  2010,
  2011,
  2012,
  2013,
  2015,
  [2017](http://compling.hss.ntu.edu.sg/courses/hg2051.2017/)
