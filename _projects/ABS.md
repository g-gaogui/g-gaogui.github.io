---
layout: page
title: Aspect-Based Sentiment Analysis with Enhanced Graph Convolutional Networks
description: An enhanced GCN architecture that integrates affective knowledge and aspect-oriented dependency structure for fine-grained sentiment classification.
importance: 2
img: assets/img/ABS.jpg
category: academic
related_publications: false
---

<h2>Overview</h2>

<p>
Aspect-based sentiment analysis (ABSA) seeks to identify sentiment polarity
toward specific aspects mentioned within a sentence, rather than assigning a
single sentiment label to the text as a whole. This project builds on graph
convolutional network (GCN) approaches that exploit syntactic dependency
structure to model relationships between aspect words and their surrounding
context. We propose an enhanced adjacency matrix that combines an
aspect-oriented, undirected dependency tree with affective knowledge from
SenticNet, and we study how architectural choices such as activation
function, positional weighting, and weight initialization affect downstream
classification accuracy.
</p>

<hr>

<h2>Project Information</h2>

<ul>
  <li><strong>Type:</strong> Course Research Project</li>
  <li><strong>Institution:</strong> National University of Singapore</li>
</ul>

<hr>

<h2>Keywords</h2>

<p>
Aspect-Based Sentiment Analysis · Graph Convolutional Networks · Dependency
Parsing · SenticNet · Affective Computing · Natural Language Processing
</p>

<hr>

<h2>Abstract</h2>

<p>
Aspect-based sentiment analysis extracts sentiment polarity at a fine-grained
level by focusing on individual aspects within a sentence. Traditional
approaches rely on recurrent and convolutional neural networks to capture
contextual dependencies, while more recent methods build graph-based models
over dependency trees to learn relationships between contextual and aspect
words. This project proposes an improved graph convolutional network built on
an enhanced adjacency matrix that jointly leverages affective information and
dependency relations between contextual and aspect words. We reshape the
standard dependency tree into an undirected, aspect-oriented structure that
preserves original word connections while adding direct links between aspect
words and the rest of the sentence. We further revise the aspect-affective
matrix formulation so that SenticNet scores and aspect indicators combine in
a way that better reflects their underlying relationship, rather than simply
summing the two signals. The resulting model is evaluated against choices of
activation function, positional awareness function, and weight initializer,
and a case study on attention distributions highlights both the strengths
and the remaining limitations of the approach in disentangling sentiment
contributions across conflicting aspects within a single sentence.
</p>

<hr>

<h2>Key Contributions</h2>

<ul>
  <li>Proposed an undirected, aspect-oriented dependency tree construction that connects aspect words directly to all contextual words while preserving the original dependency structure.</li>

  <li>Designed an enhanced adjacency matrix that combines syntactic dependency, aspect indicators, and SenticNet affective scores in a unified weighted formulation.</li>

  <li>Reformulated the positional awareness function to exclude the aspect word itself from its own context weighting, addressing an association bias in prior implementations.</li>

  <li>Conducted systematic comparisons of activation functions, positional weighting functions, and weight initialization schemes for the GCN architecture.</li>

  <li>Performed a case study analyzing attention distributions across contradictory aspects within the same sentence to surface remaining model vulnerabilities.</li>
</ul>

<hr>

<h2>Technologies</h2>

<p>
Graph Convolutional Networks · GloVe Embeddings · spaCy · Biaffine Dependency Parsing · SenticNet · PyTorch
</p>
