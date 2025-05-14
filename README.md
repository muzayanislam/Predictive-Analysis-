
# ✈️ Sentiment Analysis and Predictive Modeling of Customer Bookings

This project involves web scraping, sentiment analysis, and predictive modeling based on British Airways customer reviews and booking data. The main goals were to extract insights from user-generated content and build a model that predicts booking behavior using customer data.


## Objectives

* Scrape customer reviews from the British Airways   review website.

* Preprocess and clean the textual data.

* Perform sentiment analysis and visualize word trends.

* Use structured booking data to train a predictive model for customer bookings.
## Data Sources

### 1. Review Data
- **Source:** [AirlineQuality - British Airways Reviews](https://www.airlinequality.com/airline-reviews/british-airways)
- **Format:** HTML (scraped using `requests` and `BeautifulSoup`)
- **Size:** 1000 reviews

### 2. Booking Data
- **Source:** Provided dataset (`customer_booking.csv`)
- **Format:** Structured CSV file
- **Size:** 50,000 records

## Data Sources

### 1. Review Data
- **Source:** [AirlineQuality - British Airways Reviews](https://www.airlinequality.com/airline-reviews/british-airways)
- **Format:** HTML (scraped using `requests` and `BeautifulSoup`)
- **Size:** 1000 reviews

### 2. Booking Data
- **Source:** Provided dataset (`customer_booking.csv`)
- **Format:** Structured CSV file
- **Size:** 50,000 records

## 🛠️ Tools & Libraries Used

- **Languages & Libraries:** Python, Pandas, NumPy  
- **Web Scraping:** BeautifulSoup, Requests  
- **Text Processing & Visualization:** NLTK, WordCloud, Matplotlib, Seaborn  
- **Machine Learning:** Scikit-learn  
## 🔍 Sentiment Analysis Workflow

### 1. Web Scraping
- Scraped 10 pages (100 reviews each) of verified and unverified British Airways reviews.
- Stored the results in a `Reviews.csv` file.

### 2. Data Cleaning
- Removed irrelevant data from reviews.
- Stripped symbols, converted text to lowercase, and removed non-alphabetic characters.

### 3. Text Preprocessing
- Tokenization  
- Stopwords removal (`nltk.stopwords`)  
- Stemming using `PorterStemmer`

### 4. Visualization
- Generated a Word Cloud of top keywords.  
- Extracted and visualized top 20 most common words.  
- Plotted frequency distribution of top 4-grams.
## 🔢 Predictive Modeling Workflow

### 1. Dataset
- `customer_booking.csv` with 50,000 rows and 14 features.

### 2. Goals
- Understand patterns in customer booking behavior.  
- Predict whether a booking will be completed based on input features.  
- _Note: The modeling part is still under development._
## 📊 Key Visualizations

- WordCloud of reviews showing commonly discussed terms  
- Top 20 keywords bar chart from processed reviews  
- N-gram analysis (4-grams) to identify common phrases  

## Future Work


- Implement machine learning models like Logistic Regression, Random Forests, and XGBoost  
- Perform model evaluation (accuracy, precision, recall, F1-score)  
- Add sentiment polarity scoring and classify reviews as Positive, Negative, or Neutral