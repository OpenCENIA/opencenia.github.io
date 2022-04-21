---
title: "WEFE: The Word Embeddings Fairness Evaluation Framework" 
summary: "WEFE: The Word Embeddings Fairness Evaluation Framework is an open source library for measuring and mitigating bias in word embedding models."
tags:
- deep learning
- word embeddings
- fairness
- bias
- evaluation
- software
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: https://wefe.readthedocs.io/en/latest/

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:

url_code: https://github.com/dccuchile/wefe
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

*Word Embedding Fairness Evaluation* (WEFE) is an open source library for 
measuring an mitigating bias in word embedding models. 
It generalizes many existing fairness metrics into a unified framework and 
provides a standard interface for:

- Encapsulating existing fairness metrics from previous work and designing
  new ones.
- Encapsulating the test words used by fairness metrics into standard
  objects called queries.
- Computing a fairness metric on a given pre-trained word embedding model 
  using user-given queries.

WEFE also standardizes the process of mitigating bias through an interface similar 
to the ``scikit-learn`` ``fit-transform``.
This standardization separates the mitigation process into two stages:

- The logic of calculating the transformation to be performed on the model (``fit``).
- The execution of the mitigation transformation on the model (``transform``).

Motivation and objectives
=========================

Word Embeddings models are a core component in almost all NLP downstream systems.
Several studies have shown that they are prone to inherit stereotypical social
biases from the corpus they were built on.
The common method for quantifying bias is to use a metric that calculates the
relationship between sets of word embeddings representing different social
groups and attributes.

Although previous studies have begun to measure bias in embeddings, they are
limited both in the types of bias measured (gender, ethnic) and in the models
tested. 
Moreover, each study proposes its own metric, which makes the relationship
between the results obtained unclear.

This fact led us to consider that we could use these metrics and studies to
make a case study in which we compare and rank the embedding models according
to their bias.

We originally proposed WEFE as a theoretical framework that formalizes the
main building blocks for measuring bias in word embedding models.
The purpose of developing this framework was to run a case study that consistently 
compares and ranks different embedding models.
Seeing the possibility that other research teams are facing the same problem, 
we decided to improve this code and publish it as a library, hoping that it 
can be useful for their studies.

We later realized that the library had the potential to cover more areas than just
bias measurement. This is why WEFE is constantly being improved, which so far has
resulted in a new bias mitigation module and multiple enhancements and fixes.

The main objectives we want to achieve with this library are:

- To provide a ready-to-use tool that allows the user to run bias tests in a 
  straightforward manner. 
- To provide a ready-to-use tool that allows the user to mitigate bias by means of a 
  simple `fit-transform` interface.
- To provide simple interface and utils to develop new metrics and mitigation methods.


Similar Packages
================

There are quite a few alternatives that complement WEFE. Be sure to check them out!

- Fair Embedding Engine: https://github.com/FEE-Fair-Embedding-Engine/FEE
- ResponsiblyAI: https://github.com/ResponsiblyAI/responsibly