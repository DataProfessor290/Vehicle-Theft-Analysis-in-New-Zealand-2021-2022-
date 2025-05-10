# Vehicle Theft Analysis in New Zealand (2021-2022)

## 📜 Project Overview

This project analyzes vehicle theft patterns in New Zealand for the years 2021 and 2022. By leveraging a relational dataset that includes vehicle theft incidents, vehicle make details, and geographical location data, the goal is to uncover key insights and trends that can help in preventing vehicle thefts. This analysis aims to provide actionable recommendations for both car owners and authorities to mitigate theft risks.

### Objectives:
1. **Analyze Theft Trends Over Time**: Identify high-theft periods, seasonal fluctuations, and yearly patterns.
2. **Vehicle-Level Profiling**: Analyze theft patterns based on make, model, year, color, and type of vehicle.
3. **Geographic Risk Assessment**: Assess theft distribution across various locations and regions.
4. **Data Cleaning & Wrangling**: Handle missing values and ensure data integrity.
5. **Generate Practical Insights**: Provide actionable recommendations to prevent vehicle theft.

---

## 🔢 Data Sources

The dataset consists of three main components:

1. **Vehicle Theft Data**: Core records of theft incidents including vehicle ID, date of theft, and vehicle details (make, model, color).
2. **Make Detail**: Metadata about each vehicle, including make, model, and type.
3. **Location Data**: Geographical and jurisdictional information about each theft, such as region, country, and population density.

### Data Range:
- **Time Period**: 2021-2022
- **Location**: New Zealand

---
## 🧑‍💻 Data Cleaning & Wrangling

Data cleaning and preparation are essential to ensure that the analysis is based on high-quality data. Here are the key steps taken during the cleaning process:

1. **Missing Data**: We identified columns with missing values and handled them appropriately:
   - For categorical data, missing values were filled with the string "NA".
   - For numeric columns, missing values were filled with the median value of the respective columns.

2. **Duplicate Data**: After checking for duplicate rows, we confirmed that no duplicates were found.

3. **Column Standardization**: Column names were stripped of any extra spaces to ensure consistency across the dataset.

4. **Date Handling**: The `date_stolen` column was converted to a proper `datetime` format. We also created additional columns like `month`, `day`, and `year` for more granular analysis.

---

## 📊 Key Findings

Based on the data analysis, several key trends and insights were identified:

### 1. Theft Trends Over Time 📅
- **Yearly Increase**: There was a significant rise in thefts from 1,668 in 2021 to 2,885 in 2022, signaling a growing issue.
- **Monthly Patterns**: March saw the highest number of thefts with 1,053 incidents, possibly due to seasonal factors. April had the lowest with only 329 incidents.

### 2. Weekly Theft Patterns 📆
- **Most Active Day**: Mondays saw the most thefts (767 incidents), potentially due to lower vigilance at the beginning of the week.
- **Least Active Day**: Saturdays recorded the least thefts, likely because of increased public activity and better security on weekends.

### 3. The Most Stolen Makes and Models 🚗
- **Top Makes**: Toyota was the most stolen make, followed by Nissan and Trailer.
- **Top Models**: Vehicles from the mid-2000s (2005-2006) were most frequently targeted, likely due to their age and lower security features.

### 4. Popular Car Colors 🎨
- **Most Stolen Colors**: Silver was the most stolen color, followed by white and black.
- **Least Stolen Colors**: Gold, brown, and yellow cars were targeted the least.

### 5. Regional Risk Distribution 🌍
- **Auckland**: This region recorded the highest number of thefts, with 1,638 incidents.
- **Other High-Risk Areas**: Canterbury and Bay of Plenty also experienced significant thefts, with several other regions showing notable trends.

---

## 💡 Recommendations

Based on the analysis, the following recommendations are proposed to mitigate vehicle theft:

1. **Enhanced Surveillance and Policing in High-Theft Areas 🚓**
   - Regions such as Auckland, Canterbury, and Bay of Plenty should increase police presence and surveillance. Public awareness campaigns should also be launched to educate people about vehicle theft prevention.

2. **Targeted Security Measures for Vulnerable Makes and Models 🔒**
   - Owners of Toyota vehicles and mid-2000s models should consider installing additional security features, such as steering wheel locks, GPS tracking devices, and alarm systems.

3. **Vigilance During Peak Seasons 🎉**
   - The months of January to March and October to December have higher theft rates. Authorities should focus on raising awareness and promoting extra precautions during these months.

4. **Promote Use of Vehicle Identification Technology 🔍**
   - Vehicle owners, especially those with older models (1996-2005), should consider using VIN etching and modern anti-theft technologies to deter thieves.

5. **Encourage Parking Security for Popular Car Colors 🚗**
   - Owners of silver, white, and black cars should be encouraged to park in well-lit areas and use security devices like steering wheel locks and immobilizers.

---

## 📂 Files Included

- **`vehicle_theft_analysis.ipynb`**: Jupyter notebook containing the full analysis and visualizations.
- **`stolen_vehicles.csv`**: Contains vehicle theft incident data.
- **`make_details.csv`**: Contains metadata about vehicle makes and models.
- **`locations.csv`**: Contains location and regional data for each theft.

---

## 🛠️ Tools & Technologies

- **Python**: Programming language used for the analysis.
- **Pandas**: For data manipulation and cleaning.
- **Matplotlib & Seaborn**: Libraries for creating visualizations.
- **Jupyter Notebook**: Interactive environment for running the analysis.

---

## 📑 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
