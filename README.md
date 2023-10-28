# Module_11_challenge_scrape_analyze_mars
Module_11_assignment

#  Mars Data - Scraping and Analysis - Challenge

## Background:

Extracting and examining information from websites that provide news and weather data about Mars.

## Data Source
[Mars news site](https://static.bc-edx.com/data/web/mars_news/index.html)

[Mars Temperature Data site](https://static.bc-edx.com/data/web/mars_facts/temperature.html)

#  Deliverables:
## Deliverable 1: Scrape titles and preview text from Mars news articles.

Access the Jupyter Notebook located in the starter code folder named part_1_mars_news.ipynb. Execute the tasks outlined within the code as you proceed with the steps to scrape data from the Mars News website.
* 1 Utilize automated web browsing to navigate to the Mars news site. Examine the webpage to pinpoint the elements that need to be extracted during the scraping process.
* 2 Generate a Beautiful Soup object and leverage it to extract textual elements from the website.
* 3 Retrieve the titles and preview text from the scraped news articles. Organize the extracted data by storing the results in Python data structures as outlined below:
 Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. An example is the following:
 
  Store all the dictionaries in a Python list.

  Print the list in your notebook.

 * 4 Optionally, store the scraped data in a file (to ease sharing the data with others). To do so, export the scraped data to a JSON file. (Note: there will be no extra points for completing this.) 

## Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.
Open the Jupyter Notebook in the starter code folder named part_2_mars_weather.ipynb. You will work in this code as you follow the steps below to scrape and analyze Mars weather data.
* 1 Use automated browsing to visit the Mars Temperature Data Site. Inspect the page to identify which elements to scrape. Note that the URL is https://static.bc-edx.com/data/web/mars_facts/temperature.html.
* 2 Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. However, use Beautiful Soup here to continue sharpening your web scraping skills.
* 3 Compile the extracted data into a Pandas DataFrame. Ensure that the DataFrame columns align with the headers from the website's table. Here's a breakdown of the column headings:
 
 id: the identification number of a single transmission from the Curiosity rover

terrestrial_date: the date on Earth

sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars

ls: the solar longitude

month: the Martian month

min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)

pressure: The atmospheric pressure at Curiosity's location

* 4 Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.
* 5 Analyze your dataset by using Pandas functions to answer the following questions:

How many months exist on Mars?

How many Martian (and not Earth) days worth of data exist in the scraped dataset?

What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:

Find the average minimum daily temperature for all of the months.

Plot the results as a bar chart.

Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:

Find the average daily atmospheric pressure of all the months.

Plot the results as a bar chart.

About how many terrestrial (Earth) days exist in a Martian year? To answer this question:

Consider how many days elapse on Earth in the time that Mars circles the Sun once.

Visually estimate the result by plotting the daily minimum temperature.z