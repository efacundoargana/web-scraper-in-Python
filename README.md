# web-scraper-in-Python

A friend of mine has to leave his rented apartment and look for a new one. As painful as this experience can be, I decided to use it for help him and like an incentive to improve my Python skills! In the end I want to be able to do two things:

- Scrape all the search results from one of the main real estate websites in Buenos Aires (where we live) and build a database with all the listings found.
- Use the collected listings to perform some EDA, and ultimately try to find undervalued properties (in process).

The website I will be scraping is the real estate portal from [Argenprop](https://www.argenprop.com/), one of the oldest and most visited websites in Argentina. They have a very large amount of real estate listings for us to scrape. Chances are you are using a different website, but you should be able to adapt the code very easily.
Before we begin with the code snippets, let me just give you a summary of what I will be doing. I will use the results page from a simple search in Argenprop website where I can specify some parameters beforehand (like zone, price filters, etc) to reduce the task time, or simply query the whole list of results in Capital Federal.
We then need to use a command to reach ask a response from the website. The result will be some html code, which we will then use to get the elements we want for our final table. After deciding what to take from each search result property, we need a for loop to open each of the search pages and perform the scraping.
