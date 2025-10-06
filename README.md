# Airbnb Dataset Exploratory Data Analysis (EDA)

This project performs an exploratory data analysis on an Airbnb dataset containing 102,599 listings and 26 features. The analysis covers data loading, cleaning, and visualization to understand the distribution and relationships of key variables.

---

## Data Loading & Cleaning

- The dataset is loaded safely with error handling for malformed lines.
- Missing values in categorical columns are filled with placeholders such as `"Unknown"` or `"Not provided"`.
- Missing numerical values are filled with the median of each respective column.
- Duplicate rows are removed to ensure data integrity.

---

## Visualization

### 1. Univariate Analysis

- **Listings by Neighbourhood Group**  
  A horizontal barplot shows the count of listings across different neighbourhood groups using a pastel color palette for clarity.

- **Price Distribution**  
  A boxplot (log scale) visualizes the price distribution, highlighting the spread and outliers in listing prices with a light blue color.

- **Availability Distribution**  
  Kernel Density Estimate (KDE) plot illustrates the distribution of listing availability (number of days available per year) using a purple color palette.

### 2. Bivariate Analysis

- **Average Price by Neighbourhood Group**  
  A pointplot presents the average price across neighbourhood groups, using the viridis palette for a visually appealing gradient.

- **Number of Reviews vs Price**  
  A hexbin plot shows the relationship between the number of reviews and listing prices, with a plasma colormap to highlight data density and trends.

### 3. Correlation Heatmap

- A heatmap of numerical features’ correlations, colored with a green-blue (`YlGnBu`) palette, helps identify key relationships between variables.

---

## Usage

Run the Python scripts sequentially to:

1. Load and clean the dataset.
2. Generate the visualizations for insights on listings distribution, pricing, reviews, and availability.
3. Explore correlations between numerical features for further analysis or modeling.

---

## Tools & Libraries

- Python (pandas, numpy)
- Visualization: matplotlib, seaborn

---

## Conclusion

This EDA provides a comprehensive overview of the Airbnb listings dataset, highlighting important patterns and outliers that can inform further predictive modeling or business decisions.

---

