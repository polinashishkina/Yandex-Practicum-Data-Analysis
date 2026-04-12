# Project: Gaming Market Research

## Project Description

### Data

Historical data on game sales, user and expert ratings, genres, and platforms is available from open sources. The data is presented through 2016.

The following data on computer game sales is available:
* Game Title
* Platform Name
* Release Year
* Game Genre
* Sales in North America NA_sales (millions of copies sold)
* Sales in Europe EU_sales (millions of copies sold)
* Sales in Japan JP_sales (millions of copies sold)
* Sales in other countries Other_sales (millions of copies sold)
* Critic Rating (maximum 100)
* User Rating (maximum 10)
* Rating — rating from the ESRB. This association rates computer games and assigns them an appropriate age rating.

### Objective:
Using historical data on computer game sales, user and expert ratings, genres, and platforms, identify patterns that determine game success.

### Tasks:

1. Preprocess the data
2. Conduct exploratory data analysis
* Identify patterns that determine game success (analyze sales by platform, sales by genre, the relationship between sales and user and critic reviews, and the relationship between sales and ESRB ratings).
* Identify a potentially popular product.
* Create a user profile for each region (NA, EU, JP).
3. Test the hypotheses:
* Average user ratings for the Xbox One and PC platforms are similar;
* Average user ratings for the Action and Sports genres differ.

### Conclusions:
1. On average, platforms disappear 10-12 years after release. Platforms to focus on: PS4, Xbox One, 3DS.
2. Critic reviews have a greater impact on sales than user reviews.
3. High-selling genres: Action, Shooter, Role-Playing, Sports.
4. User profile by region:
- The top three genres in North America and Europe are the same: Action, Shooter, Sports.
- In Japan, Role-Playing is first, Action is second, with the other three genres lagging far behind.

Platform preferences varied by region:
- In North America, the X360 is the top platform.
- In Europe, the PS3 is the top platform.
- In Japan, there's one clear leader: the 3DS.

The top three ESRB-rated game categories in North America and Europe are the same:
- First place is "M" (ages 17+), second place is "E" (for everyone), and third place is games with an unspecified rating.
- In Japan, the most popular games are those with an unspecified rating.

5. Hypothesis Testing

*The average user ratings for the Xbox One and PC platforms are the same:*

The hypothesis was not confirmed, and we have grounds to reject it.
Therefore, the average user rating for the Xbox One platform differs from the average user rating for the PC platform.

*The average user ratings for the Action and Sports genres are different:*

There is no reason to reject the null hypothesis. The average user ratings for the Action and Sports genres are the same.

### Tools and skills used in the project:

Python, Pandas, plotly, matplotlib, seaborn libraries, data preprocessing, exploratory data analysis, descriptive statistics, data visualization, statistical hypothesis testing
