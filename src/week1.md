---
title: 'Week 1'
---

## Introduction

* Introduction to HG2051 ([slides](static/Wk01_slides.pdf))

## Environment Setup

* See [Configuring a Development Environment](environment-setup.html)

## Git Basics

### Overview

* [Intro to Git and GitHub](https://www.lib.uidaho.edu/media/workshops/UIdaho_git_workshop.pdf)

  (Thanks to Evan Peter Williamson of the University of Idaho)

### Commands

#### Just once

* `git clone`

#### For each changeset

1. `git add`
2. `git commit`
3. `git push`

## Introduction to GitHub

* <https://github.com/>
* Basic Concept: hosting for remote repositories (plus much more)
* Navigating the UI
* Cloning a repository

## Running Python

* Different ways of running Python
  - REPL (e.g., IDLE)
  - Script
  - Notebook (https://jupyter.org/)
* Getting results from Python

## If time allows..
[Introduction to the Natural Language Tool Kit](static/preface_NLTK.pdf)

In-class setup of NLTK:

- `$ pip install nltk` (Windows/Mac/Linux)
- `$ python`

 ```{.python .terminal}
 >>> import nltk
 >>> nltk.download()
 >>> from nltk.book import *
 ```

 - [Searching Text](https://www.nltk.org/book/ch01.html#searching-text)
 Choose an English word, and see how it is used in the different example texts by making concordances. Try other words. Find a word that is used frequently in one text and never used in the other texts.
 - Generating Text
 Generate paragraphs in the style of each different example text, using generate(). An example is shown in Searching Text.
 - [Spoken Dialog Systems](https://www.nltk.org/book/ch01.html#spoken-dialog-systems)
 [The Turing Test](http://en.wikipedia.org/wiki/Turing_test). Have a conversation with at least two different NLTK chatbots. Do any of these chatbots pass the test?

 - NLTK demos (optional)

 In VS Code (Python), run this NLTK application:

 ```{.python .terminal}
 >>> nltk.app.rdparser()
 ```

 Keep clicking Step for a while and try to see what's going on. Alternatively, click Autostep once and just watch.
 *Challenge:* can you parse the whole sentence successfully using only the Expand, Match and Backtrack buttons?

 In VS Code (Python), run this NLTK application:

 ```{.python .terminal}
 >>> nltk.app.srparser()
 ```
 Keep clicking Step for a while and try to see what's going on.
 *Challenge:* can you parse the whole sentence successfully using only the Shift and Reduce buttons?

## Homework 1

See invite for GitHub on NTULearn.

## Readings for next week:

- NLTK Chapter 1: [Language Processing and Python](https://www.nltk.org/book/ch01.html)
- NLTK Chapter 1.1: [Computing with Language: Texts and Words](https://www.nltk.org/book/ch01.html#sec-computing-with-language-texts-and-words)
- NLTK Chapter 1.2: [A Closer Look at Python: Texts as Lists of Words](https://www.nltk.org/book/ch01.html#sec-a-closer-look-at-python-texts-as-lists-of-words)
- NLTK Chapter 1.3: [Computing with Language: Simple Statistics](https://www.nltk.org/book/ch01.html#sec-computing-with-language-simple-statistics)
- NLTK Chapter 1.5: [Automatic Natural Language Understanding](https://www.nltk.org/book/ch01.html#sec-automatic-natural-language-understanding)

[vscode]: https://code.visualstudio.com/
[git]: https://git-scm.com/
[python]: https://www.python.org/
[GitHub]: https://github.com/
