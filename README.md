# Project-6 US Youtube Trending Videos Data Analysis

This exploratory data analysis will focus on trending Youtube videos in the United States of America. The purpose of this analysis is to explore and gain a better understanding of the Youtube videos that people are interested in and what factors possibly correlate with trending videos. More specifically, this analysis will tackle five questions:

1. Do the number of views have a correlation with the number of likes? How about the number of comments?
2. Is there a correlation with the publish time and the number of likes and views?
3. What were the most popular topics for trending videos in specific categories?
4. How long does it take a video to become trending? (Starting from publish date)
5. What kinds of videos would lead to a higher number likes and views? How about dislikes?

## Project at a glance:
Code used: Python, Numpy, Pandas, Matplotlib, Seaborn and Wordcloud

For this analysis I will be using two datasets, and the datasets are from the Kaggle website page entitled "Trending Youtube Trending Statistics". 

1. The first dataset contains trending videos and the following information listed below:

* Video Id
* Trending Date
* Title
* Channel title
* Category ID
* Publish time
* Tags
* Views
* Likes
* Dislikes
* Comment count
* Thumbnail link
* Comments disabled (True or False)
* Ratings disabled (True or False)
* Video error or removed (True or False)
* Description

2. The second dataset consists of the video etag and the category number and title.

## Data Cleaning and Preparation
1. Converted the date columns into the proper datetime format and extracted the publish hour and date.
2. The first dataset only has the category ID, and so I merged the first dataset with the second dataset to get the category title based on the category ID column.
3. Added columns for the number of tags, description length and title length.
4. Removed the rows with null values for description.

## Data Exploration and Visualization
![Image](https://github.com/rafationgson/Project-5/blob/master/yt-channels.png)

## Summary and Conclusion of findings
* The top channels with the most number of trending videos include ESPN, The Tonight Show Starring Jimmy Fallon and Netflix. This is also reflected in the most popular video category which are entertainment. In terms of the video categories, the dataset is imbalanced because majority of the videos are in either Entertainment or Music.
* Majority of these videos were published in 2017-2018, and based on the graph for 2018, there is a consistent trend of around 100 to 300 videos being published per month. Taking into account that the trending dates are from 2017-2018, the findings of this analysis would be more representative of Youtube videos in 2018.
* Majority of the trending videos do not have the comments disabled or ratings disabled as these can help lead to more likes and views. It also makes sense that very few are video errors or removed as this would make it more difficult for videos to become trending.
* Majority of the videos have description lengths of around 200 to 1200 characters and title lengths of around 30 to 50 characters, and so this can be good insight for people making Youtube videos.
* There is a strong positive correlation between the number of views and comments with the number of likes. A higher number of views and comments mean more engagement, and this can lead to opportunites to get more likes. There is a correlation with the number of dislikes with the number of likes as well. A reason for this can be with the increase in the number of views, likes, and comments, it will bring more people who dislike the video as well.
* Videos that were publish around 2:00 - 4:00 PM experienced the most number of likes. These times would probably have the most number of people online on Youtube. Note that there are also videos published at 4:00 AM that had large number of likes as well, and so this needs more research and data to verify.
* For the music category, the most popular topics consist of music video, official video, charlie puth, nicki minaj, dua lipa, daddy yankee, hip hop, and calvin harris. For the entertainment category, the most popular topics consist of late night, late show, will smith, funny videos, graham norton, and star wars. For the gaming category, the most popular topics consist of nintendo switch, battle royal, clash royale, smash bros, video game, and faze rug. For the howto & style category, the most popular topics consist of make up tutorials, cooking, and food.
* Most of the trending videos take around 2-6 days to become trending, and longer than that it becomes less probable that the video will become trending. BUT it is also worth noting that there are videos that became trending even after 1000 days from the publishing date. One reason for this can be that a topic suddenly became popular later on, and this led to people searching this video topic. There can be other reasons for this as well.
* The music and entertainment category videos have the most number of likes, views, and dislikes. The shows, autos & vehicles, and travel & events categories consistently have the lowest number of likes, views, and dislikes. Based on this, we can see what videos are people more interested in watching. Video categories that have a large number of likes and views also have a large number of dislikes. This makes sense as popular topics will have many people with differing opinions as well.
