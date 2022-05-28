# Movie Recommender System
## About the project
Recommender System is a system that seeks to predict or filter preferences according to the user's choices. Recommender systems are utilized in a variety of areas including movies, music, news, books, research articles, search queries, social tags, and products in general.
                        
This movie recommender system will recommend 10 similar movies to the movie selected by user using content based filtering or recommendation, based on features like genres, cast, crew etc.

### Content Based Recommendation
A Content-Based Recommender works by the data that we take from the user, either explicitly (rating) or implicitly (clicking on a link). By the data we create a user profile, which is then used to suggest to the user, as the user provides more input or take more actions on the recommendation, the engine becomes more accurate.

Movies are recommended on basis of their similarity scores.

### Similarity Score
How does it decide which item is most similar to the item user likes? Here come the similarity scores.

It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.

### Cosine Similarity
Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.

![image](https://i.stack.imgur.com/75f8g.jpg)

### Project Flow
1. Download data sets from https://www.kaggle.com to project directory
2. Preprocessing the data
3. Vectorization
4. Cosine Similarity
5. Model for recommeding movies
6. Frontend is made using streamlit

### Built With
* User Interface  - **[Streamlit](https://streamlit.io/)**
* Recommendation Model - **[Python]**  
* Fetching Movies Information and Posters - **[The Movie Database API](https://developers.themoviedb.org/3)**
* IDE - **[PyCharm and Jupyter Notebook]**

## NOTE
1. Download the datasets to your project directory.
2. similarity.pkl file is not uploaded on repo due to its larger size, consider uploading it to Project folder while running the website in PyCharm. Download it from here **[similarity.pkl](https://drive.google.com/file/d/1kqemUlnogdL1aRka-BkhKdMhptmp3Tt_/view?usp=sharing)**
3. Replace API key in app.py with your API key , while running the project in PyCharm.

## Dataset Source
 Download tmdb_5000_credits.csv and tmdb_5000_movies.csv from https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata
 
 ## How to get API key?
 Create an account in https://www.themoviedb.org/, click on the API link from the left hand sidebar in your account settings and fill all the details to apply for API  key. If you are asked for the website URL, just give "NA" if you don't have one. You will see the API key in your API sidebar once your request is approved.

## How to run the Project?
1. Clone or download this repository to your local machine.
2. Install all the libraries mentioned in the requirements.txt file with the command pip install -r requirements.txt
3. Get your API key from https://www.themoviedb.org/. (Refer the above section on how to get the API key)
4. Replace YOUR_API_KEY in app.py file and hit save.
5. Open your terminal/command prompt from your project directory(in PyCharm) and run the file app.py by executing the command "streamlit run app.py".
6. Go to your browser and type the port and your app will get run.

## Website Preview
![Screenshot (4495)](https://user-images.githubusercontent.com/82352524/170825307-73473843-072a-4c70-a11f-0064ff9b05bc.png)

![Screenshot (4496)](https://user-images.githubusercontent.com/82352524/170825334-99e9c9ac-3e71-468a-bbef-a51447efda6d.png)

![Screenshot (4497)](https://user-images.githubusercontent.com/82352524/170825352-2ba240b8-f112-4c68-bf9f-fa5499ff3a2b.png)


