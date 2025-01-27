# Customer Lookalike Model

## Project Overview
This project implements a customer lookalike model that identifies similar customers based on their purchasing behavior, demographics, and transaction history. The model uses cosine similarity to find the top 3 most similar customers for each target customer.

## Features Used
### Customer Demographics
- Region (Asia, Europe, North America, South America) 
- Days Since Signup

### Transaction Behavior
- Transaction Count
- Total Spend 
- Average Purchase Value
- Total Quantity

### Category Preferences
- Books
- Clothing 
- Electronics
- Home Decor

## Implementation Details

### 1. Data Preparation
- Merges transaction and product data
- Calculates customer-level metrics
- Handles missing values
- Creates category preference ratios

### 2. Feature Processing  
- One-hot encoding for categorical variables
- StandardScaler for numerical features
- Feature normalization

### 3. Similarity Calculation
- Uses cosine similarity metric
- Identifies top 3 similar customers
- Generates similarity scores

## Output Format
The model generates 'Rahul_Yadav_Lookalike.csv' with:
- CustomerID
- Top 3 similar customers with similarity scores


## Requirements
- Python 3.x
- pandas
- numpy
- scikit-learn

## Files
- `tasks2.ipynb`: Main implementation notebook
- `Customers.csv`: Customer data
- `Products.csv`: Product data
- `Transactions.csv`: Transaction data
- `Rahul_Yadav_Lookalike.csv`: Output file with recommendations

## Model Performance
- Similarity scores range from 0.81 to 0.99
- Comprehensive feature coverage
- Balanced consideration of multiple customer attributes
