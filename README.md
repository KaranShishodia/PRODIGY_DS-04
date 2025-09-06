# PRODIGY_DS-04

# US Traffic Accidents Data Analysis

This project performs an exploratory data analysis (EDA) on the **US Accidents** dataset from Kaggle. The primary goal is to identify patterns and contributing factors related to traffic accidents across the United States, focusing on road conditions, weather, and time of day.

---

##  Project Objectives

* **Data Preparation**: Clean the raw dataset by handling missing values and converting data types.
* **Time-Based Analysis**: Analyze accident trends based on the time of day, day of the week, and month.
* **Weather Conditions**: Explore the relationship between weather conditions and accident frequency.
* **Geospatial Analysis**: Visualize accident hotspots to identify high-risk areas.
* **Contributing Factors**: Uncover other factors like road features and visibility that may influence accident occurrence.

---

##  Key Findings

* **Rush Hour Accidents**: A significant number of accidents occur during morning and evening rush hours.
* **Weather Impact**: Adverse weather conditions, such as rain and fog, are strongly correlated with an increase in accidents.
* **Day of the Week**: Weekdays typically have more accidents than weekends.
* **Accident Hotspots**: High-density urban areas and major highways show a concentrated number of accidents.

---

##  How to Run the Project

### 1. Prerequisites
Ensure you have Python installed. It is recommended to use a virtual environment.

### 2. Get the Dataset
The dataset is too large to be included in the repository. Please download the `US_Accidents_March23.csv` file from the [Kaggle dataset page](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents) and place it in a new `data` directory within the project folder.

### 3. Installation
Install the required Python libraries using the `requirements.txt` file.
```bash
pip install -r requirements.txt

OUTPUT
 Accidents by Time of Day (Refined):

plt.figure(figsize=(15, 8)) # Increased figure size
sns.histplot(df['Hour'], bins=24, kde=False, color='#1f77b4') # Added color
plt.title('Distribution of Traffic Accidents by Hour of Day in the US', fontsize=18) # Larger, clearer title
plt.xlabel('Hour of Day (24-hour format)', fontsize=14) # Clearer label
plt.ylabel('Number of Accidents', fontsize=14) # Clearer label
plt.xticks(range(0, 24), fontsize=10) # Ensure all hours are visible and readable
plt.yticks(fontsize=10)
plt.grid(axis='y', linestyle='--', alpha=0.7) # Improved grid
plt.tight_layout() # Adjust layout to prevent labels from overlapping
plt.show()


