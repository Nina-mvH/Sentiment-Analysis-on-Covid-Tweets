# Overview
This code was developed as a final project for a Big Data course at DIS. The intent of this project was initially to run sentiment analysis on Tweets that came out about the Covid vaccine to see if there was a correlation between sentiments about the vaccine in certain areas and the percentage of populations that got vaccinated in these areas. Due to various limitations, this code just explores the Kaggle dataset “Covid Vaccine Tweets” uploaded by Kash on its own. After some preliminary data cleaning (which included restricting the Tweets to those from the USA to reduce computational time and expense), this code:
- makes a word cloud of the most common words from the Tweets
- makes word clouds of the most common words from the Tweets grouped by month and year (to see if common words changed over time)
- generates word clouds using TF-IDF scores as frequencies
- plot the Euclidean distances between embedding values per month
- plot the PCA visualization of the embedded data
- run K-means clustering on the PCA
- plot the PCA visualization of the embedded data color-coded by the time of the Tweet
- plot the Kernel Density Estimation of the PCA
- print examples of the Tweets which fell into the found PCA clusters

To see the corresponding blog for this project, visit https://medium.com/@nvhoorn/twitter-and-the-covid19-vaccine-in-the-usa-b16664f51271 

## Running this Code
If you want to run this code, it would be easiest to do on Kaggle so you can directly access the original dataset. Once you have access to the data, it should be straightforward to run, just make sure to uncomment the code under "embeddings" the first time you run it. This code will calculate embeddings for each of the Tweets and save them (I would recommend re-commenting out this code after it's done since this process is time consuming and you have to pay to use the OpenAI embeddings model). You will need to update the api_key to use OpenAI for these embeddings. 

## Acknowledgements
The main authors of this code were Nina van Hoorn, Nam Ngo, and Quynh Chu. Sebastian Ray Mason and Lucian Leahu also helped with guiding this project. ChatGPT was also used to help with coding and debugging.

