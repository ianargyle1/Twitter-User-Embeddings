# Twitter User Embeddings

I completed this project with Bryce Gillespie and Janaan Lake. For the project, we attempted to replicate and extend the techniques presented by ["user2Vec: Social Media User Representation Based on Distributed Document Embeddings" (Hallac et al. 2019)](https://ieeexplore.ieee.org/document/8875952).

Specifically, this paper proposes vectorizing/embedding a twitter account by averaging the doc2vec embeddings of it's tweets. We think this does a poor job of creating a useful embedding due to the fact that accounts that tweet about multiple subjects tend to have clusterable doc2vec tweet embeddings. So, if an account tweets about, for example, politics and economics, the user embedding would fall somewhere in between the tweet clusters of embeddings and economics. However, if we want this account to be similar to another account that only tweets about economics, than we need to compare these accounts based on their tweet clusters. This is what we attempt to do in this project.

More information can be found in the paper, twitter_embedding.pdf. The cooresponding notebook is in twitter_embedding.ipynb.
