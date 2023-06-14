# Mission to Mars
I used my knowledge of web-scraping and data analysis to obtain news titles and preview text from a website, and obtain data from a website and analyze it.
## Part 1: Scrape Titles and Preview Text from Mars News
1. I used Splinter to open Google Chrome and visit https://static.bc-edx.com/data/web/mars_news/index.html .
2. I extracted all the text elements from the website.
3. I stored the text elements in list of dictionaries with the article titles and the article previews.
4. I exported the results to a json file called 'mars_news.json'.
## Part 2: Scrape and Analyze Mars Weather Data
1. I used Splinter to open Google Chrome and visit https://static.bc-edx.com/data/web/mars_facts/temperature.html .
2. I extracted the table and all the rows of data.
3. I created a list that stored all the column names extracted from the table, and a list that stored the data extracted from the rows of data.
4. I created a DataFrame with the column names and the data.
5. I examined the data type of each column.
6. I changed the 'id', 'sol', 'ls', and 'month' columns to integer data type. I changed the 'terrestial_date' column to datetime. Then, I changed the 'min_temp' and 'pressure' columns to float data type.
7. I analyzed my dataset by answering the following questions:
    1. How many months exist on Mars?
        - 12 months exist on Mars.
    2. How many Martian (and not Earth) days worth of data exist in the scraped dataset?
        - There are 1867 Martian days worth of data in the scraped dataset.
    3. What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
        * Find the average the minimum daily temperature for all of the months.
        * Plot the results as a bar chart.

        ![alt text](https://github.com/glongo001/mars-challenge/blob/main/Starter_Code/avg_min_temp.png)

        - The coldest average minimum temperature is in month 3, and the hottest average minimum temperature is in month 8.
    4. Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
        * Find the average the daily atmospheric pressure of all the months.
        * Plot the results as a bar chart.

        ![alt text](https://github.com/glongo001/mars-challenge/blob/main/Starter_Code/avg_pressure.png)
        
        - Month 6 has the lowest average pressure, month 9 has the highest average pressure.
    5. About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
        * Consider how many days elapse on Earth in the time that Mars circles the Sun once.
        * Visually estimate the result by plotting the daily minimum temperature.

        ![alt text](https://github.com/glongo001/mars-challenge/blob/main/Starter_Code/min_temp_day_count.png)
        
        - In my graph there is a peak around days 690-740 and the next peak takes place at 1375-1425. Therefore, on Martian year is about 685 terrestial days in the graph.
