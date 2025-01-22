# Zomato Exploratory Data Analysis (EDA)

This repository contains an in-depth exploratory data analysis of Zomato restaurant data. The project aims to uncover the key factors contributing to restaurant success and customer satisfaction, providing actionable insights for restaurant owners, Zomato users, and the broader food and beverage industry.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Data Preprocessing](#data-preprocessing)
4. [Analysis and Visualizations](#analysis-and-visualizations)
5. [Insights and Recommendations](#insights-and-recommendations)
6. [Technologies Used](#technologies-used)
7. [Usage](#usage)
8. [Acknowledgments](#acknowledgments)

---

## Project Overview
Zomato, a global leader in restaurant aggregation and food delivery, operates in over 24 countries. This project analyzes its restaurant data to identify patterns in:
- Location-based trends
- Customer ratings and sentiment
- Price range and cuisine preferences
- Impact of amenities on customer satisfaction

The findings aim to:
- Guide restaurant owners in improving their services.
- Help customers make informed dining decisions.
- Offer Zomato strategies to enhance platform functionality and user satisfaction.

---

## Dataset
The dataset used for this analysis provides detailed information about restaurants, including:
- Names, establishment types, and locations
- Cuisine types and price ranges
- Customer ratings, votes, and reviews
- Service offerings like delivery, dine-in, and takeaway

**Dataset Size**: 211,944 rows and 26 columns

Missing values in key attributes such as `zipcode`, `cuisines`, and `timings` were cleaned and imputed to ensure robust analysis. 

### Access the Dataset
The dataset can be downloaded via this [link](https://drive.google.com/file/d/1HvCHOeh-Z95rX-edVVW_kl8DXpnzjubW/view?usp=drive_link).

---

## Data Preprocessing
1. **Null Value Handling**:
   - Dropped columns with over 5% missing data.
   - Imputed missing values in key columns using statistical methods and logical imputation.
   
2. **Outlier Management**:
   - Outliers in monetary values like `average_cost_for_two` were capped using the IQR method.

3. **Deduplication**:
   - Ensured uniqueness by removing duplicate restaurant entries based on `res_id`.

4. **Feature Engineering**:
   - Created new features like consolidated location data for better analysis.

---

## Analysis and Visualizations
The analysis involved various data visualization techniques to uncover insights, including:
- Distribution of restaurant ratings across cities
- Relationship between price range and ratings
- Popular cuisines and their impact on ratings
- Customer sentiment analysis via word clouds
- Features like delivery and dine-in options affecting ratings

### Key Findings
1. Cities like New Delhi and Bangalore dominate the restaurant landscape with high concentrations.
2. Restaurants offering delivery or dine-in have significantly higher average ratings.
3. Price range correlates positively with restaurant ratings.
4. Popular cuisines include North Indian, Chinese, and Fast Food.

---

## Insights and Recommendations
### For Zomato:
- **Promote High-Rated Restaurants**: Highlight top-rated options to attract customers.
- **Encourage Online Ordering**: Expand online ordering capabilities across restaurants.
- **Support Lower-Priced Restaurants**: Provide resources to improve services in budget segments.

### For Customers:
- **Explore Varied Cuisines**: Try diverse culinary options to discover new favorites.
- **Utilize Amenities**: Look for features like delivery and air conditioning for a comfortable experience.

---

## Technologies Used
- **Python**:
  - Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`, `TextBlob`
- **Visualization Tools**:
  - Heatmaps, scatter plots, bar charts, and word clouds
- **NLP Tools**:
  - Sentiment analysis with TextBlob and word cloud generation

---

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/username/zomato-eda.git
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
3. Access the Dataset: The dataset used in this project can be downloaded via the following [link](https://drive.google.com/file/d/1HvCHOeh-Z95rX-edVVW_kl8DXpnzjubW/view?usp=drive_link).
4. Run the Jupyter Notebook to reproduce the analysis and visualizations.

## Acknowledgments
This project was inspired by the dynamic restaurant industry and Zomato's role in connecting customers to excellent dining experiences. The dataset and analysis provide valuable insights to enhance the industry further.
 
