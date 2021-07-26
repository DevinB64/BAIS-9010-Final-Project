# BAIS-9010-Final-Project


BAIS:9010 – Contemporary Topics in Analytics: Applied Deep Learning

Jeffrey Hendricks

Individual Deep Learning Project Check-in

Devin Becktell

# Project Goal: #

The goal of my deep learning project will be to utilize Natural Language Processing in order to parse
through Amazon reviews and determine the star rating that each review would receive. A rating of 1-to5 can be given for a product.

# Data: #

The data for this project will encompass 497,577 amazon reviews on various video game products. The
source of this data will come from Jianmo Ni from the University of California San Diego:


(https://nijianmo.github.io/amazon/index.html)
Justifying recommendations using distantly-labeled reviews and fined-grained aspects
Jianmo Ni, Jiacheng Li, Julian McAuley
Empirical Methods in Natural Language Processing (EMNLP), 2019
pdf

Initially, I attempted to gather Amazon reviews data from Amazon itself using AWS
(https://s3.amazonaws.com/amazon-reviews-pds/readme.html). I created my own bucket, and
collected the data onto my local computer for analysis in my git repo using VSC. This method ended up
failed, as each time I went to unpack the gzipped tsv file, both VSC and Jupyter would become
unresponsive and restart my kernel. With this in mind, I have decided to load a subset of the data.

# Approach: #

For this project, the preprocessing of data will take a standard approach. I will begin by analyzing the
data for any potential concatenation of text columns, and dropping of columns that either may not
provide value to my analysis, or will leak information into the model. This will be followed with
stopword analysis, tokenization, lemmatization, and stemming where appropriate. I will plan to utilize
transfer learning using ELMo or a similar embedding representations. I will then build out my final
model. The analysis will be done majorly within Tensorflow with the potential for experimentation with
other libraries.
