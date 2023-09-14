---
title: Language and the Computer (AY2023)
instructor:
  - name: Hiram Ring
    email: hiram.ring@ntu.edu.sg
date: "Fridays, 12:30-3:20pm (Sem1)"
location: >
  [TR+29](https://maps.ntu.edu.sg/#/ntu/d386ffa80e4e46f286d17f08/poi/details/e97bc9bf4c6740ca8f3d35cc) (LHS-B2-06, The Hive)

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
    date: 18 Aug
    topic: What is Computational Linguistics? Why do it? Why use Python? CS basics
    url: week1.html
    notes: "[Setup](environment-setup.html), [VS_Code](using-vscode.html)"

  - week: 2
    date: 25 Aug
    topic: Basic Types and Data Structures; Using Python to Count Things; Lists
    url: week2.html
    notes: "[PyT 3.1](https://docs.python.org/3/tutorial/introduction.html#using-python-as-a-calculator); [NLTK 1](https://www.nltk.org/book/ch01.html)"

  - week: --
    date: 01 Sep
    topic: Polling Day, no class
    cancelled: true

  - week: 3
    date: 08 Sep
    topic: Assignment, Expressions, and Control; Strings (abbreviated class due to Student Union Day)
    url: week3.html
    notes: "[PyT 3.2](https://docs.python.org/3/tutorial/introduction.html#first-steps-towards-programming), [4](https://docs.python.org/3/tutorial/controlflow.html); [NLTK 4.1](http://www.nltk.org/book/ch02.html#wordlist-corpora)"

  - week: 4
    date: 15 Sep
    topic: Text Corpora and Conditional Frequencies
    url: week4.html
    notes: "[DIP 2.2](https://diveintopython3.problemsolving.io/native-datatypes.html#booleans),
    [2.8](https://diveintopython3.problemsolving.io/native-datatypes.html#none); [PT 5.3](https://docs.python.org/3/tutorial/datastructures.html#tuples-and-sequences),
    [5.5](https://docs.python.org/3/tutorial/datastructures.html#dictionaries), [4.7.1](https://docs.python.org/3/tutorial/controlflow.html#default-argument-values)-[2](https://docs.python.org/3/tutorial/controlflow.html#keyword-arguments); [NLTK 2.1](http://www.nltk.org/book/ch02.html#accessing-text-corpora)-[2](http://www.nltk.org/book/ch02.html#conditional-frequency-distributions)"

  - week: 5
    date: 22 Sep
    topic: Lexical Resources and WordNet
    # url: week5.html
    # notes: "[NLTK 2.4](http://www.nltk.org/book/ch02.html#lexical-resources), [2.5](http://www.nltk.org/book/ch02.html#wordnet), ([How To](http://www.nltk.org/howto/wordnet.html))"
    # notes: "[notebook](static/week5-practice.ipynb)"

  - week: 6
    date: 29 Sep
    topic: Processing Raw Text
    # url: week6.html
    # notes: "[notebook](static/week6-practice.ipynb)"

  - week: --
    date: 06 Oct
    topic: Recess
    cancelled: true

  - week: 7
    date: 13 Oct
    topic: Mid-review; Working with Software Projects
    notes: "Coding challenge"
    #[Midterm Quiz](static/quiz1_modelsolution.py)"
    # url: week7.html

  - week: 8
    date: 20 Oct
    topic: Regular Expressions and Algorithmic Thinking
    # url: week8.html

  - week: 9
    date: 27 Oct
    topic: N-Grams and Collocations
    # url: week9.html

  - week: 10
    date: 03 Nov
    topic: Part-of-speech Tagging
    # url: week10.html
    # notes:

  - week: 11
    date: 10 Nov
    topic: Classification
    # url: week11.html
    notes: "Project 1 due"
    # notes: "[Project 1](project1.html) due"

  - week: 12
    date: 17 Nov
    topic: Ethics, Language Models, and Software Libraries
    # url: week12.html

  - week: 13
    date: 24 Nov
    topic: Review and Final Quiz
    # url: final-review.html
    notes: "Coding challenge"

  - week: 14
    date: 01 Dec
    topic: Extras
    # url: week14.html
    notes: "Project 2 due"
    # notes: "[Project 2](project2.html) due"
---

## Course Pages

- [Environment Setup](environment-setup.html) -- instructions for setting up your computer for HG2051
- [Using Visual Studio Code](using-vscode.html) -- how to get, complete, and submit assignments
- [Glossary](glossary.html) -- definitions of some technical terms
- [Midterm Review](midterm-review.html)
- [Final Review](final-review.html)

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
  - Learn Python the Hard Way (beginner's guide) -- <https://learnpythonthehardway.org/book/>
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
previous years. Below are some of the archives of the previous courses:

- Hiram Ring:
  [2022](https://hg2051-ntu.github.io/AY2022/)
- Michael Wayne Goodman:
  [2019](https://compling.hss.ntu.edu.sg/courses/hg2051/),
  [2020](https://ntu-hg2051.github.io/)
- Francis Bond:
  2010,
  2011,
  2012,
  2013,
  2015,
  [2017](http://compling.hss.ntu.edu.sg/courses/hg2051.2017/)
