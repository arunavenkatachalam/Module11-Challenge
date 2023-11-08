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
			

Finally quit the browser.

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
	a) How many months exist on Mars? - Using groupby and count fuction we can get the months exist on mars.
	b) How many Martian (and not Earth) days worth of data exist in the scraped dataset? - We can get the answer by using count function.
	c) What are the coldest and the warmest months on Mars (at the location of Curiosity)? 
  		 1) Find the average minimum daily temperature for all of the months - With groupby function we can find the minimum temperature for all months. Then we have to sort it in ascending order(sort 		    the temperature in coldest to warmest). Looking at the data we can see the coldest temperature is in the month of march(3) with the temperature -83.307292 and warmest temperature is in the 		    month of August(8) with the temperature -68.382979.
		 2) Plot the results as a bar chart.- Bar chart has been ploted to visually show the temperature based on the months 
	d) Which months have the lowest and the highest atmospheric pressure on Mars? 
		1) Find the average daily atmospheric pressure of all the months - With groupby function we can find the Average pressure for all months. Then we have to sort it in ascending order(sort 		    	   the pressure in lowest to highest). Looking at the data we can see the lowest pressure is in the month of June(6) with the pressure 745.054422 and highest pressure is in the 		   		   month of September(9) with the pressure 913.305970.
		2) Plot the results as a bar chart - Bar chart has been ploted to visually show the pressure based on the months 
	e) About how many terrestrial (Earth) days exist in a Martian year?  - Plot the graph to visually represent the Earth days exist in martian year
   		1) Consider how many days elapse on Earth in the time that Mars circles the Sun once.
		2) Visually estimate the result by plotting the daily minimum temperature.
   
7. Export the DataFrame to a CSV file.

 
