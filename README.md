# Movie-recommender-system
 
# Movie Recommender System using Machine learning

This project is based on a recommender system in Machine Learning.
I have taken two data sets from Kaggle to get information about the movie data I would need for building a recommender system that would suggest suggestions similar to the movie we would enter.

I took a dataset from the site TMBD,
It is a data set of about 5000 movies.
Among the two dataset one contains about movie_id,title,genres,keywords,overview,....and others

The other one contains columns about the title, cast(people who acted in the movie), crew(people involved in making the movie i.e behind the camera),.....and other columns

We would consider in our project the columns mentioned earlier 

i.e movie_id, title, genres, keywords, overview, cast, crew

we would first read both data using -->pandas library

Then we would merge both data sets on a similar column between them which is the title

We would consider among all our required columns they are
movie_id, title, genres, keywords, overview, cast, crew

We would then boil down the genres, keyword, overview, cast, crew 
i.e merge all these columns by converting them into the same format and name that one column as tags

On these tags, we would then perform stemming by using a natural language toolkit

Until here -->1.PREPROCESSING of the data is done 

Now for -->2.PREPARING the  model, we would do

we would perform text vectorization which would convert our text into vectors

Each vector represents a movie

The similarity of the movie is determined by other vectors that are closer to that particular selected movie

Now on these vectors, we would use cosine similarity to calculate the angle between two vectors 

PS We are calculating the angle between two vectors instead of the regular Euclidean distance since our data which has about 5,000 movies is of higher dimensionality
![cosine](https://github.com/Shravya1-0/Movie_recommender_system/assets/121577600/84232d9c-25b1-4688-884e-046d2c1cdddc)




The lesser the angle between two movie vectors the more similar the two movies are


## Acknowledgements
 
 -  https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata

 - https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.CountVectorizer.html
 - https://www.youtube.com/@campusx-official
 - https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.cosine_similarity.html


## Demo


https://drive.google.com/file/d/16veWmd08paLtCPuvF88Iorx751iPeWLf/view?usp=sharing
## 🔗 Links

![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)www.linkedin.com/in/ke-shravya


