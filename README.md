IntelligentMusicRecommendationSystem
========================================================

**Mood Detection** model can detect face from any image and then it can predict the emotion from that face.
It can do this from both still images and videos.
After predicting the emotion from the person's face, this recommender system takes the predicted emotion as input and generates recommendations by processing a Spotify dataset taken from a Kaggle contest. The music's mood is predicted from a model trained with **data_moods.csv**. The recommender system will generate top 40 songs as recommendations for a spotify playlist.

Mood Detection
--------------
**Mood Detection** model will predict one of the emotion among 7 emotions listed below-
* Happy
* Sad
* Angry
* Disgust
* Surprise
* Neutral
* Fear

Music Mood Prediction
---------------------

Every songs in the main dataset in the **Datasets.7z** folder predicted to one of the mood among 4 moods listed below-
* Happy
* Sad
* Energetic
* Calm

By using a music mood classifier model  each song's mood was predicted in the intermediate dataset **kaggleSpotifyMusicMood** in the Dataset.7z folder.

Music Recommendation
--------------------
The main project file is **music_recommender.ipynb** file. This recommendation system is using content based filtering. The following steps should be followed to recommend music-
* Dataset Pre-processing
* Feature Engineering
* Connect to Spotify API
* Create Playlist Vector
* Generate Recommendation using cosine similarity

In summary,this project will take an image of an user and predict emotion using **Emotion Detection** model. By prioritizing the songs from the main dataset **kaggleSpotifyMoodFinal.csv** with music mood getting compared to different face emotions, this system will generate top 40 songs to recommend for a particular Spotify playlist. 


