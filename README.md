# CascadeCup
Data Science Hackathon by Trell in partnership with CNA club IIT Guwahati.

## Overview
Built a model to help Trell provide better experience to their users by giving them a better user age specific content which people might find more relatable. Built an ensembling model using Random Forest, XGBoost and LGBM classifiers trained using RandomizedSearchCV on a dataset containing the user activity of Trell's users and used Pipeline to keep the code clean and feature engineering to get better performance and achieved a "f1_score" of 80.42 and a ranked 50 out of 500 participants in the second round of the hackathon. 

## Aim
The competition aimed to predict the age-group of the user based in his activity on the social media platform of Trell, thus helping trell improve its user feed.

## Requirements
The following packages must be installed with Python3 already installed:

* Numpy
* Pandas
* Scikit-LearnWeighted F1 Score
* Matplotlib
* Seaborn
* XGBoost
* Lightgbm

## Evalutaion
The evaluation metric for this competition was the Weighted F1 Score. In Weighted F1 Score - The F1 Scores are calculated for each label and then their average is weighted by support - which is the number of true instances for each label. 

## Data 
The data was provided by Trell in the CSV format(the same has been included in the repo) and consisted of basic details about the user and thier activity on the social media platform of Trell.

###### Data fields:

'userId'
: Unique number given to each user.

'tier'
: Tier of the city in which the user is residing.

'gender'
: Categorical feature representing the gender of the user. 1 represents male and 2 represents female.

'following_rate'
: Number of accounts followed by the user(feature is normalized)

'followers_avg_age'
: Average of age groups of all the followers of the user.

'following_avg_age'
: Average of age groups of all the accounts followed by the user.

'max_repetitive_punc'
: Maximum repititive punctuations found in the bio and comments of the user.

'num_of_hashtags_per_action'
: Average nubmer of hashtags used by the user per comment.

'emoji_count_per_action'
: Average number of emojis used by the user per comment.

'punctuations_per_action'
: Average number of punctuations used by the user per comment.

'number_of_words_per_action'
: Average number of words used by the user per comment.

'avgCompletion'
: Average watch time completion rate of the videos.

'avgTimeSpent'
: Average time spent by the user on a video in seconds.

'avgDuration'
: Average duration of the videos that the user has watched till date.

'avgComments'
: Average number of comments per video watched.

'creations'
: Total number of videos uploaded by the user.

'content_views'
: Total number of videos watched.

'num_of_comments'
: Total number of comments made by the user (normalized)

'weekends_trails_watched_per_day'
: Number of videos watched on weekends per day.

'weekdays_trails_watched_per_day'
: Number of videos watched on weekdays per day.

'slot1_trails_watched_per_day'
: The day is divided into 4 slots. This feature represents the average number of videos watched in this particular time slot.

'slot2_trails_watched_per_day'
: The day is divided into 4 slots. This feature represents the average number of videos watched in this particular time slot.

'slot3_trails_watched_per_day'
: The day is divided into 4 slots. This feature represents the average number of videos watched in this particular time slot.

'slot4_trails_watched_per_day'
: data

'avgt2'
: Average number of followers of all the accounts followed by the user.

###### Target:

'age_group'
: This is a categorical feature denoting the age of the user. Age of users is divided into 4 groups, 1: <18y; 2: 18-24y; 3: 24-30y; 4: >30y
