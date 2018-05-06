## Drill: What can data science do?
Estimated Time: 1-2 hours

### As we outlined in the previous section, a lot of data science work can be classified as translation: taking a question and translating it into mathematical or statistical tests or taking statistical results and translating them into something everyone can understand.

### Below we have a series of questions for you to translate into a technical plan. For each question, describe how you would make it testable and translate it from a general question into something statistically rigorous. Write your answers down in a shareable document and submit the link below.

* You work at an e-commerce company that sells three goods: widgets, doodads, and fizzbangs. The head of advertising asks you which they should feature in their new advertising campaign. You have data on individual visitors' sessions (activity on a website, pageviews, and purchases), as well as whether or not those users converted from an advertisement for that session. You also have the cost and price information for the goods.

```
To recommend which product to feature in our advertisement 
I will determine the value or trend for 3 questions.

      A. Which product has the highest profit-margin ?
      B. Which product is trending in sales popularity ?
      C. Which product webpages have the highest pageviews ?

          A. Using a pandas dataframe and the .apply method() I can use the 
          cost & price information for each sale to determine the profit for each sale.  
          I would add this as a new column to the dataframe.  Using this calculated 
          feature and group-by-on-product-category, I can now create histogram chart 
          with mean & standard deviation to give a picture of profit margin over our sales period.

          B.  Using group-by-product-category on my dataframe, I will chart/plot 
          the sales figure trends for each category for each month in our sales period.  
          Using the line chart, we can see which times of the yaer are popular sales 
          months for each respective product category.

          C.  For each page on our website I will chart pageviews for our end - users.  
          The highest visited pages will be easy to determine from the histogram.  
          Once we know our highest rated webpages, we will join this data against 
          the products mentioned on each of those pages.

          Based on the time-of-year, sales-data, & webpage-views I can determine the 
          highest value product to feature on our ad-campaign.

```

* You work at a web design company that offers to build websites for clients. Signups have slowed, and you are tasked with finding out why. The onboarding funnel has three steps: email and password signup, plan choice, and payment. On a user level you have information on what steps they have completed as well as timestamps for all of those events for the past 3 years. You also have information on marketing spend on a weekly level.

```
To determine why signups have slowed, I will determine which users who 
have not completed the onboarding funnel.

I will then created a new feature that calculates how many 
hours (cycle-time) each user spent in each stage of the onboarding funnel.

I can create 2 charts to help explain the slowing down of completed sign-ups.

1.  I will determine which months have the highest number of onboarding events unfinished.
2.  I will chart the marketing spend for each each.

By overlaying marketing spend with long-cycle times for onboarding events, 
I may be able to visually see if where there is a correlation between marketing
spend and cycle time.
```

* You work at a hotel website and currently the website ranks search results by price. For simplicity's sake, let's say it's a website for one city with 100 hotels. You are tasked with proposing a better ranking system. You have session information, price information for the hotels, and whether each hotel is currently available.

```
Use Price and Occupancy to rank each hotel.

Load booking data into a pandas dataframe.

In the dataframe, Create a new measure called 'Popularity' that equates to the 
occupancy-rate of bookings / availabile rooms as a percentage


Perform a group-by against Price & Popularity and use it as the new ranking metric
for web-search
```

* You work at a social network, and the management is worried about churn (users stopping using the product). You are tasked with finding out if their churn is atypical. You have three years of data for users with an entry for every time they've logged in, including the timestamp and length of session.

```
Let's determine Active Users:

After loading the data in a pandas df, let's group users based on login activity.

To visualize this, let's load login data into a histogram.

Let's create enough bins and overlay mean & std-dev.

Once we know the mean login counts we can compare this to our top 25% & 50% users.
```

