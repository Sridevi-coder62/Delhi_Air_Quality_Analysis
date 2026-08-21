# Delhi_Air_Quality_Analysis

# 🌍 Environmental Monitoring & Pollution Analysis using PySpark

## 📌 Project Overview

This project is a hands-on **Environmental Monitoring and Pollution Analysis** project built using **Apache PySpark**.

The project focuses on processing and analyzing environmental pollution data to identify pollution patterns, highly polluted records, pollution trends, and location-wise pollution statistics.

It demonstrates practical **PySpark DataFrame operations, data transformation, aggregation, statistical analysis, and ETL workflows**.

---

## 🎯 Project Objectives

The main objectives of this project are to:

- Explore environmental pollution data
- Identify unique pollution parameters
- Analyze pollution readings
- Find the highest pollution readings
- Calculate average pollution by location
- Find maximum pollution for each pollutant
- Classify pollution based on severity
- Identify highly polluted locations
- Analyze pollution trends by hour
- Remove duplicate records
- Generate statistical summaries
- Analyze specific pollutants such as PM2.5
- Extract highly polluted records
- Generate a location-wise environmental monitoring report

---

## 🛠️ Technologies & Tools

- **Python**
- **Apache PySpark**
- **Google Colab**
- **Git**
- **GitHub**

---

## 📊 Dataset

The dataset contains environmental pollution readings recorded across different locations and time periods.

### Dataset Columns

| Column | Description |
|---|---|
| `DateTime` | Date and time of the pollution reading |
| `Locations` | Location where the reading was recorded |
| `Parameters` | Type of pollutant being measured |
| `Values` | Pollution measurement value |
| `Units` | Unit of measurement |
| `hour` | Hour extracted from the timestamp |

### Example Pollution Parameters

The dataset contains pollution parameters such as:

- NO
- NO₂
- O₃
- PM2.5
- PM10

> **Note:** The original dataset is not included in this repository because of its large file size. The complete dataset was used during the analysis in Google Colab.

---

# 🔎 Analysis Performed

The project contains multiple practical PySpark analysis tasks.

## 1. Data Loading

Loaded the environmental pollution dataset into a PySpark DataFrame and inspected the dataset structure.


## 2. Data Exploration

Explored the dataset using PySpark DataFrame operations and examined the available columns and records.
<img width="507" height="290" alt="image" src="https://github.com/user-attachments/assets/7e061a0c-cab4-4d73-8339-4d6608f421af" />


## 3. Find Unique Pollution Parameters

Identified all unique pollutants available in the dataset.

<img width="347" height="322" alt="image" src="https://github.com/user-attachments/assets/3d3c0d90-b401-4b2f-834b-8c1d353baf5b" />


## 4. Find Top 10 Highest Pollution Readings

Retrieved the 10 highest pollution readings from the dataset.

<img width="509" height="284" alt="image" src="https://github.com/user-attachments/assets/e95eca1f-71fd-4aea-884f-a82dca378dfb" />


## 5. Average Pollution by Location

Calculated the average pollution reading for each location.

<img width="368" height="200" alt="image" src="https://github.com/user-attachments/assets/63610cc2-1694-4fcb-b490-a77d0495717f" />


## 6. Maximum Pollution per Parameter

Identified the maximum pollution value recorded for each pollutant.

<img width="327" height="297" alt="image" src="https://github.com/user-attachments/assets/1902236e-60a4-41f8-8625-d174dda92fde" />


## 7. Pollution Severity Classification

Created pollution severity categories based on pollution values.

| Pollution Value | Category |
|---|---|
| Greater than 300 | 🔴 High |
| 100 to 300 | 🟠 Medium |
| Below 100 | 🟢 Low |

<img width="519" height="336" alt="image" src="https://github.com/user-attachments/assets/9ab5adc7-2dc9-4089-b4d8-c0e4bb713146" />


## 8. Most Polluted Locations

Analyzed pollution readings by location to identify locations with higher pollution levels.

<img width="334" height="267" alt="image" src="https://github.com/user-attachments/assets/7ed8e847-f88f-4264-acdd-30dfca4fd5bd" />


## 9. Hour-wise Pollution Trend

Calculated average pollution readings for each hour of the day to understand hourly pollution patterns.

<img width="385" height="323" alt="image" src="https://github.com/user-attachments/assets/c868d565-250c-441f-b76a-fee1fdc95905" />


## 10. Rename Columns

Renamed columns where required to make the dataset easier to work with.

For example:

