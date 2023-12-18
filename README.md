![Illustration of BeautifulSoup](https://yganalyst.github.io/assets/images/crawling.png)
# Exploring-Mars-with-BeautifulSoup
## Description
I've learned to identify HTML elements on a page by their 'id' and 'class' attributes, and use this knowledge to extract information via both automated browsing with Splinter and HTML parsing with BeautifulSoup. In this project, I will be applying these skills and knowledge to practice. 

First, I used Splinter for automated web-browsing and BeautifulSoup to parse desired information. Subsequently, I stored this information in a Pandas dataframe for data analysis and visualisation. 

## Usage
To see the code for 'Part 1:Scrape Titles and Preview Text from Mars News', please navigate to the 'web_scraping_part1&2' folder and select 'part_1_mars_news.ipynb'.

To see the code, data analysis and visualisations for 'Part 2: Scrape and Analyse Mars Weather Data' of the project, please navigate to the 'web_scraping_part1&2' folder and select 'part_2_mars_news.ipynb'.

To see the output dataframe for 'Part 2: Scrape and Analyse Mars Weather Data', please navigate to the 'web_scraping_part1&2' folder and select 'Output' and choose the 'Mars_temp_df.csv' file. 

## Installations
The following dependencies were imported to run the code:
1. `from splinter import Browser`
2. `from splinter import Browser`

Make sure you have these libraries pre-installed:
1. `!pip install splinter selenium`
2. `!pip install beautifulsoup4`

## Mars information scraping with BeautifulSoup
Below is a list of dictionaries, holding information about the title and preview text of each article retrieved as from `https://static.bc-edx.com/data/web/mars_news/index.html`:
![Alt text](<Screenshot 2023-12-18 at 2.12.39 pm.png>)

HTML elements were scraped and converted into a Pandas table (shown below):
![Alt text](<Screenshot 2023-12-18 at 2.18.12 pm.png>)

Here’s an explanation of the column headings:

* `id`: the identification number of a single transmission from the Curiosity rover
* `terrestrial_date`: the date on Earth
* `sol`: the number of elapsed sols (Martian days) since Curiosity landed on Mars
* `ls`: the solar longitude
* `month`: the Martian month
* `min_temp`: the minimum temperature, in Celsius, of a single Martian day (sol)
* `pressure`: The atmospheric pressure at Curiosity's location

Specifically, we wanted to answer these questions:
* How many months exist on Mars?
* How many Martian (and not Earth) days worth of data exist in the scraped dataset?
* What are the coldest and the warmest months on Mars (at the location of Curiosity)? Plot the results in a bar chart
* Which months have the lowest and the highest atmospheric pressure on Mars? Plot the results in a bar chart.
* About how many terrestrial (Earth) days exist in a Martian year? 
1. How many days elapse on Earth in the time that Mars circles the Sun once.
2. Visually estimate the result by plotting the daily minimum temperature.

The bar graph below depicts Mars's temperatures and pressures by month:
![Alt text](<Screenshot 2023-12-18 at 2.21.26 pm.png>)

![Alt text](<Screenshot 2023-12-18 at 2.24.10 pm.png>)

To know how many terrestrial (Earth) days exist in a Martian year, I generated the plot below:
![Alt text](<Screenshot 2023-12-18 at 2.26.06 pm.png>)

From the plot, the distance from peak to peak is roughly 1083 - 440 = 643 days. In 1 Martian year, there're about 643
terrestrial days.

## Credits
Special thanks to the folloiwng individuals for their contribution:

-AskBCS learning assistants

-Jefferery Chieh-Liu (TA)


