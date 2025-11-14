## Project Overview
The group used exploratory data analysis to generate insights for a business stakeholder.

## Business Understanding
#### Business Problem

The company management has decided to create a new movie studio, but they don’t know anything about creating movies. As a data scientist you are charged with exploring what types of films are currently doing the best at the box office. You must then translate those findings into actionable insights that the head of your company's new movie studio can use to help decide what type of films to create.

#### Research Objective
Determine the best performing genres and studios and their financial outcome to determine the investment and production decisions.

#### Research Objectives
1. To determine the best performing genres according to ratings
2. To determine the best performing genre based on popularity(num of votes)
3. To analyze film performance across studios, years and domestic versus international markets
## The Data

In the folder `zippedData` are movie datasets from:

* [Box Office Mojo](https://www.boxofficemojo.com/)
* [IMDB](https://www.imdb.com/)
* [Rotten Tomatoes](https://www.rottentomatoes.com/)
* [TheMovieDB](https://www.themoviedb.org/)
* [The Numbers](https://www.the-numbers.com/)

### Source of Data
* `im.db.zip`
  * Zipped SQLite database 
  * `movie_basics` and `movie_ratings` tables are most relevant
* `bom.movie_gross.csv.gz`
  * Compressed CSV file 

### Research Finding
![alt text](image-1.png)
The graph shows that News, Documentary and Biography are the top-rated genres on average, with News having the highest average rating of 7.13. 
This suggests that audiences tend to favor movies in these genres in terms of quality. 
Genres like Reality_TV, Horror and Adult while popular, have slightly lower average ratings among the top 10.

![alt text](image-2.png)
Genres like Adventure, Sci-Fi and Fantasy dominate audience attention and generate the highest average votes per movie.
Genres like Documentary are have low average votes or have smaller audiences even if there are many movies.
This can guide studios on which genres have both high engagement and high potential for audience reach.
The studio can balance high-reach genres with niche genres to diversify content and capture both mass and loyal niche audiences.

![alt text](image-3.png)
There is a strong positive relationship(0.79) between the number of movies and the number of votes
This means that the number of movies produced influence the number of votes.

For a hypothesis test to check whether some studios perform better in terms of gross total income;
         Reject Ho since p_value(0.00) < than 0.05
Atleast one studio has a difference in the mean if the gross income. 
Concluding that the type of films the best performing studios produce have a higher income


![alt text](image-4.png)
The high performance in 2016 and 2017 suggests that the industry is still capable of generating massive revenue.

![alt text](image-5.png)
There is a strong positive correlation between domestic and foreign market (0.79)
The studio can safely assume that films successful locally are likely to perform well internationally and investment in global marketing can increase profit.

With evidence from a hypothesis test and true means, global markets have higher revenue.
In conclusion, the datasets used are the im.db dataset and the box office mojo(bom.movie_gross.csv) dataset to conduct the analysis.
1. **Based on the rating:**  
    News, Documentary and Biography are the top-rated genres on average, suggesting that audiences tend to favor movies in these genres in terms of quality. Genres like Reality_TV, Horror and Adult while popular, have slightly lower average ratings.

2. **Based of popularity:**  
    Adventure, Sci-Fi and Fantasy genres dominate audience attention and generate the highest average votes per movie.Genres like Documentary are have low average votes or have smaller audiences even if there are many movies.
    This can guide studios on which genres have both high engagement and high potential of audience reach.
    Though the number of votes is highly influenced by the number of movies in the genre with a corr=(0.7).

3. **Based on the income generation:**  
    An ANOVA test confirmed that there is a significant difference in mean gross income among film studios, meaning certain studios consistently outperform others financially. Benchmarking the HC(Hallmark), P/DW(Paramount DreamWorks) to see the type of films they produce thus their high income is a great strategy to determine the best films to invest in.

    There is a strong positive correlation (0.79) between domestic gross and foreign gross.A film that is successful in the domestic market is highly likely to perform well internationally. Investing in global marketing for films that perform well domestically is a strong strategy to increase overall profit.

    There is also an upward trend in the gross total income of the movies over the years suggesting that the studio is likey to make profit.
