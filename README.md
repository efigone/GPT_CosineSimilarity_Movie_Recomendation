# GPT_CosineSimilarity_Movie_Recomendation
Movie Recomendations from IMDB's top 1000 movies using GPT for Embedding and Scikit-Learn for Cosine Similarity.
Data: https://www.kaggle.com/datasets/harshitshankhdhar/imdb-dataset-of-top-1000-movies-and-tv-shows/data

The dataset was downloaded as is from Kaggle. Use the Data_Cleaning notebook to preprocess the data. We strip away whitespace, remove duplicates and null values. We then reformat the data to make one column that is a combination of all the text columns formatted for input into OpenAI's small embedding model.

Set an environmental variable with your own OPENAI API key (you will need credits on your account) and run the Movie_Recomendation notebook to first get the required embeddings and then we use cosine similarity to recommend a movie! The recommendations are limited to the dataset of IMDB's top 100 movies but work pretty well! 
