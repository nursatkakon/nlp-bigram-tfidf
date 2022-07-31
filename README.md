
# Language Modeling with bigram & TF-IDF
<br>
<br>
<div class="alert alert-block alert-warning">

Natural Language Processing (NLP) is a subfield of artificial intelligence that deals understanding & processing human language. Language models are one of the most important parts of Natural Language Processing. 
</div>
<br>
<br>
<div class="alert alert-block alert-warning"> 

There are primarily two types of language models:
* **Statistical Language Models** - These models use traditional statistical techniques like n-grams, Hidden Markov Models (HMM) and certain linguistic rules to learn the probability distribution of words.
* **Neural Language Models** - These models surpass statistical language models in their effectiveness. They use different kinds of neural networks to model language.
</div>
<br>
<br>
<div class="alert alert-block alert-warning">

Both 'TF-IDF' and 'n-grams' are used to prepare text documents for searching. They provide different indexing rules to find matching documents. In this shot, we will work on `bigram model` & `TF-IDF` implementation.
</div>
<br>
<br>

## What is Bigram Model?
<div class="alert alert-block alert-warning"> 

In the `bigram model`, we find bigrams, which are two words coming together in the corpus (the entire collection of words/sentences). We use a `bigram model` to predict the conditional probability of the next word. To estimate bigram probabilities, we can use the following equation:

  $$ P(W_n| W_{n-1}) = \frac {count(W_{n-1}, W_n)} {count(W_{n-1})} $$
  
</div>
<br>
<br>

## What is TF-IDF? 

<div class="alert alert-block alert-warning"> 

`TF-IDF` is useful in many natural language processing applications. For example, Search Engines use `TF-IDF` to rank the relevance of a corpus for a query. `TF-IDF` is also employed in text classification, text summarization, and topic modeling.
</div>
<br>
<br>

### Term Frequency (TF)

<div class="alert alert-block alert-warning">
TF measures how frequently a term occurs in a corpus. Since every corpus is different in length, it is possible that a term would appear much more times in long corpuss than shorter ones. Thus, the term frequency is often divided by the corpus length (aka. the total number of terms in the corpus) as a way of normalization: 

  $$ tf_{(i,j)} = \frac {n_{(i,j)}} {\sum_k n_{(i,j)}} $$
  
Every corpus has its own term frequency.   
</div>
<br>
<br>

### Inverse corpus Frequency (IDF)

<div class="alert alert-block alert-warning"> 
IDF measures how important a term is. While computing TF, all terms are considered equally important. The log of the number of corpuss divided by the number of corpuss that contain the word w. Inverse data frequenct determines the weight of rare words across all corpuss in the corpus. 

  $$ idf(w) = log (\frac{N}{df_t}) $$ 
  
</div>




