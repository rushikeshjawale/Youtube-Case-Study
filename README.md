# Youtube Case Study
## Project Description:

YouTube is a source of income for a lot of people. It started as an excellent platform to upload videos to share knowledge, experiences, and tutorials. Also, many people have dedicated their lives to creating content just for youtube and so many have earned not only recognition and fame but also money.

In this case study, we analyze certain features and try to find an appropriate outcome or data. This data will help understand youtube's chronology that will help them build or start their own business on this platform.

This case study also helps other businesses in digital marketing that use youtube platform for marketing and advertising. By studying the extracted data, we can analyze which category of video is most watched, loved and disliked by viewers.

Below are some problem statements that have been considered and solved

Then i begin by scraping internet web sites and accessing APIs to collect data in various formats like .csv files, excel sheets, and databases.   
 
 

Once this was completed, i made that data ready for analysis using data wrangling techniques. 
 


once the data was ready i applied statistical techniques to analyze the data.  Then i collected all this information together by using  IBM Cognos Analytics to create my dashboard. And finally, showed off my storytelling skills by sharing my findings in a presentation.

# Outline:

| SL. NO |       Outline       |
|:------:|:-------------------:|
|   1    |  Executive Summery  |
|   2    |    Introduction     |
|   3    | Question for Analysis |
|   4    |       Results       |
|   5    |     Conclusion      |


## Executive Summary:

This Project will give you an overview of :

1. Trending videos of youtube.

2. Positive and negative comments ratio.

3. Engagement of audience.

4. Likes and Dislike ratio as per category.

5. Affects of views over likes.

## Introduction:

- This presentation has been created for digital marketing companies and business to help them in advertisement and promotion.


- The presentation will help identify the parameters which are responsible for type of audience engagement on youtube platform.

## Question for Analysis:

- Perform Sentiment analysis and prepare a word cloud representation ?

- Perform Emoji Analysis and find out Top 10 emojis used emojis in comments ?

- Analyse which video category has maximum likes ?

- Find out which category has more rate of likes ?

- Analyse whether views affects likes or not ?

- Find which channel has the largest count of trending videos ? 

## Software used in this project:

In case of local machine We are going to use the following softwares in this project :

