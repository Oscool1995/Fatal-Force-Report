Fatal Force: US Police Killings Analysis
https://www.python.org/
https://pandas.pydata.org/
https://plotly.com/

LICENSE
A comprehensive data analysis project exploring fatal police shootings in the United States using The Washington Post's Fatal Force database (2015-2024) , combined with US Census demographic data to examine socioeconomic correlations.

📊 Project Overview

This project analyzes patterns in fatal police shootings across the United States, investigating:
Demographic patterns by race, age, and gender
Geographic distribution across states and cities
Socioeconomic correlations with poverty rates, education levels, and income
Circumstances of shootings (armed status, mental illness indicators, manner of death)
Racial disparities relative to population demographics
The analysis was inspired by The Washington Post's groundbreaking investigation that began tracking these incidents after the 2014 killing of Michael Brown in Ferguson, Missouri , filling a critical gap where federal data was found to undercount shootings by more than half .

🗂️ Data Sources

Primary Dataset
Fatal Force Database: The Washington Post's comprehensive database of every fatal shooting by an on-duty police officer in the line of duty since January 1, 2015 
Records: 10,000+ fatal shootings (2015-2024)
Features: Race, age, gender, armed status, signs of mental illness, fleeing status, location, agency involved
Supplemental Census Data
Median_Household_Income_2015.csv - Median household income by city
Pct_People_Below_Poverty_Level.csv - Poverty rates by geographic area
Pct_Over_25_Completed_High_School.csv - High school graduation rates
Share_of_Race_By_City.csv - Racial demographics by city
Source: US Census Bureau

🔧 Technical Stack

Python 3.7+
Data Manipulation: Pandas, NumPy
Visualization:
Plotly Express (interactive charts)
Seaborn (statistical plots)
Matplotlib (custom visualizations)
Analysis: Collections, statistical correlation

📈 Key Analyses & Visualizations

1. Socioeconomic Patterns
State-by-state poverty rate rankings
High school graduation rate analysis
Correlation between poverty and education (dual-axis charts, joint plots, regression analysis)
2. Demographic Analysis
Racial makeup visualization by state (stacked bar charts)
Age distribution analysis with histograms and KDE plots
Gender breakdown of fatalities
Race-specific age distribution patterns
3. Incident Characteristics
Armed Status: Weapon types, armed vs. unarmed percentages
Mental Illness: Prevalence of documented mental health crises
Manner of Death: Box plots analyzing age/gender distributions by death classification
4. Geographic Analysis
Top 10 Cities: Highest concentration of police killings
Choropleth Map: State-by-state fatality distribution
Racial Disparity Heatmap: Comparing killing rates to population proportions in high-incident cities
5. Advanced Insights
Racial disparity ratios (killings proportion vs. population share)
Interactive visualizations with hover details and filtering

🚀 Getting Started
Prerequisites
bash
Copy
pip install pandas numpy plotly seaborn matplotlib
Installation
bash
Copy
git clone https://github.com/yourusername/fatal-force-analysis.git
cd fatal-force-analysis
Usage
Ensure all CSV files are in the working directory:
Deaths_by_Police_US.csv
Median_Household_Income_2015.csv
Pct_People_Below_Poverty_Level.csv
Pct_Over_25_Completed_High_School.csv
Share_of_Race_By_City.csv
Run the analysis script:
bash
Copy
python fatal_force_analysis.py

🎯 Key Findings

Based on the analysis (spoiler alert):
Gender Disparity: Over 95% of victims are male
Age Distribution: More than half of victims are between 20-40 years old 
Racial Disproportionality: Black Americans are killed at more than twice the rate of White Americans relative to population size 
Armed Status: Vast majority of incidents involve armed individuals (guns being most common)
Mental Health: Significant percentage of victims showed signs of mental illness
Geographic Concentration: Certain cities and states show disproportionately high rates

🧹 Data Cleaning Methodology

The project implements robust data cleaning:
Missing Values:
Categorical fields (race, armed, flee) → filled with 'Unknown'
Numerical fields (age, income) → filled with 0 or converted to numeric
Special handling for ' - ' strings in census data
Duplicates: Removed across all datasets
Type Conversion: Ensured proper numeric types for analysis

📊 Sample Visualizations

The project generates multiple interactive charts including:
Interactive bar charts with color scaling
Dual-axis line charts showing poverty vs. education correlations
Stacked bar charts for racial demographics
Choropleth maps for geographic distribution
Heatmaps for racial disparity analysis
Box plots for age/manner of death analysis
KDE plots for age distribution by race

🤝 Contributing

This project is for educational and research purposes. The original Washington Post data is available under CC BY-NC-SA 4.0 license .
To provide information about fatal police shootings since Jan. 1, 2015, contact The Washington Post at: policeshootingsfeedback@washpost.com

📚 References

The Washington Post - Fatal Force Database 
GitHub - Washington Post Data Repository 
Peabody Award - Fatal Force Recognition 

📄 License

This analysis code is provided under the MIT License. The underlying data belongs to The Washington Post and US Census Bureau under their respective licenses.
🙏 Acknowledgments
The Washington Post for their decade-long commitment to documenting these incidents 
US Census Bureau for demographic data
The open-source Python data science community
Note: This analysis deals with sensitive topics involving loss of life. The data represents real people and should be treated with appropriate respect and context when sharing findings.
