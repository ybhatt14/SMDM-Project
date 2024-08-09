**Informal Analysis of Twitter Usage Amidst the COVID-19 Pandemic**

**Overview**
In this project, we have analyzed a dataset of tweets related to the COVID-19 pandemic to gain insights into how people are using Twitter to express their emotions and opinions during this challenging time.

**Data Source**
The data, which includes a sample of 10,000 tweets with COVID-19-related hashtags like #COVID19, #coronavirus, and #pandemic, was gathered using the Twitter API. After the data had been cleaned up of stopwords, punctuation, and URLs, it was subjected to several natural language processing techniques for analysis.

**Using LDA for Topic Modeling**

Topic modeling using LDA, an unsupervised machine learning method that separates topics from a collection of documents, was the first step. Tokenizing, lemmatizing, and stopword elimination were done during the preprocessing of the tweets. The most crucial subjects in the tweets were then determined using the LDA model, which had been trained on the preprocessed data. Coherence ratings were used to estimate the ideal amount of topics. To give an overview of each topic, the top words for each topic were printed.

**Sentiment Analysis**
The dataset we have generated in this project is a CSV file containing tweets related to COVID-19 and is saved in tweet_sentiments.csv. The dataset includes the following columns:

- Tweet: The text of the tweet.
- Polarity: A numeric score indicating the sentiment polarity of the tweet (ranging from -1 to 1, where -1 is very negative and 1 is very positive).
- Subjectivity: A numeric score indicating the subjectivity of the tweet (ranging from 0 to 1, where 0 is very objective and 1 is very subjective).
Sentiment Analysis
We began by performing sentiment analysis on the tweets to categorize them into positive, neutral, and negative categories based on their polarity scores. We found that out of 500 tweets, 196 tweets were positive, 184 were neutral, and 120 were negative. (these value differ everytime we will run the code)

**Emotion Analysis**
We then performed emotion analysis on the tweets using the VADER sentiment analyzer and a set of predefined emotion categories (fear, happiness, sorrow, and neutral). We first identified the dominant emotion category for each tweet based on the presence of specific keywords in the tweet. If no emotion category was identified, we used the VADER sentiment scores to determine the dominant emotion category.

The results of the emotion analysis showed that out of 500 tweets, 43.6% expressed happiness, 31.6% expressed sorrow, 20.2% expressed fear, and 4.6% were neutral. (these value differ everytime we will run the code)

**How to run the code**
-Install Jupyter Notebook and Python 3.9 on your computer.
-The repository can be downloaded from blackboard in .zip format, extract it and open the folder in Visual Studio Code and thus run the file using the run code.
-Visual Studio Code should now display the project folder.
-By hitting Ctrl + Shift + in VSCode, the terminal will be displayed.
-In the terminal, type jupyter notebook and hit Enter/Alternatively run directly use the run icon.
-Find the index.ipynb file by navigating to it in the Jupyter Notebook browser window.
-Use the Run button or the keyboard shortcut Shift + Enter to run each cell in turn after opening the index.ipynb file.
Note: Before running the code, be sure to install the external libraries that the index.ipynb file utilizes. Do note that the results would be different each time you run the code.

**Conclusion**
Our analysis provides insight into how people are using Twitter to express their emotions and opinions during the COVID-19 pandemic. We found that overall, the majority of tweets expressed happiness, but a significant portion also expressed sorrow and fear. These results can be useful for understanding the emotional impact of the pandemic on people and for developing interventions to support individuals during these difficult times.