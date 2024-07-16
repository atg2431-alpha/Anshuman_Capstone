This model is basically fine-tuning a pre-trained llm named 'Distill-Bert' in hugging face using a Question answer dataset, i found online named 'Amazon Dataset'.
I have preprocessed the original csv file which i provided in the repo.
As already said, this is a question answer type model, i have converted the queries and responses into embeddings using tokenizer provided by the model itself.
I stored the embeddings into Vector Database using Faiss, it can accessed through queries.index and responses.index.
Then I trained the model using the context from both embeddings of queries and answers.

