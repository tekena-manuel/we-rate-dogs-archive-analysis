# (WeRateDogs)
## by (Manuel Tekena)


## Dataset


> The dataset that I will be wrangling (and analyzing and visualizing) is the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has over 4 million followers and has received international media coverage.

## Summary of Findings

> Summarize all of your findings from your exploration here, whether you plan on bringing them into your explanatory presentation or not.

During my analysis, I attempted  to answer 4 questions  <br />

What is the most retweeted tweet and which dog is the tweet about? In order to get the answer to this question, we will be using two tables which were during my wrangling after splitting my original Twitter archive table into two because there are two elements that can be observed separately which are the dogs and the tweets. I queried the tweet count data frame using .loc and idmax() to locate the row with the highest number of retweets. <br />
After locating this row I used the tweet_id which is the foreign key here to find the dog stage of the dog the tweet was about and it was doggo.<br />

what dog stage has generally better ratings? In order to get the answer to this question, we will be plotting a scatter plot graph to show the relationship between the ratings and the different dog stages. To get our ratings we will be using the numerator score because that is the actual score as opposed to the denominator which is the total score. After plotting the scatter plot it occurred to me that the only dog stage in the data set was doggo. Doggo dogs have a relatably low rating compared to other dogs but because the other dogs have empty dog stages we can't identify what dog stages they are.<br />

Lastly, I attempted to check which dog had the best rating in the we rate dogs archive. To achieve this I used a similar code to question to return the row with max value in rating and the dog's name is Atticus