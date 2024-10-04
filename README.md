# Google Play Store EDA (Exploratory Data Analysis)

## Overview

This repository contains the exploratory data analysis (EDA) conducted on the Google Play Store dataset. The analysis focuses on cleaning the data, deriving insights, and performing statistical tests to explore the relationship between key app metrics such as installs, ratings, and app type (free vs. paid). This analysis is crucial for APPDEV Inc. to make informed business decisions regarding app development and marketing strategies on the Google Play Store.

---

## Dataset

The dataset used in this analysis contains the following columns:
- **App**: Name of the application.
- **Category**: The category of the app.
- **Rating**: Average user rating of the app.
- **Reviews**: Number of user reviews.
- **Size**: Size of the app.
- **Installs**: Number of installs.
- **Type**: Whether the app is free or paid.
- **Price**: Price of the app (for paid apps).
- **Content Rating**: Age group the app is appropriate for.
- **Genres**: Genres of the app.
- **Last Updated**: The date the app was last updated.
- **Current Ver**: Current version of the app.
- **Android Ver**: Minimum required Android version for the app.

---

## Key Steps

### 1. Data Cleaning
- **Handling Missing Data**: Columns with missing values above a threshold of 5% were identified and removed. The remaining columns with few missing values were cleaned by dropping the rows with null values.
- **Removing Duplicates**: Duplicate records were identified and removed from the dataset to ensure accurate analysis.
- **Handling Outliers**: A logarithmic transformation was applied to the "Installs" column to minimize the impact of outliers and present a more meaningful distribution.

### 2. Data Exploration and Visualization
- **Installs Distribution**: A boxplot was created to display the distribution of installs across different app categories, using a log transformation for the number of installs to handle outliers.
- **Reviews vs. Rating**: A scatterplot was used to explore the relationship between the number of reviews and the app ratings, providing insight into user engagement and satisfaction.

### 3. Statistical Hypothesis Testing
- **Paid vs. Free Apps**: A hypothesis test was conducted to determine if there is a statistically significant difference in ratings between free and paid apps. Using a t-test for independent variables:
  - **Null Hypothesis**: There is no significant difference in ratings between paid and free apps.
  - **Alternative Hypothesis**: There is a significant difference in ratings between paid and free apps.

---

## Results and Insights

- **Installs Distribution**: The distribution of installs shows that certain categories such as "Games" and "Productivity" dominate in terms of user base, while niche categories have fewer installs. This insight can inform APPDEV Inc.’s focus areas for app development.
- **Reviews vs. Rating**: A weak correlation was observed between the number of reviews and app ratings. High numbers of reviews do not necessarily translate to better ratings, suggesting that quality rather than quantity of reviews is important.
- **Paid vs. Free Apps**: The t-test revealed that there is no statistically significant difference in the ratings of paid and free apps, suggesting that app cost does not inherently influence user satisfaction.

---

## Conclusion

The analysis provided valuable insights for APPDEV Inc.:
1. **Category Focus**: Targeting high-install categories like "Games" could maximize user acquisition.
2. **Quality Over Quantity**: Focusing on improving app quality rather than just increasing reviews can positively impact app ratings.
3. **Pricing Strategy**: There’s no significant difference in ratings between paid and free apps, so pricing strategies should be based on market conditions rather than the assumption that paid apps will automatically receive higher ratings.

---

## Usage

To reproduce this analysis:
1. Clone the repository.
2. Install required libraries 
3. Run the Jupyter notebook to explore the dataset and perform analysis.

---

## Requirements

- pandas
- matplotlib
- seaborn
- numpy
- scipy

---

## Author

This analysis was conducted by **Dave**, focusing on providing actionable insights for business decisions in the app development industry.

# google_playstore_eda
