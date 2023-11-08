# Module11 Challenge

Part 1 : Scrape Titles and Preview Text from Mars News

STEP 1 -  a) Import Splinter and BeautifulSoup to scrape the elements from the website. 

		b) Use automated browsing to visit the Mars news site. Inspect the page to identify the elements to scrape.

STEP 2 - a) Scrape the website. Create a beautiful soap object(soup_obj). Extract all the text elements. 
			text_elements = soup_obj.find_all('div', class_='list_text')
		
STEP 3 - Store the results. 
	      a) Store each title-and-preview pair in a Python dictionary. And, give each dictionary two keys: title and preview 
	      b) Store all the dictionaries in a Python list
	      c) Print the list in your notebook
			

Finally quit the browser

Part 2: Scrape and Analyze Mars Weather Data

1. Use automated browsing to visit the Mars Temperature Data Site

2. Create a Beautiful Soup object and use it to scrape the data in the HTML table. 

3. Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:

id: the identification number of a single transmission from the Curiosity rover
terrestrial_date: the date on Earth
sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
ls: the solar longitude
month: the Martian month
min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
pressure: The atmospheric pressure at Curiosity's location

4. Examine the data types that are currently associated with each column. Convert the data to the appropriate datetime, int, or float data types.

5. Analyze your dataset by using Pandas functions to answer the following questions:
	a) How many months exist on Mars? 
	b) How many Martian (and not Earth) days worth of data exist in the scraped dataset?
	c) What are the coldest and the warmest months on Mars (at the location of Curiosity)? 
		Find the average minimum daily temperature for all of the months.
		Plot the results as a bar chart.
	d) Which months have the lowest and the highest atmospheric pressure on Mars? 
		Find the average daily atmospheric pressure of all the months.
		Plot the results as a bar chart.
	e) About how many terrestrial (Earth) days exist in a Martian year? 
		Consider how many days elapse on Earth in the time that Mars circles the Sun once.
		Visually estimate the result by plotting the daily minimum temperature.

6. Export the DataFrame to a CSV file.

 
