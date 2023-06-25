# SemanticSearchExperimentation
Experimentation on Semantic Search implementation from basic models to much more advanced LLM embeddings based approaches.

Implementing a semantic search module for a dataset of computer science research papers utilizing TF-IDF, Bi-encoders, Cross-encoders and FAISS.

## TF-IDF
* Used TF-IDF vectors and cosine similarity metric to perform search on abstract of research papers.

## Sentence Transformers
* Pre-trained a Bert-Base-Uncased model using TSDAE task for a domain model to perform semantic search.
* Used Sentence-Transformers all-MiniLM-L6-v2 model for performing semantic search using cosine similarity metric.
* Used Sentnece-Transformer re-ranking pipeline with a Bi-encoder to get a subset of relevant results and then further filtered them out for more accurate results with a Cross-encoder model.
* FAISS in-memory index for demonstrating speeding up of search in case of large corpus of text data. In the current case, as the corpus was within a milion, there were minor gains. But in case of larger text corpus, with Approximate search enabled through clustering, FAISS can help with much more faster searches.


