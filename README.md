# Sephora Beauty Product Review Analytics

## Project Overview

This project explores **customer satisfaction patterns in beauty products sold on Sephora** by analyzing product reviews, ratings, and brand performance. The goal is to understand **what factors drive higher customer satisfaction**, such as brand reputation, product category, and customer engagement through reviews.

The project is divided into two main components:

1. **Exploratory Data Analysis in Python (Jupyter Notebook)**

   * Data cleaning and manipulation using **Pandas**
   * Exploratory analysis and visualizations using **Matplotlib** and **Seaborn**

2. **Interactive Dashboard in Tableau**

   * A business-focused dashboard summarizing key metrics and insights
   * Visual exploration of brand performance, category ratings, and market dominance

Together, these components demonstrate an end-to-end data workflow from **data preparation → exploratory analysis → business intelligence visualization**.


# Dataset

The dataset contains product review information from **Sephora beauty products**, including:

* Brand name
* Product name
* Product category
* Price
* Customer rating
* Number of reviews
* Skin type
* Skin tone
* Recommendation indicators

The dataset represents **2,351 products across 142 brands** with millions of aggregated customer reviews.


# Part 1 — Data Cleaning & Exploration (Python)

## Tools Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

## Data Cleaning Process

The raw dataset required several preprocessing steps before analysis.

Key cleaning tasks included:

### Handling Missing Values

Missing values were identified in variables such as:

* `is_recommended`
* `skin_type`
* `skin_tone`

These were handled by:

* Converting some missing values into an **"Unknown" category**
* Dropping irrelevant or unusable records where necessary

### Removing Irrelevant Columns

Columns that did not contribute to the analysis were removed to simplify the dataset.

Examples include:

* Unnamed index columns
* Non-informative metadata

### Data Type Conversion

Certain variables required conversion to appropriate data types:

* Numeric columns such as `price`, `rating`, and `reviews`
* Categorical variables such as `brand` and `product category`

### Aggregation

Additional metrics were computed to support analysis:

* Average rating by brand
* Average rating by product category
* Total number of reviews per brand

These aggregated metrics enabled clearer comparisons across brands and product types.


# Part 2 — Exploratory Data Analysis

Exploratory data analysis was conducted to identify patterns in customer satisfaction.

Visualizations were created using **Matplotlib and Seaborn** to explore relationships between variables.

Key analyses included:

### Brand Rating Analysis

Average ratings were calculated for each brand to identify **top-performing brands in terms of customer satisfaction**.

This analysis revealed that several brands consistently receive ratings above **4.6**, indicating strong perceived product quality.

---

### Price vs Rating Relationship

A scatter plot was used to analyze whether **higher-priced products receive better ratings**.

Key observation:

* There was **little to no correlation between price and rating**.

This suggests that **expensive products do not necessarily guarantee higher customer satisfaction**, and affordable products can perform equally well.


### Product Category Ratings

Average ratings were compared across product categories such as:

* Cleansers
* Masks
* Moisturizers
* Lip products
* Eye care

Key finding:

* **Cleansers and masks tend to receive the highest average ratings**, suggesting that skincare basics may generate stronger customer satisfaction.


### Review Volume Analysis

The number of reviews per product was examined to understand **customer engagement**.

Key insight:

* Some brands dominate the platform in terms of **review volume**, indicating stronger brand visibility and customer interaction.


# Part 3 — Tableau Dashboard

To translate the analysis into a business-friendly format, an **interactive Tableau dashboard** was developed.

The dashboard summarizes key metrics and insights from the dataset.

## Dashboard Components

### Key Performance Indicators

The dashboard highlights several headline metrics:

* **Average Overall Rating:** 4.30
* **Total Products:** 2,351
* **Total Brands:** 142
* **Total Reviews:** Large-scale customer engagement across the platform

These metrics provide context for the scale of the dataset and overall customer sentiment.


### Top Brands by Average Rating

A bar chart identifies brands with the highest customer ratings.

This helps highlight **brands that consistently deliver high customer satisfaction**.


### Price vs Rating Scatter Plot

A scatter plot visualizes the relationship between **product price and rating**.

The chart reinforces the earlier finding that **higher price points do not necessarily lead to better ratings**.


### Ratings by Product Category

A horizontal bar chart compares average ratings across product categories.

This allows quick identification of **product types that perform best with customers**.


### Skin Type & Skin Tone Heatmap

A heatmap visualizes ratings across combinations of:

* Skin type (dry, oily, combination)
* Skin tone

This helps explore whether **product satisfaction varies across different customer profiles**.


### Market Dominance by Brand

A pie chart illustrates **brand dominance based on total review volume**, showing which brands attract the most customer attention.

Brands such as **Laneige and Dr. Dennis Gross Skincare** appear to capture a significant share of engagement.


# Key Business Insights

From the analysis, several insights emerge:

### 1. Customer Satisfaction is Generally High

The average product rating is **4.30**, indicating strong overall customer satisfaction across Sephora products.


### 2. Price is Not a Major Driver of Satisfaction

The analysis shows **minimal correlation between price and rating**.

Implication:

* Premium pricing does not guarantee higher satisfaction
* Affordable products can compete effectively with luxury brands


### 3. Skincare Categories Perform Best

Categories such as **cleansers and masks** tend to receive the highest ratings.

Implication:

* Basic skincare routines may generate more consistent satisfaction than niche or specialty products.


### 4. A Few Brands Dominate Customer Engagement

Review volume is heavily concentrated among a smaller group of brands.

Implication:

* Strong brand reputation and visibility drive customer engagement.


### 5. Satisfaction is Consistent Across Skin Profiles

The heatmap analysis suggests **relatively consistent ratings across skin types and tones**, indicating that many products perform well across diverse customer groups.


# Skills Demonstrated

This project demonstrates several key data analytics skills:

**Data Preparation**

* Data cleaning
* Handling missing values
* Data transformation

**Exploratory Data Analysis**

* Aggregation and grouping
* Pattern identification
* Statistical reasoning

**Data Visualization**

* Matplotlib and Seaborn visualizations
* Dashboard development in Tableau

**Business Insight Generation**

* Translating data analysis into actionable insights
* Communicating findings through visual storytelling


# Conclusion

This project demonstrates how customer review data can be leveraged to uncover insights about product performance, brand reputation, and consumer behavior in the beauty industry.

By combining **Python-based exploratory analysis with an interactive Tableau dashboard**, the project highlights the value of data analytics in understanding customer satisfaction and market dynamics.


# Future Improvements

Potential extensions to this analysis include:

* Sentiment analysis on review text
* Predictive modeling of product ratings
* Time-based trend analysis
* Brand comparison dashboards
