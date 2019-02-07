# InnoplexusHack_AV
Approach and code for the innoplexus hackathon held on analytics vidhya (15th position). This is the first ever hackathon I participated in and glad that I was in top 25.

## Problem Statement
The problem statement was to predict the list of other articles that will be referenced by an article. 

## Dataset
The train dataset contains information about the article, authors, title, abstract, full text, set, published date and the list of all other articles which were used by this article as reference. The test dataset also contains the same information except the reference list.
**Note:** The articles in both the datasets are distributed into disjoint sets and the articles can only reference other articles from the same set number.

## Challenge
As a newbie the main challenge I faced in this competition was to use this information and convert the problem into supervised learning format.

## Approach
The approach I used is very simple and basic. 
* Preprocessed the data by stemming and removing stop words to create a clean corpus.
* Computed the cosine similarities of the "Title" and "Abstract" columns of all the articles in each set.
* Intuition: an article can only reference articles which are published before in time.
* Combined the above computed title similarity and abstract similarity and output the top 5 articles filtered by the above intuition.

## Learnings
* Converting the problem into supervised learning format and training a model would've given better results.
* Hackthons are a great way to get to know how machine learning can be used to tackle the different kinds of problems prevailent in the industry. 

