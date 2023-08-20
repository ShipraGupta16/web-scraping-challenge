# web-scraping-challenge

This challenge is about full web-scraping and data analysis from Mars Weather Data. It consists of two technical products. Following are the deliverables:

Deliverable 1: Scrape titles and preview text from Mars news articles.

Deliverable 2: Scrape and analyze Mars weather data, and cleans, visualizes and analyzes the data which exists in a table.

These are the step-by-step desciptions on the written code:

### 1: Scrape Titles and Preview Text from Mars News

a) Used automated browsing to visit the Mars news siteLinks to an external site. Inspected the page to identify which elements to scrape.

b) Created a Beautiful Soup object and used it to extract text elements from the website.

c) Extracted the titles and preview text of the news articles that was scraped. Stored the scraping results in Python data structures as follows:

d) Stored each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. An example is the following:

`{'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm", 
 'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."}`

e) Stored all the dictionaries in a Python list.

f) Printed the list in the notebook.

g) Stored the scraped data in a file. Exported the scraped data to a mars_article.json file.

### 2: Scrape and Analyze Mars Weather Data

a) Used automated browsing to visit the Mars Temperature Data SiteLinks to an external site. Inspected the page to identify which elements to scrape. The URL is https://static.bc-edx.com/data/web/mars_facts/temperature.html.

b) Created a Beautiful Soup object and used it to scrape the data in the HTML table. (Note that this can also be achieved by using the Pandas read_html function.) Beautiful Soup was used here to continue sharpening web scraping skills.

c) Assembled the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:

`id`: the identification number of a single transmission from the Curiosity rover <br>
`terrestrial_date`: the date on Earth <br>
`sol`: the number of elapsed sols (Martian days) since Curiosity landed on Mars <br>
`ls`: the solar longitude <br>
`month`: the Martian month <br>
`min_temp`: the minimum temperature, in Celsius, of a single Martian day (sol) <br>
`pressure`: The atmospheric pressure at Curiosity's location <br>

d) Examined the data types that are currently associated with each column. Converted the data to the appropriate datetime, int, or float data types as needed.

e) Analyzed the dataset by using Pandas functions to answer the following questions:

	- How many months exist on Mars?
	- How many Martian (and not Earth) days worth of data exist in the scraped dataset?
	- What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
	- Find the average minimum daily temperature for all of the months.
	- Plot the results as a bar chart.
	- Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
	- Find the average daily atmospheric pressure of all the months.
	- Plot the results as a bar chart.
	- About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
	- Consider how many days elapse on Earth in the time that Mars circles the Sun once.
	- Visually estimate the result by plotting the daily minimum temperature.

f) Exported the DataFrame to a mars_weather.csv file.

