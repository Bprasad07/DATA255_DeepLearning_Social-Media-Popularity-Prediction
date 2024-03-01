# DATA255_DeepLearning_Social-Media-Popularity-Prediction
DATA255_DeepLearning_Social-Media-Popularity-Prediction

The Social Media Popularity Prediction project is dedicated to forecasting the potential impact of sharing different posts on social media platforms by a publisher. This involves analyzing various attributes of a post, such as its content and format, to automatically predict its popularity metrics, such as view count for Flickr etc.

For further information and insights into this prediction task, please visit the official website: http://smp-challenge.com/.

This dataset encompasses 680K social media posts extracted from Flickr.com and traces the photo-sharing activities of anonymized users over three years. The dataset is multifaceted, comprising photo URL, time flag of posts, and user metadata. To measure an online post's popularity, the SMPD dataset consists of popularity scores premised on the engagement of each post. To ensure users' privacy and sharing patterns, user and post-identification details are anonymized, and post-timestamps are transmuted into time segments with integer indices.
To augment the capabilities of the SMPD dataset, scraped metadata detailing the post's reach across various groups and engagement metrics for individual users is integrated. This additional data aided in assessing the breadth and depth of the post's influence, factoring in the prominence of the groups it reaches and the individuals it engages.

This project addresses this gap by incorporating novel social network effect parameters, namely Flickr group interactions, group popularity, and group posts count, to enhance the predictive accuracy of the models.


# Approach

The approach combines machine learning techniques and Deep Learning frameworks with in-depth analysis of Flickr posts data, encompassing features such as post content, user engagement, and metadata along with Flickr group interactions, group popularity, and group posts count. The challenge of seamlessly integrating multi-channel metadata, encompassing image features, text content, and various numerical and categorical attributes, into a unified deep learning model architecture as one framework and a sophisticated combination of ML and NLP techniques as another framework is a focal point of the approach. 

The results reveal insights into the nuanced dynamics that drive image popularity on social media. Among the four models from two frameworks, LightGBM, XGBoost, CatBoost, and Multimodal Fusion NN model, LightGBM demonstrates high accuracy in predicting the engagement levels of posts, considering aspects such as contextual relevance, and user and group interactions with the lowest MAE of 0.5451 and SRC of 0.9259 by employing sophisticated feature engineering with NLP and ML techniques. The results underscore the significance of incorporating SNE context, revealing that group interactions, popularity, and post count significantly contribute to the predictive power of the model.

The LightGBM model outperformed other models with a MAE of 0.545 and SRC of 0.925. In contrast, the Multimodal Deep Learning (DL) model showed lower performance despite ranking 8th on the SMP Challenge leaderboard, where LightGBM secured the top position on the leaderboard.



