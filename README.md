# Checkout the app on this link
<img src="images/image.jpg">

# Introduction

For some years, mostly since the rise of social media, fake news have become a society problem, in some occasion spreading more and faster than the true information. Fake news has quickly become a society problem, being used to propagate false or rumour information in order to change peoples behaviour. It has been shown that propagation of fake news has had a non-negligible influence of 2016 US presidential elections. A few facts on fake news in the United States:
• 62% of US citizens get their news for social medias.
• Fake news had more share on Facebook than mainstream news.

So how will you detect the fake news? We will be using Multinomial Naive Bayes method to classify the news article scrapped from the news article link, as fake or real.

# Data
The dataset used is news.csv. This dataset has a shape of 7796×4. The first column identifies the news, the second and third are the title and text, and the fourth column has labels denoting whether the news is REAL or FAKE.

# Project Structre
This project has four major parts :

* fake_news_detection.py - This contains code fot our Machine Learning model to classify the model 
* app.py - This contains Flask APIs that receives news url through GUI or API calls, extracts the article from the url, feeds it to the model and returns the prediction.
* templates - This folder contains the HTML template to allow user to enter url and displays whether the news is fake or real.
* static - This folder contains the CSS file.
* requirements.txt - It contains the list of libraries required to run the heroku app

# Running the project on local machine

 Once you are in the project home directory. Create the machine learning model by running below command -
python fake_news_detection.py
This would create a serialized version of our model into a file model.pkl

Run app.py using below command to start Flask API
python app.py
By default, flask will run on port 5000.

Navigate to URL http://127.0.0.1:5000 

