# Scrape and Analyze Mars Weather Data

## Overview
This project focuses on scraping and analyzing Mars weather data. The challenge involves automating the process of extracting data from a website, cleaning and organizing the data, performing analysis to uncover insights about Martian weather, and visualizing the results. The project demonstrates proficiency in web scraping, data analysis, and visualization techniques.

---

## Tools and Technologies
The following tools and libraries were utilized:

- **Python**: For implementing scraping and data analysis workflows.
- **Splinter**: To automate web browsing and page interaction.
- **Beautiful Soup**: For parsing HTML and extracting targeted data.
- **Pandas**: For data cleaning, transformation, and analysis.
- **Matplotlib**: For creating visualizations of the analyzed data.

---

## Steps and Methodology

### **Step 1: Visit the Mars Temperature Data Website**
- Used Splinter to visit the Mars Temperature Data website: [Mars Temperature Data Site](https://static.bc-edx.com/data/web/mars_facts/temperature.html).
- Inspected the web page using Chrome DevTools to locate and identify elements of interest for scraping.

### **Step 2: Scrape the Weather Data Table**
- Created a Beautiful Soup object to parse the HTML content.
- Extracted rows of weather data from the HTML table and assembled them into a structured format.

### **Step 3: Store Data in a DataFrame**
- Organized the scraped data into a Pandas DataFrame with the following columns:
  - `id`: Transmission ID
  - `terrestrial_date`: Earth date
  - `sol`: Martian day since Curiosity's landing
  - `ls`: Solar longitude
  - `month`: Martian month
  - `min_temp`: Minimum temperature (°C) on Mars
  - `pressure`: Atmospheric pressure on Mars
- Converted data types to appropriate formats (e.g., `datetime`, `int`, `float`).

### **Step 4: Data Analysis**
- Answered the following questions:
  1. **How many months exist on Mars?**
     - Identified 12 unique Martian months.
  2. **How many Martian days' worth of data exist?**
     - Found data for 1,977 Martian days (`sols`).
  3. **What are the coldest and warmest months on Mars?**
     - Calculated the average minimum temperature for each Martian month.
     - Visualized results in a bar chart.
  4. **Which months have the lowest and highest atmospheric pressure?**
     - Analyzed average monthly atmospheric pressure.
     - Visualized results in a bar chart.
  5. **How many terrestrial (Earth) days are in a Martian year?**
     - Estimated 675 terrestrial days based on temperature trends.

### **Step 5: Save the Data**
- Exported the cleaned and analyzed data to a CSV file (`mars_weather_data.csv`) for sharing and further analysis.

---

## Key Insights

### Martian Weather
- The **third month** is the coldest on Mars, while the **eighth month** is the warmest.
- Atmospheric pressure is lowest during the **sixth month** and highest in the **ninth month**.
- A Martian year is approximately **675 Earth days**, as observed from temperature trends.

### Data and Visualization
- Created bar charts to visualize the average minimum temperature and atmospheric pressure by Martian month.
- Plotted daily minimum temperature trends to estimate the length of a Martian year.

---

## Skills Demonstrated

- **Web Scraping:**
  - Automated browsing and HTML extraction using Splinter and Beautiful Soup.
  - Analyzed website structure to locate and extract specific elements.

- **Data Cleaning and Analysis:**
  - Organized raw HTML data into a structured Pandas DataFrame.
  - Converted data types for effective analysis.
  - Performed exploratory analysis to identify trends and answer questions.

- **Data Visualization:**
  - Generated bar charts and line plots using Matplotlib to present insights.
  - Highlighted seasonal variations and long-term trends.
