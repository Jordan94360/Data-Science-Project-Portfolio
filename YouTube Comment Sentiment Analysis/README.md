
<p align="center">
    <img src="https://cdn.analyticsvidhya.com/wp-content/uploads/2018/07/performing-twitter-sentiment-analysis1.jpg" width="" height="">
</p>

# **Sentiment Analysis of YouTube Comments**

## 1. Introduction
Ken Jee is a Data Scientist and YouTuber with 190k subsribers to his [channel](https://www.youtube.com/c/KenJee1) that produces data related content. Ken was kind enough to make his YouTube data publicly available for interested data enthusiest to see what unique insights can be found from the data. 

Ken includes 4 different data sets containing data about the metrics of each individual video (Views, Shares, Revenue, etc), his video's comments, etc. 

Ken made a video about this community project that you can watch [here](https://www.youtube.com/watch?v=YPph59-rTxA).

***
## 2. Project Overview


#### **Concept**
After intially reviewing the different data provided by Ken I immediatly became drawn towards the over 10k comments he had and how a sentiment analysis of those comments could be useful. From this intial thought I developed two questions that I would use to drive the purpose of this project. 
-  What's the overall sentiment of the video comments and how does sentiment correlate with successful videos?
-  If sentiment isn't a good predictor of success, then what is? 

#### **Process**
To answer my questions I had two main tasks to complete, **calculate the sentiment** and then **analyze how sentiment impacts the performance of a video**. Below is a narrative outline of how I accomplished this. 

- Using a well known Natural Language Processing (NLP) library called [TextBolb](https://textblob.readthedocs.io/en/dev/) to give a sentiment rating for each comment. TextBlob assigns sentiment on a spectrum with -1 representing negative sentiment, 1 representing positive sentiment and 0 representing a neutral sentiment. 

- Analyzing the sentiment to include the distribution of sentiment, the top/bottom 10 videos by average sentiment score, how sentiment changed over time from the first video posted to the most recent video and how sentiment correlated with the  metrics for each video. 

- Determining what the top/bottom 10 videos were by ranking all the videos by number of Shares, Likes, Sub­scribers gained, Views, and how much revenue was made.

- Analyzing the top 10 videos by their sentiment rating, video length, day of the week they were posted and their average watch time. To make an easy comparrison I included the averages of the top 10 videos, overall average and bottom 10 videos. 

***
## 3. Key Findings

Below are the key findings from my analysis that answer the two intial questions. The findings were assessed based on the insights derrived from the visuals referenced below. 

- **What's the overall sentiment of the video comments and how does sentiment correlate with successful videos?**
    - Comment sentiment is NOT correlated with video performance success or failure. (See Plot 8-17)
    - The majority of comment sentiment is neutral, but is largely more positive than negative. (See Plot 1)
    - None of the best performing videos were ranked in the top 10 videos with high sentiment. (See Plot 3, 5, 19-20)
    - Average sentiment for each video is normally distributed over a medium positive sentiment rating. (See Plot 2)
    - Sentiment increased progressivly from the first video until September 2020 where it has been on the decline since. (See Plot 7)

- **If sentiment isn't a good predictor of success, then what is?**
    - The top 10 best performing videos all were between 6-13 minutes long or were long form (+30 minutes). (See Plot 21)
    - The date a video is posted doesn't really matter. (See Plot 24)
    - Average watch time for the top 10 videos was 3 mintues even thought the total video length was longer than 3 minutes. (See Plot 25)
    - Common topics among the top 10 videos included data science projects and ways to learn data science. (See Plot 24-28)
***
## 4. Tools

- Pandas
- NLTK
- TextBlob
- Seaborn
- Matplotlib

***
