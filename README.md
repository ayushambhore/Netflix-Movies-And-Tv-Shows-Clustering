# Netflix-Movies-And-Tv-Shows-Clustering
The project involves building a content-based recommender system for Netflix movies and TV shows using a dataset collected from Flixable, a third-party Netflix search engine. The dataset comprises 7787 rows and 12 columns, providing information about show IDs, types (TV show or movie), titles, directors, cast, country of production, date added to Netflix, release year, content rating, duration, genre, and brief descriptions.

The data exploration phase reveals that the 'director' column has the highest number of missing values, followed by the 'cast' column. To address this, we perform data preprocessing, including handling missing values, removing stopwords, punctuations, and non-ASCII characters, and lemmatizing the text. We also perform tokenization and vectorization to convert the text data into numerical vectors, making it suitable for machine learning models.

The model building process starts with dimensionality reduction using PCA to reduce the number of features to 3400 dimensions. The PCA-transformed data is then used to build two clustering models - KMeans and Agglomerative Clustering. For the KMeans model, we utilize the Elbow Method and Silhouette Score to find the optimal number of clusters. The KMeans clustering results in five clusters, each containing different proportions of movies and TV shows. The Agglomerative Clustering creates 11 clusters, providing insights into different content genres and patterns.

The content-based recommender system leverages the intrinsic features of the content, such as title, genre, description, and cast, to make personalized recommendations to users. It offers suggestions based on similarities between items, ensuring relevant and niche recommendations even for new users or items with limited information.

The project's focus on model building highlights the importance of data preprocessing, dimensionality reduction, and clustering algorithms in creating an effective content-based recommender system. By integrating external datasets like IMDB ratings or rotten tomatoes, we can enrich the recommendations with additional insights and enhance the system's performance further.

Overall, this project demonstrates how content-based recommender systems can provide valuable insights into content preferences and trends, guiding content creators and producers in generating captivating and well-suited content for viewers on streaming platforms like Netflix.




