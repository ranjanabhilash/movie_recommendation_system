# movie_recommendation_system
data link : https://www.kaggle.com/code/rounakbanik/movie-recommender-systems/input


About Dataset
Context
These files contain metadata for all 45,000 movies listed in the Full MovieLens Dataset. The dataset consists of
movies released on or before July 2017. Data points include cast, crew, plot keywords, budget, revenue, posters,
release dates, languages, production companies, countries, TMDB vote counts and vote averages.
This dataset also has files containing 26 million ratings from 270,000 users for all 45,000 movies. Ratings are on a
scale of 1-5 and have been obtained from the official GroupLens website.

Content
This dataset consists of the following files:

movies_metadata.csv: The main Movies Metadata file. Contains information on 45,000 movies featured in the Full
MovieLens dataset. Features include posters, backdrops, budget, revenue, release dates, languages, production
countries and companies.

keywords.csv: Contains the movie plot keywords for our MovieLens movies. Available in the form of a stringified
JSON Object.

credits.csv: Consists of Cast and Crew Information for all our movies. Available in the form of a stringified JSON
Object.

links.csv: The file that contains the TMDB and IMDB IDs of all the movies featured in the Full MovieLens dataset.

links_small.csv: Contains the TMDB and IMDB IDs of a small subset of 9,000 movies of the Full Dataset.

ratings_small.csv: The subset of 100,000 ratings from 700 users on 9,000 movies.

The Full MovieLens Dataset consisting of 26 million ratings and 750,000 tag applications from 270,000 users on all
the 45,000 movies in this dataset can be accessed here


Acknowledgements
This dataset is an ensemble of data collected from TMDB and GroupLens.
The Movie Details, Credits and Keywords have been collected from the TMDB Open API. This product uses the
TMDb API but is not endorsed or certified by TMDb. Their API also provides access to data on many additional
movies, actors and actresses, crew members, and TV shows. You can try it for yourself here


Simple Recommender¶
The Simple Recommender offers generalized recommnendations to every user based on movie popularity
and (sometimes) genre. The basic idea behind this recommender is that movies that are more popular and
more critically acclaimed will have a higher probability of being liked by the average audience. This model
does not give personalized recommendations based on the user.
The implementation of this model is extremely trivial. All we have to do is sort our movies based on ratings
and popularity and display the top movies of our list. As an added step, we can pass in a genre argument to
get the top movies of a particular genre.




