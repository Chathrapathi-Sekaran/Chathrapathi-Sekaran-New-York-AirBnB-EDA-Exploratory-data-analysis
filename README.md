# New York Airbnb Listings EDA Project



## Project Overview
This project performs **Exploratory Data Analysis (EDA)** on New York Airbnb data to uncover trends and patterns in rental listings. Libraries such as **Pandas**, **Numpy**, **Matplotlib**, and **Seaborn** were used for data cleaning, visualization, and analysis.

![](https://github.com/Chathrapathi-Sekaran/Python_Data_cleaning_app/blob/main/DALL%C2%B7E%202024-12-07%2017.19.38%20-%20A%20sleek%20and%20modern%20concept%20design%20for%20a%20data%20cleaning%20application%20in%20Python.%20The%20interface%20features%20a%20clean%2C%20intuitive%20layout%20for%20data%20cleaning%20tasks.webp)

---

## Objective
The goal of this project is to:

- Analyze room types, prices, and availability across different neighborhoods.
- Understand host behavior and listing patterns.
- Detect potential outliers in prices.
- Provide actionable recommendations for both guests and hosts based on insights.

---

## Dataset
The dataset contains **20,765 entries** and **22 features**, including:

- **id**: Unique identifier for each listing.
- **name**: Title of the Airbnb listing.
- **host_name**: Name of the host.
- **neighborhood_group**: Group (borough) where the listing is located.
- **latitude/longitude**: Geolocation of listings.
- **price**: Nightly rental price.
- **room_type**: Type of accommodation (e.g., entire home, private room).
- **reviews_per_month**: Average monthly reviews for the listing.
- **availability_365**: Number of available days in the year.

---

## Steps and Workflow

### 1. Data Cleaning
- **Handle Missing Data**: Columns like `price`, `neighborhood`, and `beds` with null values were handled.
- **Fix Data Types**: Converted `last_review` to a datetime object.
- **Remove Outliers**: Listings with prices > $1,000 were capped to avoid skewed visualizations.

### 2. EDA (Exploratory Data Analysis)

#### Room Type Distribution:
- Visualized the count of each room type using bar plots.
- Identified **Entire home/apt** as the most common room type.

#### Neighborhood Group Insights:
- Analyzed price variations by boroughs.
- **Manhattan** had the highest average prices.

#### Availability Trends:
- Used heatmaps to show correlations among `price`, `availability_365`, `number_of_reviews`, and `beds`.

#### Price Distribution:
- Used histograms to show the distribution of prices.
- Majority of the listings were priced between **$50 - $300**.

#### Host Listings:
- Analyzed hosts with multiple listings using boxplots to identify key contributors.

#### Review Behavior:
- Used pair plots to show relationships between `number_of_reviews`, `price`, and `availability`.

### 3. Data Visualization
- **Pairplot**: To see correlations among `price`, `availability`, and `number_of_reviews`.
- **Heatmap**: Showing correlations among numerical features.
- **Histograms and Boxplots**: To detect outliers in `price`.
- **Bar Charts**: Displaying room types and neighborhood group distributions.

---

## Key Findings and Insights

### Price Trends:
- **Manhattan** has the most expensive listings, followed by **Brooklyn**.
- Entire homes/apartments cost significantly more than private or shared rooms.

### Room Type Distribution:
- Entire homes/apartments are the most common, but private rooms offer budget-friendly options.

### Outliers in Price:
- Few listings priced at $10,000+ were detected, indicating the need to filter such extreme values.

### Availability Patterns:
- Listings with high availability tend to have lower prices and more reviews, likely due to better guest experiences.

### Host Behavior:
- Some hosts manage multiple listings, indicating a trend toward professional hosting.

---

## How to Run This Project

1. **Clone the repository**:
   ```bash
   git clone https://github.com/najirh/Python-Project-P2-New-York-AirBnb-Listing-2024.git
   ```
2. **Install the required libraries**:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. **Run the Jupyter notebook or Python script**:
   ```bash
   jupyter notebook day23_airbnb_eda.ipynb
   ```

---

## Recommendations

### For Guests:
- Look for listings with high availability and good reviews for a better experience.
- **Private rooms in Brooklyn** offer affordable stays compared to Manhattan.

### For Hosts:
- Improve availability and review response rates to attract more bookings.
- Manage pricing effectively to compete within the borough's market.

---

## Future Work

1. Use machine learning to predict prices based on room type and location.
2. Perform sentiment analysis on reviews to better understand guest experiences.
3. Create an interactive dashboard using Plotly or Tableau for live monitoring.

---

## Conclusion
This project offers valuable insights into the New York Airbnb market, helping both guests and hosts make informed decisions. By leveraging EDA techniques, we identified key trends and developed actionable recommendations. Future improvements can involve advanced analytics and predictive modeling to further enhance the findings.
