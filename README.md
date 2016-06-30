# Accounting for Taste

My capstone project aims to improve product review systems by accounting for individual biases among reviewers. To demonstrate, I analyze a dataset of 20 million film reviews across 27,000 films from the MovieLens project

Most review aggregation algorithms are a simple average of all existing reviews. However, this method overlooks the fact that people have different standards and use different criteria when forming opinions. I implement a new algorithm that adjusts each review to account for the individual’s reviewing behavior. Specifically, I normalize each review based on the mean and standard deviation of all of that individual’s reviews.

We can aggregate these normalized ratings and compare them to conventionally aggregated movie scores. Although there is substantial correlation between the two measures, normalizing individual reviews does change the distribution of movie scores.

Given these new scores, we can assess the value of normalizing individual reviews by comparing the accuracy with which each method predicts domestic box office grosses. Earnings for nearly 10,000 films were scraped from IMDb.

Compared with a model using unadjusted reviews, my model using normalized film  reviews performs better across a variety of metrics. Granted, the improvements are generally small, but this should change as the base model is refined.

Further work will focus on improving the base model to more accurately predict earnings. I plan to incorporate data on film studios, directors, and casts, as well as use text analysis on film titles, plots, and critic reviews.
