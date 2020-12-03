# Myers-Briggs Type Indicator (MBTI) Machine Learning Model

Personality as defined by the American Psychological Association (https://www.apa.org/topics/personality) refers to individual differences in characteristic patterns of thinking, feeling and behaving. The study of personality focuses on two broad areas: One is understanding individual differences in particular personality characteristics, such as sociability or irritability. The other is understanding how the various parts of a person come together as a whole.

This project was designed to predict the personality of a person based on user inputs.

Various Machine Learning algorithms were used to find the best predictive accuracy and then was designed into an interactive webpage that has been hosted through Heroku.

The data was collected through the PersonalityCafe forum, as it provides a large selection of people and their MBTI personality type, as well as what they have written.
The dataset contains over 8600 rows and has 2 columns: type of Myers-Briggs personality 4-letter code and section of each of the last 50 things posted. The classification methods used to train and test the data were:

Neural Networks
Random Forests
Support Vector Machine (SVM)
k-nearest neighbors (KNN)
Binomial Naïve Bayes.

Key findings were extracted from the heavily texted data and captured features such as number of words per post, the punctuation used as well as made use of a sentiment analysis to determine polarity and subjectivity in the text. Sentiment determines the ‘positivity’ or ‘negativity’ of a piece of writing. The TextBlob library was used to process the comments in the dataset and determine the sentiment for each row. Sentiment is rated from -1.0 to 1.0, where -1.0 is the most negative and 1.0 is most positive.

Since the data was severely imbalanced in personality type, identifying all the 16 different categories was affecting the accuracy scores of the models and hence decided to divide the personality types from 16 different categories into 2 categories. We wanted to focus on predicting whether a post was from an introverted personality or an extroverted personality.

We then tried calculating the accuracy for each category to compare if our model would be able to accurately predict if a post is Intuitive or Sensing, Feeling or Thinking, Judging or Perceiving. We later found out that the Neural Network model was best able to predict scores in all categories with the most accurate being in Intuition – Sensing and a close second being Introversion – Extroversion.

Finally, we visualized the results in Tableau and designed a webpage for the users to interact with and hosted it through Heroku.
