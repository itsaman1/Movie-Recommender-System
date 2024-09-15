
# Movie Recommedation System

Designed and implemented a content-based movie recommender system using movie metadata from TMDB. Processed and engineered features from movie genres, keywords, cast, and crew to generate movie similarity scores.
Utilized data preprocessing techniques, including handling missing values and converting text data into numerical vectors using CountVectorizer. Calculated movie similarities using cosine similarity to facilitate accurate recommendations
Developed an interactive web application using Streamlit to provide movie recommendations. Integrated movie poster retrieval through the TMDB API and designed a user-friendly interface to display recommendations and posters based on user input.



## How to get API Key?

Create an account in https://www.themoviedb.org/, click on the `API` link from the left hand sidebar in your account settings and fill all the details to apply for API key. If you are asked for the website URL, just give "NA" if you don't have one. You will see the API key in your API sidebar once your request is approved.
## How to Run Project?

1. Clone or download this repository to your local machine.
2. Install all the libraries mentioned in the requirements.txt file with the command pip install -r requirements.txt
3. Get your API key from https://www.themoviedb.org/. (Refer the above section on how to get the API key)
4. Replace YOUR_API_KEY in files and hit save.
5. Open your terminal/command prompt from your project directory and run the file app.py by executing the command streamlit run app.py 

Hurray! That's it.
## Similarity Score?

How does it decide which item is most similar to the item user likes? Here come the similarity scores.

It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.


## How Cosine Similarity works?

Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.


![cosime](https://github.com/user-attachments/assets/bcd2c581-fe84-4adf-a38e-79032fcb7bd9)

More about Cosine Similarity : [Understanding the Math behind Cosine Similarity](https://www.datastax.com/guides/what-is-cosine-similarity)
## Sources of Dataset

1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)
2. [tmdb_5000_credits](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata?select=tmdb_5000_credits.csv)
3. [tmdb_5000_movies](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata?select=tmdb_5000_movies.csv)
