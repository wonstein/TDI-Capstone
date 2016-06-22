# Making Sense of Review Data

My capstone project aims to improve product review systems by accounting for individual biases among reviewers. Most review aggregation algorithms are a simple average of all existing reviews. However, this method overlooks the fact that people have different standards and use different criteria when forming opinions.

I implement a new algorithm that adjusts each review to account for the individual’s reviewing behavior. Specifically, I normalize each review based on the mean and standard deviation of all of that individual’s reviews. For instance, if an reviewer typically gives 2 or 3 stars, a 5 star review from them is worth more the same rating from an individual that typically gives 4 or 5 stars.

The dataset of reviews I use is sourced from the MovieLens project, which has collected over 20 million movie reviews across over 25,000 films. I evaluate my algorithm by using normalized movie reviews to predict the amount of money a film earns in the box office and compare the results to a model using unaltered reviews.

I am currently in the process of refining the predictive model to include additional features that should help improve accuracy. In particular, I am scraping cast information, budget, and release dates for films from IMDB. I also plan on developing a web app that will allow users to input movie metadata, either real or hypothetical, and generate predicted box office earnings.
