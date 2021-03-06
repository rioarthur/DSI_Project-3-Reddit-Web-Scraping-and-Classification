### Executive Summary

**What Could Make A Post Popular?**

There's no denying the popularity of Reddit and its many users. It's the source of a lot of internet activity within areas such as politics, entertainment, and education for example. With all of the posts placed on Reddit, they are divided into various sub-categories (known as "sub-reddits") and have corresponding ranks and comments to their posts. Perception may say that popular posts have more comments, but is the number of comments the most important factor to determine the popularity of a post?

The goal here is to show through our analysis which factors do make the most impact on post popularity.

**Methods**

Obtaining the data is an interesting process. On February 19, 2018 data pertaining to the most popular posts was scraped (meaning taking data off of the website) from Reddit's "All" section on its home page. At 10 A.M., 4 P.M., and 10 P.M., the data was scraped to account for the various times people post on Reddit. The data collected from each Reddit post includes:

- Title
- Sub-reddit
- Number of comments
- Time of post
- Domain
- Score (rating of the post)

After dropping duplicates, I was able to come up with 3000 unique posts for analysis. Our indicator of determining if a post was popular out of a sea of random posts was the number of comments that post had. I grouped posts into two categories: 'high' (median number of comments on the post is greater than 22) and 'low' (median number of comments on the post was less than 22). Using an array of variables (such as sub-reddit, domain, etc.) independently and in different combinations was I able to determine what made a post popular.

**Findings**

Using a combination of all the variables listed above, I was able to determine the popularity of a post with 99.1% accuracy. However, which variable was the most important? The findings (along with their accuracy score) are below:
- Only subreddit: 59%
- Only domain: 57%
- Only time: 64%
- Only score: 67%

I also created some new variables (with information from the "Title" of the post) to see if those could help with determining the popularity of a post from a random selection. Based on Google Trends for the week of the data collection, the two most popular topics were the movie Black Panther and "gun control". After creating two distinct variables for those topics, they didn't prove as fruitful as our original variables as they only predicted post popularity with 50.7% and 50.5% accuracy respectively.

In this age of technology, our team assumed that the number of characters in a post would be a strong indicator of determining the popularity of a post. With a median of 48 characters to distinguish between 'high' and 'low', and creating a new variable from that, our accuracy of determining a post popularity was 50.7%.

Our conclusion is that if one were to determine the post popularity using only a single feature, score would be it. However, a better model would be to incorporate all of these various features into analysis.

