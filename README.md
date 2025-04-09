# 🏠 California Housing Data Analysis Project

This project explores the **California Housing dataset** from the 1990 U.S. Census. It provides valuable insights into the housing landscape across California by analyzing factors like income, population, housing age, and geographical attributes. The project highlights key data analysis techniques such as data cleaning, visualization, and basic feature engineering — making it ideal for showcasing entry-level data analyst skills.

---

## 📊 Dataset Overview

The dataset contains **20,640 records**, each representing a block group (smallest census unit with ~1,425 residents). It includes **10 features** describing housing, demographic, and geographic variables:

| Feature             | Type        | Description                                |
|---------------------|-------------|--------------------------------------------|
| `longitude`         | Continuous  | Geographic coordinate                      |
| `latitude`          | Continuous  | Geographic coordinate                      |
| `housing_median_age`| Discrete    | Median age of houses in the block group    |
| `total_rooms`       | Discrete    | Total number of rooms                      |
| `total_bedrooms`    | Discrete    | Total number of bedrooms                   |
| `population`        | Discrete    | Population in the block group              |
| `households`        | Discrete    | Number of households                       |
| `median_income`     | Continuous  | Median income of residents                 |
| `median_house_value`| Discrete    | Median house price                         |
| `ocean_proximity`   | Categorical | Location category relative to the ocean    |

---

## 🔍 Key Questions & Analysis

### 1. **What is the distribution of median income?**
- Used histograms to visualize.
- **Insight:** Positively skewed — higher incomes are less frequent.

### 2. **What does the distribution of housing age look like?**
- Histogram analysis with skewness calculation.
- **Insight:** Near-symmetrical distribution (skew ≈ 0.06).

### 3. **How does income relate to housing prices?**
- Scatter plot between `median_income` and `median_house_value`.
- **Insight:** Strong positive correlation observed.

### 4. **How was missing data handled?**
- Deleted rows with missing `total_bedrooms`.
- Alternatively, imputed missing values with column mean.

### 5. **How were central tendencies used?**
- Created custom function to calculate median values across variables.

### 6. **What geographical patterns emerge?**
- Plotted `latitude` vs `longitude`.
- **Insight:** Locations with similar coordinates share housing patterns.

### 7. **What's different near the ocean?**
- Filtered dataset by `ocean_proximity = 'Near Ocean'`.
- Calculated average and median income for this subset.

### 8. **Can we categorize bedroom sizes?**
- Engineered a new feature: `total_bedroom_size` with categories:
  - `Small`, `Medium`, `Large` based on bedroom count.

---

## 📌 Conclusion

This project demonstrates:

- 📂 **Data Cleaning**: Handling missing values using deletion and imputation.
- 📊 **Data Visualization**: Histograms, scatter plots, and geographic maps.
- 🛠️ **Feature Engineering**: Creating custom categories and median value functions.
- 📈 **EDA**: Drawing insights from patterns and correlations.

Overall, this analysis provides a strong foundation for understanding housing data trends and applying key data analyst skills using Python.

---

## 🛠️ Tools & Libraries

- Python (Pandas, NumPy)
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 📁 Project Structure

# California-Housing-Explorer
