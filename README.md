
# How to maximize a post retweet count on Twitter

#### Abstract

> We’d like to figure out what one can do to make a tweet seen by more people (get more retweeted). We propose to analyse the factors that covary with the retweet count from user and tweet perspectives. At the user level, the original paper showed us the number of followers/ followees are positively associated with retweet count. However, we still have little idea of how exactly are they correlated: for example, **is the retweet count linearly increase with the number of followers? Is there certain "threshold effect”?** Also, we are interested in **whether posting in English - an international language - helps in getting more retweet count.** At the post level, they found that the presence of hashtags is positively correlated and the presences of URLs. However, one might also be interested to know **when is the best to post**: is there a time in a day when a post gets a higher chance of being retweeted? What about holidays when people may be more active on social media?


### Research Questions :rocket: 


- [x] When is the best time to tweet?
- [x] (We know from the paper adding hashtags in the post might be helpful, while not adding URLs.)
- [x] How does the number of followers/ followers/ friends matter? (We knew from the paper that the number of followers/ followers are positively associated with retweet count, but is the effect linear?)
- [x] Does tweeting in a more commonly spoken language (like English) help?


### Proposed dataset
	
:memo:EgoTimelines: The dataset contains ego users’ dynamic activities, including posting original tweets, retweeting, replying and @-mentioning. It also contains information about the number of retweets, presence of URLs and presence of hashtags for each tweet. The dataset is ideal to analyze the contributions of factors at the post level to the post’s influence.

:memo:EgoAlterProfiles: The dataset contains sampled users profiles, including the number of followers, languages, account created time, etc. Combined with the “retweet_count” term in EgoTimelines dataset we can analyze the effect of the number of followers and language (factors on the user level) on the post’s influence.

:memo:EgoNetwork: This dataset contains all pairs of ego-alter relationships, where the number of followees for each ego users can be calculated and further analyzed.

### Methods
First plot relevant graphs to get a rough idea about data, then make observations or propose hypotheses and test them.

Specifically, on the tweet level, plot time of posting against the number of retweets. On the user level, plot graphs to show the distribution of average number of retweets with number of followers/ followers/ friends. 

According to the plots, make observations or formulate hypotheses. For instance, we may observe that the number of retweets grows considerably after some threshold for the number of followers. Or, we may hypothesize that the relationship between the number of followers and average number of retweets is nonlinear. 

Then we carry out necessary data processing, like propensity score matching and perform hypothesis testing.


### Proposed timeline

- [x] Load data, understand the dataset and preprocess data. Week1
- [x] Gain an insight through visualization and start to prepare the story. Week2
- [x] Carry out regression analysis and use techniques for controlling covariants. Week3
- [ ] Prepare the presentation. Week4

### Organization within the team
- Shuqi Wang: Analyze the factors on the user level.
- Yingxue Yu: Analyze the factors on the post level.
- Yian Wang: Write up the story and prepare the final presentation. 

### Questions for TAs (optional)
- What does each column (especially ‘id’, ‘retweetedUserID’,	‘replytoUserID’, ‘metionID’) mean in the dataset EgoTimelines?
- Should the video be similar to an online presentation?