Programming Language : [Python](https://www.python.org/)

IDE : [Jupyter Notebook](https://jupyter.org/)

Packages : [Pandas](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html), [Numpy](https://numpy.org/), [Seaborn](https://seaborn.pydata.org/), [Matplotlib](https://matplotlib.org/), [TextBlob](https://textblob.readthedocs.io/en/dev/).

## The Data Sets:
Download dataset zip file and extract it into your system to use

[Youtube_dataset](https://drive.google.com/drive/folders/17xmw-xuN0aw5RoQrqgoRzeTfMlKoXLby) zip file
# Results:

## Q1) Perform Sentiment analysis and prepare a word cloud representation ?
To perform the sentiment analysis you should consider two key points polarity and subjectivity.
    
polarity value lies between the range of -1 to +1, so if polarity of comment is near to -1 or less  than 0 the comment is consider as negative and if polarity value is close to +1 or more than zero then comment is consider positive.

After performing Sentiment analysis this is a result.

![p1.png](https://github.com/rushikeshjawale/Youtube-case-study/blob/master/images/1.png)

As you can see here the comments which has polarity 1 or close to 1 are positive comments
and comments which has polarity less than 0 are negative comments

### 1. Positive Word Cloud:

![positive_word_cloud.jpeg](https://github.com/rushikeshjawale/Youtube-case-study/blob/master/images/positive_word_cloud.jpeg)

### 2. Negative Word Cloud:

![Negative_word_cloud.jpeg](https://github.com/rushikeshjawale/Youtube-case-study/blob/master/images/Negative_word_cloud.jpeg)

#### Conclusion:

The words that are bigger in size are the words that have been used in the comment section most of the time.
you can plot pie chart to compare the percentage of negative and positive polarity further. From which you can 
decide whether the video is positive or hateful.

## Q2) Perform Emoji Analysis and find out Top 10 emojis used emojis in comments ?
Emojis are small digital images or icons that are depictions of human emotions, living beings, objects, and even certain symbols.
These can be used across the internet such as in text messaging, social media platforms and pretty much on any informal modes of communication.

To conduct emoji analysis. First, we install and import the emoji library, Every emoji has its own unicode.
An emoji library is the library which contains emojis with respect to their unicode.

After carrying out certain operations, we trace the result in the bar graph using Plotly.

![Top10_emoji.jpeg](https://github.com/rushikeshjawale/Youtube-case-study/blob/master/images/Top10_emoji.jpeg)

#### Conclusion:

Based on the bar chart, you may conclude that the youtube data we use has more funny videos.

## Q3) Analyse which video category has maximum likes ?

YouTube likes are one of the criteria the algorithm considers when choosing videos to highlight.
The more likes a video gets, the more likely it is to be featured in relevant YouTube search results.

After carrying out certain operations, we trace the result into box plot.

![likes_count.jpeg](https://github.com/rushikeshjawale/Youtube-case-study/blob/master/images/likes_count.jpeg)

#### Conclusion:

Here we can see their are lot of audience who likes music videos

## Q4) Find out which category has more rate of likes ?

For example, if gaming videos have an average 5.47% like-to-view engagement ratio,
while music videos get more views, but only an average 2.28% of viewers will hit the like button.
This is called like rate.

![Like_rate.jpeg](https://github.com/rushikeshjawale/Youtube-case-study/blob/master/images/Like_rate.jpeg)

#### Conclusion:

Above box plot helps us to understand which category has more like rate or you can say on which category audience
engaged the most

## Q5) Analyse whether views affects likes or not ?

The core idea is we have to find the correlation between views and likes,
if there is a higher correlation value that is close to 1 
eg- 0.8, 0.9, 0.7 ... then there is a higher probability that if any
the video has a higher number of views then it may have a higher
number of the likes

Correlation is a statistical measure that expresses the extent to which two variables are linearly related
(meaning they change together at a constant rate). 
It's a common tool for describing simple relationships without making a statement about cause and effect.

### 1. Regression Plot:

![views_affect_likes.jpeg](https://github.com/rushikeshjawale/Youtube-case-study/blob/master/images/views_affect_likes.jpeg)

The strainght line is regration line

### 2. Heat map:

![heatmap_correlation.jpeg](https://github.com/rushikeshjawale/Youtube-case-study/blob/master/images/heatmap_correlation.jpeg)

 These are all the correlation values
 as you can see that:

     on views 1.0, likes 0.7
     on views  0.7, likes 1.0

## Q6) Find which channel has the largest count of trending videos ?

As we know the trending videos has more number of likes as compare to other videos or you can say that the highly liked
videos are on trending list.
So we have to find 

![Top20_channel_MostTrending_videos.jpeg](https://github.com/rushikeshjawale/Youtube-case-study/blob/master/images/Top20_channel_MostTrending_videos.jpeg)

#### Conclusion:

These are top20 channels which has most number of trending videos.
and hence the most trending video channel is 'The Late Show with stephen colbert'

# Ovearall Conclusion:

By solving these above problem statements now we have an overall idea about the algorithms of the youtube platform,
and we know what kinds of videos go on the trend list and what kinds of videos people love the most.
we also have some idea of the types of videos that may have hateful comments and emojis.

So, if someone wants to begin their career on YouTube, they may have an idea,
about what kind of youtube channel he or she should begin.
This data also helps digital marketing businesses advertise their products because it shows the most trendy channel.

# Authors

- [@Rishikesh Jawale](https://github.com/rushikeshjawale?tab=repositories)

# 🔗 Connect with me
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rishikesh-jawale-433551252/)