# Task 01: Python Programming, Data Analysis & Visualization

**Devixo Solutions - AI/ML Internship Program**

**Author:** Wajiha Waqar
**Internship Domain:** AI/ML

---

## Project Objective

The objective of this project is to perform a complete data analysis workflow on a real-world Kaggle dataset, starting from raw data and ending with meaningful conclusions. The project covers data loading, data understanding, data cleaning and preprocessing, exploratory data analysis (EDA), statistical analysis, data visualization, and insight generation.

## Dataset Description

- **Dataset Name:** Laptop Price Dataset
- **Total Records:** 823 originally, **802** after removing 21 duplicate rows
- **Total Columns:** 19
- **Description:** Each row is one laptop listing. The dataset describes the laptop brand, processor, RAM, storage (SSD and HDD), operating system, graphics card memory, warranty, touchscreen and MS Office availability, price, and customer feedback (star rating, number of ratings, number of reviews).
- **Key Columns:** brand, processor_name, ram_gb, ssd, hdd, graphic_card_gb, os, warranty, price, rating, number_of_ratings, number_of_reviews
- **Column types:** 3 numerical (price, number_of_ratings, number_of_reviews), 16 categorical, no date/time columns

## Dataset Source

Kaggle (public dataset, downloaded as a CSV file).

## Technologies Used

- Python 3.x
- Google Colab / Jupyter Notebook
- Git and GitHub

## Libraries Used

- Pandas: data loading, cleaning and analysis
- NumPy: numerical operations
- Matplotlib: data visualization
- Seaborn: statistical visualization

## Project Workflow

1. Dataset selection
2. Data loading
3. Data understanding (shape, data types, column types)
4. Data cleaning (missing values, duplicates, data types, renaming columns, invalid values)
5. Exploratory data analysis (value counts, outliers, group averages)
6. Statistical analysis (mean, median, mode, standard deviation, variance, correlation)
7. Data visualization (10 charts)
8. Insights and findings
9. Conclusion
10. Project documentation and GitHub organization

## Data Cleaning Summary

- **Missing values:** none found in any of the 19 columns (0%), so no imputation was needed
- **Duplicates:** 21 duplicate rows found and removed (823 rows to 802 rows)
- **Data types:** the 16 text columns were converted to the category type; numerical columns were already correct
- **Invalid values:** no negative or impossible values were found
- **Renamed columns:** Touchscreen to touchscreen, Price to price, Number of Ratings to number_of_ratings, Number of Reviews to number_of_reviews

## Visualizations Created

Histogram, bar chart, pie chart, scatter plot, line chart, box plot, correlation heatmap, count plot, pair plot, and violin plot. All images are saved in the `images/` folder.

## Major Findings

1. Laptop prices are right-skewed: the mean price is 76,625.54 while the median is 63,990, and 49 laptops are price outliers (above 154,827.5).
2. APPLE has the highest average price (157,081.30) and Avita the lowest (56,346.50).
3. ASUS has the most listings (243 laptops, 30.3%); ASUS, DELL, Lenovo and HP together make up about 84% of the dataset.
4. 8 GB is the most common RAM size (404 laptops, 50.4%), and average price rises with RAM size.
5. Number of ratings and number of reviews are almost perfectly correlated (0.99), while price has only weak negative correlations with them (-0.15 and -0.16).

The full list of 12 insights is available in the PDF report.

## Project Structure

```
Devixo-Solutions-Task-01/
|-- dataset/
|   |-- (laptop dataset CSV file)
|-- notebook/
|   |-- Task_01_Data_Analysis.ipynb
|-- images/
|   |-- visualization_01.png ... visualization_10.png
|-- report/
|   |-- Task_01_Report.pdf
|-- README.md
```

## How to Run the Project

**1. Clone the repository**

```
git clone https://github.com/wajihawaqar903-cpu/Devixo-Solutions-Task-01.git
cd Devixo-Solutions-Task-01
```

**2. Install the required libraries**

```
pip install pandas numpy matplotlib seaborn jupyter
```

**3. Run the notebook**

Open `notebook/Task_01_Data_Analysis.ipynb` in Jupyter Notebook or upload it to Google Colab, upload the dataset CSV from the `dataset/` folder when asked, and run all cells in order.

## Report

The complete PDF report is available in the `report/` folder (`Task_01_Report.pdf`).

## Author

**Wajiha Waqar**
BS Robotics and Intelligent Systems, NUML Islamabad
AI/ML Intern, Devixo Solutions
GitHub: https://github.com/wajihawaqar903-cpu