```text
Values → pollution_value

<img width="505" height="302" alt="image" src="https://github.com/user-attachments/assets/1f1585bf-325c-4dc1-8bfc-9b506e95902b" />


11. Remove Duplicate Records

Identified and removed duplicate pollution records using PySpark.

<img width="415" height="291" alt="image" src="https://github.com/user-attachments/assets/b2498573-e379-45a3-a058-328752691080" />


12. Generate Statistical Summary

Generated statistical information for pollution values, including:

Count
Mean
Standard Deviation
Minimum
Maximum

<img width="478" height="230" alt="image" src="https://github.com/user-attachments/assets/279e544c-79f0-4886-96d8-fa690b84c78f" />

13. Pollutant-specific Analysis

Filtered the dataset to analyze records for a specific pollutant such as PM2.5.

<img width="392" height="317" alt="image" src="https://github.com/user-attachments/assets/864a818d-6c7c-4434-af00-335048fd8485" />


14. Save Highly Polluted Records

Filtered pollution readings where:

Values > 300

and saved the resulting records into a separate CSV output.

<img width="629" height="74" alt="image" src="https://github.com/user-attachments/assets/cfae10ae-05e9-4ca1-9543-ed57f6921487" />


15. Environmental Monitoring Dashboard Dataset

Generated a location-wise monitoring report containing:

Average Pollution
Maximum Pollution
Total Records

<img width="846" height="196" alt="image" src="https://github.com/user-attachments/assets/b9a93999-dbf5-4e62-b1cf-1e30a83fe525" />

🧰 PySpark Operations Used

This project provided hands-on practice with several important PySpark DataFrame functions and operations.

select()
filter()
distinct()
groupBy()
agg()
avg()
max()
sum()
count()
orderBy()
withColumn()
withColumnRenamed()
when()
otherwise()
dropDuplicates()
describe()
write.csv()
🔄 ETL Workflow

The project follows a practical ETL-style data processing workflow:

              Raw Pollution Data
                      │
                      ▼
                Load Dataset
                      │
                      ▼
              Data Exploration
                      │
                      ▼
             Data Transformation
                      │
                      ▼
                  Filtering
                      │
                      ▼
                 Aggregation
                      │
                      ▼
             Statistical Analysis
                      │
                      ▼
              Pollution Analysis
                      │
                      ▼
              Report Generation
                      │
                      ▼
                  CSV Output

📈 Final Environmental Monitoring Report

The final analysis generates a location-wise environmental monitoring dataset containing:

Location	Average Pollution	Maximum Pollution	Total Records
Location 1	Calculated value	Maximum value	Record count
Location 2	Calculated value	Maximum value	Record count

This report can be further used for business intelligence and dashboard development using tools such as Power BI or Tableau.

💡 Key Learning Outcomes

Through this project, I strengthened my practical understanding of:

Apache PySpark
PySpark DataFrames
Data filtering
Data transformation
Data aggregation
GroupBy operations
Statistical analysis
Handling duplicate records
Conditional transformations
CSV data processing
ETL workflows
Environmental data analysis
Preparing datasets for reporting and dashboards
📌 Skills Demonstrated
Programming
Python
PySpark
Data Processing
Data Cleaning
Data Transformation
Data Aggregation
Statistical Analysis
ETL
Data Analysis
Pollution Trend Analysis
Location-wise Analysis
Pollutant-specific Analysis
Severity Classification
Tools
Google Colab
Git
GitHub
🔮 Future Improvements

The project can be further enhanced by:

Creating an interactive Power BI dashboard
Adding pollution trend visualizations
Performing detailed time-series analysis
Comparing pollution levels between locations
Adding more environmental parameters
Automating the ETL workflow
Deploying the PySpark pipeline on a cloud platform
Adding predictive analysis for future pollution levels
🎓 Project Purpose

This project was developed as a hands-on learning and portfolio project to strengthen practical skills in PySpark, data analysis, and ETL workflows.

It demonstrates how raw environmental data can be transformed into meaningful analytical datasets that can support reporting and decision-making.

👩‍💻 Author
Sridevi K

BCA Analytics Graduate | Data Analytics Fresher

Technical Interests
Data Analytics
Python
SQL
PySpark
Power BI
Data Visualization
Big Data
ETL
🔗 Connect With Me

GitHub:
https://github.com/Sridevi-coder62

LinkedIn:
https://www.linkedin.com/in/sridevi-k/

⭐ Acknowledgement

This project was created as part of my hands-on learning journey in Data Analytics and Big Data Processing, with a focus on applying PySpark to a real-world environmental monitoring use case.

⭐ If you found this project useful, feel free to explore the notebook and connect with me!
