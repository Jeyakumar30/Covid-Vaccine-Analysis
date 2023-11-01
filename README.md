COVID Vaccine Analysis

This README file provides an overview of the code for analyzing COVID vaccination data. The code includes data loading, preprocessing, and visualization to gain insights into global vaccination efforts. This project aims to comprehensively analyze Covid-19 vaccine data, specifically concentrating on vaccine effectiveness, distribution patterns, and adverse reactions. The primary objective is to generate actionable insights to assist policymakers and healthcare entities in enhancing their vaccination deployment strategies. 

Contributers:

Jeyakumar N K

Dinesh Babu P K

Mohamed Arsath T

Yashwanth  J A

Prithivi Raj S D

1. Introduction
This project involves the analysis of COVID-19 vaccination data using Python and various data analysis libraries. The analysis is performed on two datasets: one containing information about vaccine manufacturers, and the other containing country-level vaccination data.

Data Sources:
The project utilizes two primary data sources:
- [country_vaccinations_by_manufacturer.csv](https://raw.githubusercontent.com/Jeyakumar30/NM-Project/main/country_vaccinations_by_manufacturer.csv): Data on vaccine manufacturers.
- [country_vaccinations.csv](https://raw.githubusercontent.com/Jeyakumar30/NM-Project/main/country_vaccinations.csv): Country-level vaccination data.

Running the Code in Google Colab

To run the code in Google Colab, follow these steps:

1. Open Google Colab in your web browser.
2. Click on "File" > "New Notebook" to create a new Colab notebook.
3. Copy and paste the code from `vaccine_data_analysis.py` into the Colab notebook.
4. Upload the dataset files `country_vaccinations_by_manufacturer.csv` and `country_vaccinations.csv` to your Google Drive.
5. Mount your Google Drive in the Colab notebook using the following code:

Import the drive module from google.colab

from google.colab import drive

Mount Google Drive at /content/drive
drive.mount('/content/drive')


2. Required Libraries
The code utilizes the following libraries:
NumPy
Pandas
Seaborn
Matplotlib
Plotly Express
Plotly Graph Objects

3. Loading Data Set
The code loads data from two CSV files: country_vaccinations_by_manufacturer.csv and country_vaccinations.csv.

4. Columns Present in Given Data Set
The columns present in the loaded data sets are displayed for reference.
country_vaccinations_by_manufacturer.csv comprises of following columns:
Columns in `country_vaccinations.csv :

- `location`: The location or country where vaccinations are recorded.
- `date`: The date on which vaccination data was reported.
- `vaccine`: The type of vaccine administered.
- `total_vaccinations`: The total number of vaccinations administered on the specified date.

country_vaccinations.csv comprises of following columns:
i) country			
ii) iso_code
iii) date	
iv) total_vaccinations
v) people_vaccinated	
vi) people_fully_vaccinated	
vii) daily_vaccinations_raw	
viii) daily_vaccinations	
ix) total_vaccinations_per_hundred	
x) people_vaccinated_per_hundred	
xi) people_fully_vaccinated_per_hundred	
xii) daily_vaccinations_per_million	
xiii) vaccines	
xiv) source_name	
xv) source_website


5. Shape of DataFrames
The code provides information about the shape of the loaded data frames.
country_vaccinations_by_manufacturer.csv => (35623, 4)
country_vaccinations.csv => (86512, 15)

6. Information About Given Data Sets
Details about the data sets, such as data types and non-null counts, are presented.

7. Vaccines Manufactured on a Particular Date
The code filters and displays vaccines manufactured on a specific date from the manufacturer data set.

8. Country-Wise Vaccination Status on a Particular Date
Similarly, the code filters and displays country-wise vaccination status on a specific date from the vaccination data set.

9. Preprocessing Data
The code performs data preprocessing steps, including handling missing values, dropping duplicates, and filling mean values.

10. Visualization of Data
The code includes various visualizations, such as heatmaps, bar plots, and statistical analyses, to explore and understand the COVID-19 vaccination data.
       

Analysed: 
Heatmap Visualization to check correlation between attributes
![1](https://github.com/Jeyakumar30/NM-Project/assets/121599159/666e079a-8f12-47e9-b44e-3a8fc26e5b46)

Top countries in vaccinations Utilization
![2](https://github.com/Jeyakumar30/NM-Project/assets/121599159/785b6a6c-ac55-4daa-aa21-5a7750ea2cd1)

Type of vaccine utilized Vs Count
![3](https://github.com/Jeyakumar30/NM-Project/assets/121599159/d233ca9f-f5ef-4f05-a2e2-8c736f9fa379)
