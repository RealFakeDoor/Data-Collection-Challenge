
Mars Climate Analysis

Overview:
	This project aims to analyze climate data collected by NASA's Curiosity rover 	on Mars. The analysis includes exploring temperature and atmospheric pressure 	variations over Martian months and terrestrial days. The project involves web 	scraping, data cleaning, analysis, and visualization.
The project contains two scripts:

	part_1_mars_news.ipybn- Web scrapes news data, title and preview of all news 	articles on a page, from the Nasa website and exports as Json file.

	part_2_mars_weather.ipybn - Web scrapes temperature and pressure data 	collected by the curiosity rover and analyses the following questions:
		How many months exist on Mars?
	
		How many Martian (and not Earth) days worth of data exist in the scraped dataset?
		
		What are the coldest and the warmest months on Mars (at the location of Curiosity)? 

		Which months have the lowest and the highest atmospheric pressure on Mars?
		
		About how many terrestrial (Earth) days exist in a Martian year? 


Dependencies:
	Python 3
	Pandas
	Matplotlib
	BeautifulSoup
	Splinter (for web scraping)
	
	Chrome Web Browser


Usage:

	Make sure you have installed the required dependencies.

	Run the Python script part_1_mars_news.ipybn

	Run the Python Script part_2_mars_weather.ipybn

Inputs
	Mars Climate Data: 
	The script fetches climate data from two web sources:

	Mars News: 
	Collects news articles related to Mars exploration.

	Mars Temperature Facts: 
	Gathers temperature and atmospheric pressure data.

	Web Scraping: 
	The data is extracted using BeautifulSoup and Splinter from the provided 	URLs.


Logic
	Mars News Scraping: 
	Scrapes news articles related to Mars exploration and 	stores them in a JSON 	file.

	Climate Data Scraping: 
	Extracts temperature and atmospheric pressure data 	from the provided 	website using BeautifulSoup.

	Data Cleaning: 
	Cleans the extracted data and converts it into a structured DataFrame.

	Data Analysis:
	Counts the number of Martian months and Martian days' worth of data.
	Calculates the average low temperature and average pressure by month.
	Plots the average temperature and pressure by month for visualization in ascending order (coldest --> Warmest).
	Estimates the number of terrestrial days in a Martian year.

	Data Export: 
	Writes the cleaned data to a CSV file for further analysis or reporting.

Outputs:
	Mars News Articles: 
		A JSON--- file containing news articles related to Mars exploration.
	
	Cleaned Climate Data: 
		A CSV --- file containing cleaned temperature and atmospheric pressure data.

	Visualizations: 
		Plots showing the average temperature and pressure by month on Mars.
	
	Terrestrial Days Estimation:
	 	A plot indicating the number of terrestrial days in a Martian year.


Results:

Number of Months on Mars: 
	12 months.

Number of Martian Days' Worth of Data: 
	1867 days

Average Low Temperature by Month: 
	On average, the third month has the coldest minimum temperature 
	on Mars, and the eighth month is the warmest. 

Average Pressure by Month: 
	Atmospheric pressure is, on average, lowest in the 
	sixth month and highest in the ninth.

Terrestrial Days in a Martian Year: 
	 The distance from peak to peak is roughly 1480-795 & 795-150. 
	 Which equals 685 days and 645 days, which has an average of 
	 665 days from peak to peak.
	 A year on Mars appears to be about 665 days from the plot.