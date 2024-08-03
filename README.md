# Air Quality Index (AQI) Analysis and Visualization 
## Overview
This project provides analysis and visualization of Air Quality Index (AQI) data collected from various cities and regions. The primary objective is to understand the variation of air quality over time, identify patterns and trends, and provide insights into the levels of different pollutants. This comprehensive analysis includes data cleaning, processing, and various visualizations.
## Table of Contents
1. [Installation](#installation)
2. [Data Collection](#data-collection)
3. [Data Cleaning](#data-cleaning)
4. [Data Analysis](#data-analysis)
5. [Data Visualization](#data-visualization)
6. [Contributing](#contributing)
7. [License](#license)
8. [Contact](#contact)

## Installation
To set up the project locally, use the following:

    git clone https://github.com/HermelaDev/aqi-analysis.git
    cd aqi-analysis
    pip install -r requirements.txt

## Data Collection
The dataset for this project was obtained from the OpenAQ API, which provides air quality data from around the world. We collected data for multiple cities and pollutants, covering a time range from January 2018 to July 2024. The data was gathered on a monthly basis and includes measurements of various pollutants such as NO2, O3, PM10, and PM2.5.

### Data Collection Process
API Key: To access the data, an API key was required. You can obtain your API key by creating an account on the OpenAQ platform.

API Endpoints: The API endpoints were crafted to fetch average monthly data for different parameters (pollutants) across multiple locations. The key parameters we focused on were:NO2: Nitrogen Dioxide, O3: Ozone, PM10: Particulate Matter (10 micrometers), PM2.5: Particulate Matter (2.5 micrometers)
### Implementation
The data collection was implemented in Python using the requests library for making HTTP requests and pandas for data manipulation.

## Data Cleaning
To ensure the dataset's quality and usability, several data cleaning steps were undertaken. We began by removing duplicate values to avoid redundancy and potential distortion in the analysis. Missing values were addressed through imputation or removal, depending on their extent and impact. We standardized the 'average' values by rounding them to a consistent number of decimal places.

Unnecessary columns, such as 'id', 'parameterId', and 'displayName', were removed to streamline the dataset. The 'months' column was modified to display month names (e.g., 'January', 'February') instead of numerical values, enhancing readability and facilitating time series analysis.

The dataset was reorganized to have pollutants as primary columns, with rows representing different cities and months. Parameters with insufficient data were dropped to maintain the dataset's robustness. Finally, the cleaned dataset was saved in a new CSV file, ready for analysis and modeling. These steps ensured the data was accurate, consistent, and reliable for the subsequent analysis.

## Data Analysis
The data analysis phase involved several key steps to derive meaningful insights from the dataset. First, we calculated the Air Quality Index (AQI) using the provided pollutant concentrations for each location and month. This was essential to quantify the air quality levels in a standardized manner.

Next, we conducted summary statistics to understand the central tendency, dispersion, and distribution of the data. This included calculating mean, median, standard deviation, and range for each parameter, providing a comprehensive overview of the dataset's characteristics.

We then analyzed yearly trends in air quality, examining how AQI and individual pollutant levels varied over time. This analysis was crucial for identifying patterns, seasonal variations, and potential long-term improvements or deteriorations in air quality. Additionally, we explored correlations between different pollutants, offering insights into their interrelationships.

Overall, this data analysis provided a thorough understanding of the air quality patterns in the studied regions, laying the foundation for further modeling and visualization.

## Data Visualization

Data visualization was a crucial component of our project, enabling us to interpret and communicate the findings effectively. We employed various visualization techniques to explore and present the data insights:

- **Trends of Each Parameter AQI and Overall AQI Throughout the Years:** We visualized the trends of each pollutant's AQI over the years, along with the overall AQI. This helped us understand variations across different cities and identify long-term trends in air quality.

- **Parameter Trends Within a City:** By analyzing the trends of specific parameters within a city, we could identify which pollutants had the most significant impact on air quality. This comparison was essential for understanding local environmental challenges and prioritizing mitigation efforts.

- **Monthly Variations:** We plotted the monthly variations of AQI across the cities to highlight seasonal patterns and fluctuations in air quality. This analysis was useful for understanding how different times of the year influenced pollution levels.

- **Line Plots for Average AQI Trends:** Line plots were used to visualize the average AQI trends throughout the years. This provided a clear view of the overall air quality trajectory and highlighted any significant changes or anomalies.

- **Insight into 2023 Trends:** A focused analysis of the AQI trends in 2023 was conducted to understand the most recent air quality conditions and compare them with previous years.

- **Monthly AQI Variation Throughout the Years:** We explored how AQI varied on a monthly basis across multiple years. This helped us identify recurring patterns and potential outliers in the data, offering insights into the temporal dynamics of air quality.

These visualizations were instrumental in conveying complex data insights in an intuitive and accessible manner, making it easier to draw actionable conclusions and inform decision-making.

## Contributing
We welcome contributions! Please fork the repository, create a new branch, and submit a pull request with detailed descriptions of your changes.

## License
This project is licensed under the MIT License. For more details, see the [LICENSE](https://github.com/HermelaDev/Python_class_project/blob/main/LICENSE) file.

## Contact
For questions or inquiries, please contact [@HermelaDev](https://github.com/HermelaDev), [@abogejacob](https://github.com/jacobaboge) and [@HarinaChohan](https://github.com/HarinaChohan).
