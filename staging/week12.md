---
title: 'Week 12'
---

## Reading

### Ethics in NLP

Computational linguistics and natural language processing have, in the recent
decade or two, been quickly propelled from somewhat niche academic interest to
a huge industry with many consumer-facing products (e.g., Google Translate,
Siri, autocomplete, etc.) and other applied systems (stock market prediction,
risk assessment, hate speech detection, etc.). Unfortunately, the explosion
of popularity did not coincide with increased understanding of the ethical
questions particular to the field.

Please read the following short paper as a broad overview of the problems:

*   Dirk Hovy and Shannon L. Spruit. [The Social Impact of Natural Language Processing](https://www.aclweb.org/anthology/P16-2096.pdf). In the _Proceedings of the 54th Annual Meeting of the Association for Computational Linguistics_. 2016.

**Questions**

*   Why, in the authors’ view, has there been few discussions about ethics
in NLP, and what situation has changed to make such discussions more urgent?

*   Give examples of ethical problems for the following sources:
    *   _exclusion_
    *   _overgeneralization_
    *   _overexposure_ / _underexposure_
    *   _dual-use_

**Additional Reading**

*   There are many links to papers and course websites in the ACL wiki on [Ethics in NLP](https://aclweb.org/aclwiki/Ethics_in_NLP)

### Language Models

A “language model” is a model that gives a probability for a sequence of words
and/or predicts missing (e.g., next) words in a sequence. They are used for
judging the fluency of machine translation outputs and for text generation.
The traditional method of creating language models uses n-grams. For this,
read the following sections from Jurafsky and Martin’s _Speech and Natural Language Processing_:

*   [JM 3 – N-gram Language Models](http://web.stanford.edu/~jurafsky/slp3/3.pdf) Just the introduction and _3.1 – N-grams_.

In recent years, “neural language models”, in particular [transformer](https://en.wikipedia.org/wiki/Transformer_(machine_learning_model))\-based
models like [BERT](https://en.wikipedia.org/wiki/BERT_(language_model)) and
[GPT-3](https://en.wikipedia.org/wiki/GPT-3), have completely altered the
direction of academic research and industry applications of NLP. The quality of
their generated text is so good that it is often indistinguishable from
human-produced text, at least when the prompts or outputs are carefully
selected. Advocates of these models get mesmerized by the “magic” of their
[uninterpretable performance](https://en.wikipedia.org/wiki/BERT_(language_model)#Analysis)
and may claim that they “understand” or “comprehend” text. Critics point out
that they have only memorized and resynthesized linguistic form without any
other signals (e.g., vision, sound, joint attention and social context, etc.)
and cannot possibly have any true understanding of the world. The Bender and
Koller (2020) paper (see “additional reading”, below) does an in-depth look at
the claims of machine comprehension (and don’t miss the humorous example
outputs of GPT-2 in the appendix).

**Additional Reading**

*   Wikipedia article on [Language Model](https://en.wikipedia.org/wiki/Language_model)
(a bit dry, but it’s a decent survey)
*   Emily M. Bender and Alexander Koller. [Climbing towards NLU: On Meaning, Form, and Understanding in the Age of Data](https://www.aclweb.org/anthology/2020.acl-main.463.pdf). In the
_Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics_. 2020.

### Software

The following are some additional libraries for Python that you may find useful for NLP:

*   General-purpose, pretrained models:
    *   [https://spacy.io/](https://spacy.io/)
    *   [https://stanfordnlp.github.io/stanza/](https://stanfordnlp.github.io/stanza/)
*   Useful for data science or for designing machine-learning experiments:
    *   [https://allennlp.org/](https://allennlp.org/)
    *   [https://pandas.pydata.org/](https://pandas.pydata.org/)
    *   [https://scikit-learn.org/stable/](https://scikit-learn.org/stable/)
*   If you are taking/plan to take a course in HPSG:
    *   [https://github.com/delph-in/pydelphin](https://github.com/delph-in/pydelphin)

There are tons more. E.g., here’s an “Awesome” list of NLP software for Python
(and other languages): [https://github.com/keon/awesome-nlp#user-content-python](https://github.com/keon/awesome-nlp#user-content-python)
