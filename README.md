# Topic-Modelling-NLP
This repo marks my attempt to learn and consequently practice the implementation of Topic modelling using algos like LDA, LSA and NMF

# Abstract 🚀
Well, put in a 🥜: Topic modeling is like a magic tool that helps computers understand what a bunch of texts or articles are all about. Imagine you have a big box of letters, and you want to sort them into different categories based on their content. That's what topic modeling does with the texts. It reads through all the documents, finds the main themes, or "topics," and groups similar ones together. So basically, if I have a large source of news articles, and I aim at grouping them to see for only those that revolved around some political stresses, topic modelling would help me narrow down my choices.

Getting into details 📑:
Topic modeling is a statistical and machine learning technique used in natural language processing to discover hidden thematic structures, known as "topics," within a collection of documents. The main goal of topic modeling is to automatically identify the underlying themes or subjects that frequently appear across the documents in the dataset.

The typical input for topic modeling is a set of textual documents, such as articles, reviews, or social media posts. The output is a set of topics, each represented as a probability distribution over words. Each document is assumed to be a mixture of these topics, where the proportions of each topic in the document indicate the relevance of that topic to the document.

![image](https://github.com/UdayG01/Topic-Modelling-NLP/assets/67233899/9774f6c0-dbb9-4706-9b60-ca5fa78aac51)


# 🤔Now why would I use it?
That's what occured to me first, but actually, as the corpuses get larger and larger (which indeed they are getting, given the amount of data users produce each day), techniques like what we are discussing become essential for more fruitful and efficient analysis.
* Information Retrieval: It can help organize and index large document collections, making it easier to retrieve relevant documents based on topics of interest.
* Content Analysis: Researchers and businesses can use topic modeling to gain insights into the main themes present in a corpus of text.
* Recommendation Systems: Topic modeling can be used to recommend relevant content to users based on their interests and preferences.
* Text Summarization: It aids in generating summaries of lengthy documents by identifying the most important topics.
* Market Research: Businesses can use topic modeling to analyze customer feedback, reviews, and social media data to understand customer preferences and opinions.

# 🧮💻
* Well, you may find a ton of algos supporting the purpose, but I went ahead with three, namingly LDA(Latent Dirichlet Analysis), LSA(Latent Semantic Analysis) and NMF (Non-Negative Matrix Factorization).
* Latent Dirichlet Allocation (LDA):
LDA is based on the principles of probabilistic modeling and Bayesian statistics. The model employs the Dirichlet distribution, a multivariate probability distribution defined on the simplex (a multi-dimensional geometric figure that lies between the coordinate axes). In LDA, the Dirichlet distribution is used to model the topic distributions within documents and word distributions within topics. The central idea is to estimate the optimal topic-word assignments by maximizing the likelihood of generating the observed documents

![image](https://github.com/UdayG01/Topic-Modelling-NLP/assets/67233899/28f224ad-f107-4663-b9d0-abd5cd93f3a5)

* Latent Semantic Analysis (LSA):
LSA is primarily grounded in linear algebra and matrix factorization. It leverages the concept of singular value decomposition (SVD) to reduce the dimensionality of the term-document matrix. SVD is a powerful linear algebra technique that decomposes a matrix into three matrices (U, Σ, and V^T), where U and V^T represent orthogonal matrices, and Σ is a diagonal matrix containing singular values. By truncating the singular values and corresponding matrices, LSA effectively identifies the most important latent semantic structures in the data

![image](https://github.com/UdayG01/Topic-Modelling-NLP/assets/67233899/44aa414f-795d-43a3-a62b-b05e94dd605e)


* Non-negative Matrix Factorization (NMF):
NMF is also rooted in linear algebra and matrix factorization. Unlike traditional matrix factorization methods like SVD, NMF restricts all elements of the factorized matrices to be non-negative. This property makes NMF suitable for data that exhibits additive, non-negative relationships, such as term frequencies in text data. The factorization aims to find non-negative basis vectors and non-negative coefficients that, when multiplied together, approximate the original data matrix

![image](https://github.com/UdayG01/Topic-Modelling-NLP/assets/67233899/e425fc21-07b9-486e-8fe5-ec64faa9d110)

![image](https://github.com/UdayG01/Topic-Modelling-NLP/assets/67233899/ee27feee-b85f-4e3a-9f76-785705966f59)



# References 🤓
These are some sources that I used for understanding the math, the intuition and implementation for topic modelling. These will help you dive deeper into these algorithms - help you get their math, code and preprocessing strategies like 'tokenization', 'lemmatizing', 'stemming', 'omitting stopwords' etc. 
* Topic Modeling and Latent Dirichlet Allocation (LDA) in Python | by Susan Li | Towards Data Science
https://towardsdatascience.com/topic-modeling-and-latent-dirichlet-allocation-in-python-9bf156893c24
* Latent Semantic Analysis: intuition, math, implementation | by Ioana | Towards Data Science
https://towardsdatascience.com/latent-semantic-analysis-intuition-math-implementation-a194aff870f8
* Topic Modelling Using NMF. Well, In this blog I want to explain… | by Vijay Choubey | Voice Tech Podcast | Medium
https://medium.com/voice-tech-podcast/topic-modelling-using-nmf-2f510d962b6e
* Frontiers | A Topic Modeling Comparison Between LDA, NMF, Top2Vec, and BERTopic to Demystify Twitter Posts
https://www.frontiersin.org/articles/10.3389/fsoc.2022.886498/full



