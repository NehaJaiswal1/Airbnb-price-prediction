🏡 Airbnb Data Analysis Project
📌 Project Overview

This project explores an Airbnb dataset by performing data cleaning, preprocessing, and exploratory data analysis (EDA).
The goal is to understand patterns in pricing, reviews, and property distribution, and to prepare the dataset for further analysis or modeling.

❓ Project Questions & Answers
Q1. What is the objective of this project?

👉 The main objective is to analyze Airbnb listings to identify:

Pricing trends

Host and property details

Patterns in reviews

Popular neighborhoods

Q2. What dataset is used?

👉 The dataset used is airbnb_dataset.csv, which contains information about Airbnb listings such as:

name, host name

neighbourhood

room type

price, service fee

reviews per month, last review

Q3. How did you clean the data?

👉 Steps taken for cleaning:

Checked for missing values using df.isnull().sum().

Converted date columns (e.g., last review) to datetime.

Filled missing values in:

reviews per month → 0

last review → minimum date available

Dropped rows with missing name or host name.

Removed unnecessary columns (license, house_rules).

Converted price and service fee from strings ($) to float.

Removed duplicates.

Q4. What kind of analysis did you perform?

👉 Performed Exploratory Data Analysis (EDA):

Distribution of room types.

Average price per neighborhood.

Relationship between reviews and price.

Hosts with the highest number of listings.

Service fee analysis.

Q5. What visualizations are included?

👉 Using Matplotlib & Seaborn, the following plots are created:

Bar plots of room type distribution.

Boxplots of price vs room type.

Heatmaps for correlation between variables.

Line plots for reviews over time.

Q6. What insights did you gain?

👉 Key insights:

Some neighborhoods have much higher prices compared to others.

Private rooms are the most common room type, but entire homes generate higher revenue.

Listings with frequent reviews are often moderately priced.

Service fees contribute significantly to the final cost.

Q7. Tools & Libraries used?

👉

Python

Pandas, NumPy (data cleaning & analysis)

Matplotlib, Seaborn (visualization)

Q8. How can someone run this project?

Clone this repository:

git clone https://github.com/yourusername/airbnb-analysis.git


Install dependencies:

pip install pandas numpy matplotlib seaborn


Run the Jupyter Notebook:

jupyter notebook Airbnb.ipynb

📊 Conclusion

This project demonstrates data wrangling, cleaning, and exploratory data analysis (EDA) on Airbnb listings. It provides useful business insights into pricing, hosts, and customer reviews, which can be extended into predictive modeling (e.g., price prediction or demand forecasting).
