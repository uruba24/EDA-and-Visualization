
# 🏡 Airbnb Listings EDA - Airbnb Open Data

This repository contains an exploratory data analysis (EDA) of the Airbnb Listings dataset for New York City in 2008. The dataset was sourced from [Inside Airbnb](http://insideairbnb.com/get-the-data.html) and provides insights into listings, pricing, availability, and other features.

---

## 📁 Dataset Used

- **File:** `Airbnb_Open_Data.csv`
- **Source:** Inside Airbnb
- **Contents:** Listings data for NYC including location, price, room type, availability, and host information.

---

## 📊 Project Steps

### 1. **Loading the Dataset**
The dataset is extracted from a ZIP archive and loaded using `pandas`.

### 2. **Data Cleaning**
- Dropped rows with missing critical fields (`price`, `room type`, `neighbourhood group`)
- Filled remaining missing numeric values with median
- Removed duplicate records

### 3. **Outlier Detection**
- Visualized outliers in the `price` column using a boxplot

### 4. **Visualizations**
- Bar chart: Distribution of room types
- Histogram: Distribution of prices
- Correlation heatmap: Relationship between numeric features

### 5. **Summary Insights**
- Total number of listings
- Average price of listings
- Most common room type
- Most common neighbourhood group

---

## 🛠️ How to Run the Script

### Prerequisites
Make sure you have the following Python libraries installed:

```bash
pip install pandas matplotlib seaborn
```

### Running the Script

1. Clone the repository:
```bash
git clone https://github.com/your-username/airbnb-eda.git
cd airbnb-eda
```

2. Place the dataset ZIP file (`archive (1).zip`) in the project directory.

3. Run the script:

```bash
python airbnb_eda.py
```

---

## 📌 Observations

- **Manhattan** had the highest number of listings and the highest average prices.
- **Entire home/apt** is the most frequently listed room type.
- There are extreme outliers in price that may need to be further investigated or capped for modeling.
- A slight correlation exists between price and number of reviews, though not very strong.

---

## 📁 Output

- Cleaned dataset saved as `cleaned_airbnb_listings.csv`
- Visualizations displayed inline when script is run

---

## 📬 Contact

For any questions or feedback, feel free to reach out at [urubaftb@gmail.com].
