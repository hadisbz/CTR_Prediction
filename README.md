**Click-Through Rate (CTR) Prediction using Decision Trees**
---
*   In this tutorial, I’ll walk you through an example of predicting CTR. We will use the dataset from a Kaggle competition, [Click-Through Rate Prediction](https://www.kaggle.com/c/avazu-ctr-prediction), sponsored by Avazu. 

**1. Introduction**

In this tutorial, I will try to predict click-through rate of ads with the Decision Tree algorithm.

**What does Click-Through Rate Prediction mean?**

Let’s assume that you are designing an algorithm for a search engine, and your task is to maximize revenue by displaying the best ads — ads that are both related to search results and are most likely to be clicked — at the top of the search results. How would you do it?

You might say that revenue can be maximized by first filtering on relevancy and then displaying the ad from the highest bidder at the top. There is a problem with this solution. Most advertisers pay for the clicks and not for ad views — they want to be sure that ads lead to their website — so just displaying the ad from the highest bidder wouldn’t maximize revenue. Under this cost-per-click model, advertisers will only be charged if the users actually click on their ads.  So how to correctly approach this problem?

Let’s say you have two ads:

1.   A 1.00$ ad with a 10% probability of being clicked

2.   A 2.00$ ad with a 1% probability of being clicked

Which one would provide the most revenue? The expected revenue (cost * click-probability) for the first ad is higher than that of the second one, even though its dollar-cost is lower, because there is a higher chance that the user will click the first ad. In other words, we can look at the problem of maximizing revenue in terms of accurately predicting the probability that a given ad will be clicked i.e. “click-through rate” (CTR).
