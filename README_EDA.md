# Zomato Restaurant Dataset — Exploratory Data Analysis (EDA)

## Project Overview
This project explores the Zomato Restaurant Dataset after completing data cleaning and preparation in Task 1 of my internship with **SWYNEX Technologies**. The goal is to calculate descriptive statistics, visualize patterns, identify potential anomalies, and communicate at least five useful insights.

## Objectives
- Understand the dataset structure and key characteristics.
- Analyze restaurant ratings and rating categories.
- Identify cities with the most restaurant listings.
- Find the most frequently listed cuisines.
- Compare ratings across price ranges.
- Examine online delivery and table-booking availability.
- Explore the relationship between average cost for two and restaurant ratings.
- Flag potential cost outliers and validate ratings and vote counts.

## Tools and Libraries
- Python
- Jupyter Notebook in Visual Studio Code
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Dataset
The project uses the cleaned Zomato Restaurant Dataset from Task 1.

The dataset includes information such as restaurant name and ID, country code, city, cuisines, average cost for two, currency, table-booking and online-delivery availability, price range, aggregate rating, rating text, and votes.

The notebook expects the cleaned CSV to be named:

`Zomato_Restaurant_Dataset_Cleaned.csv`

Make sure the CSV is in the notebook's working directory or update the path in the notebook. Check the dataset license before sharing the CSV publicly.

## Suggested Repository Structure

```text
Zomato-Data-Analysis/
├── Zomato_Data_Cleaning.ipynb
├── Zomato_EDA.ipynb
├── Zomato_Restaurant_Dataset_Cleaned.csv
├── README.md
├── restaurant_rating_distribution.png
├── top_10_cities.png
├── top_10_cuisines.png
├── ratings_by_price_range.png
├── online_delivery_distribution.png
├── table_booking_distribution.png
├── cost_vs_rating.png
├── cost_outliers.png
├── top_cities.csv
├── top_cuisines.csv
├── ratings_by_price_range.csv
└── rating_distribution.csv
```

Include only files that exist in your repository. `cost_outliers.png` is optional.

## Analyses Performed

### 1. Dataset Overview
- Inspected dataset dimensions, column names, data types, and descriptive statistics.
- Checked remaining missing values and duplicate records.

### 2. Restaurant Rating Distribution
- Calculated mean, median, minimum, and maximum aggregate ratings.
- Created a histogram to examine rating distribution.

Output: `restaurant_rating_distribution.png`

### 3. Restaurant Listings by City
- Counted restaurant listings by city.
- Visualized the ten cities with the most listings.

Output: `top_10_cities.png`

### 4. Most Common Cuisines
- Split multi-cuisine entries into individual cuisine names.
- Counted cuisine occurrences and visualized the ten most common cuisines.

Output: `top_10_cuisines.png`

### 5. Ratings by Price Range
- Compared the count, mean, and median ratings across price ranges.
- Used a box plot to compare rating distributions.

Output: `ratings_by_price_range.png`

### 6. Online Delivery Availability
- Calculated counts and percentages for online-delivery availability.
- Created a pie chart to visualize the distribution.

Output: `online_delivery_distribution.png`

### 7. Table Booking Availability
- Calculated counts and percentages for table-booking availability.
- Created a pie chart to visualize the distribution.

Output: `table_booking_distribution.png`

### 8. Average Cost for Two vs. Rating
- Calculated average, median, and maximum listed cost.
- Used a scatter plot to explore the association between cost and rating.

Output: `cost_vs_rating.png`

### 9. Potential Anomaly Detection
- Used the interquartile range (IQR) method to flag unusually low or high costs.
- Checked for ratings outside the 0–5 range and negative vote counts.

Output: `cost_outliers.png` (optional)

## Key Insights
Add at least five findings based on the actual output from `Zomato_EDA.ipynb`. For each finding, include the result and a short explanation.

Suggested format:
1. **Restaurant ratings:** [Add your observed rating distribution and what it suggests.]
2. **City listings:** [Add the city with the most listings and its count.]
3. **Popular cuisines:** [Add the most frequently listed cuisine and its occurrence count.]
4. **Price range and ratings:** [Summarize the observed average or median ratings across price ranges.]
5. **Online delivery:** [Add the Yes/No percentages and explain which is more common.]
6. **Table booking (additional):** [Add the Yes/No percentages.]
7. **Cost and ratings (additional):** [Describe the pattern observed in the scatter plot.]

Replace these placeholders with your actual results before submitting. Do not assume a conclusion before inspecting the output.

## Anomaly Notes
- IQR flags identify potential outliers, not automatically incorrect data.
- Costs may use different currencies across countries, so cross-country cost comparisons can be misleading.
- Document any values investigated and whether they were retained or corrected.

## How to Run the Project
1. Download or clone the repository.
2. Open the project folder in Visual Studio Code.
3. Open `Zomato_EDA.ipynb`.
4. Install the required libraries:

   ```bash
   python -m pip install pandas numpy matplotlib seaborn jupyter
   ```

5. Select the Python environment used by the notebook.
6. Ensure the cleaned CSV path in the notebook is correct.
7. Run the notebook cells from top to bottom.

## Conclusion
This EDA project uses descriptive statistics and visualizations to explore restaurant ratings, city listings, cuisines, pricing, and service availability. It also demonstrates basic anomaly detection and the importance of interpreting results in context. Final conclusions should be based on the actual notebook output.

## Internship
**Organization:** SWYNEX Technologies  
**Task:** Task 2 — Exploratory Data Analysis (EDA)

## Author
**Mansi Jain**
