# Mars Weather Data Analysis

This project involves analyzing weather data collected by the Curiosity rover on Mars. The analysis focuses on understanding temperature variations and atmospheric conditions on Mars, including identifying the coldest and hottest months, and calculating the number of Earth days in a Martian year.

## Project Overview

The main objectives of this project are:
- To calculate the average minimum temperature by Martian month.
- To identify the coldest and hottest months at Curiosity's location on Mars.
- To calculate the number of terrestrial (Earth) days in a Martian year.

## Data

The data used in this analysis includes:
- `id`: The identification number of a single transmission from the Curiosity rover.
- `terrestrial_date`: The date on Earth corresponding to the rover's transmission.
- `sol`: The number of elapsed sols (Martian days) since Curiosity landed on Mars.
- `ls`: The solar longitude.
- `month`: The Martian month.
- `min_temp`: The minimum temperature in Celsius for a single Martian day (sol).
- `pressure`: The atmospheric pressure at Curiosity's location.

### Data Source

The data was scraped from a web page containing tabular information about Martian weather conditions.

## Analysis Steps

1. **Data Extraction**: The data was scraped from the web using BeautifulSoup and Splinter, and then cleaned and stored in a Pandas DataFrame.
2. **Data Processing**: The data types were corrected for accurate analysis, including converting dates and numerical values to appropriate types.
3. **Temperature Analysis**:
   - The average minimum temperature by month was calculated.
   - A plot was created to visualize the average minimum temperature by Martian month.
   - The coldest and hottest months were identified based on the sorted temperature data.
4. **Martian Year Calculation**:
   - The number of terrestrial (Earth) days in a Martian year was calculated by finding the difference in Earth days between the first and last sol in the dataset.
5. **Data Export**: The processed data was saved to a CSV file for further analysis or sharing.

## Findings

- **Coldest and Hottest Months**:
  - The coldest month at Curiosity's location is Martian month 3, with an average minimum temperature of approximately -83.3°C.
  - The hottest month is Martian month 8, with an average minimum temperature of approximately -68.4°C.
  
- **Number of Earth Days in a Martian Year**:
  - The calculated number of Earth days in a Martian year based on the dataset is approximately 687 days.

## Visualizations

The analysis includes a plot of the average minimum temperature by Martian month, providing a visual representation of seasonal temperature changes on Mars.

## Reproducing the Analysis

To reproduce the analysis, follow these steps:

1. **Set Up the Environment**:
   - Install the required Python libraries: `pandas`, `beautifulsoup4`, `splinter`, `matplotlib`.
   - Ensure you have a compatible web driver for Splinter (e.g., ChromeDriver).

2. **Run the Scripts**:
   - Use the provided scripts to scrape the data, perform the analysis, and generate visualizations.

3. **View the Results**:
   - The final results, including the analysis and plots, are displayed within the notebook and saved as CSV files.

## Dependencies

- Python 3.x
- Pandas
- BeautifulSoup4
- Splinter
- Matplotlib
-
