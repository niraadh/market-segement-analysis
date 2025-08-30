# Market Segment Analysis

## Overview
This project analyzes customer purchase behavior and transaction data to identify market segments based on **lifestyle stage** and **premium status**.  
The goal is to derive insights into customer demographics, spending patterns, and potential marketing strategies.

---

## Dataset
### 1. `purchase_behaviour.csv`
Contains customer demographics and segmentation attributes.

| Column Name       | Description                                          |
|-------------------|------------------------------------------------------|
| LYLTY_CARD_NBR    | Unique customer loyalty card number                  |
| LIFESTAGE         | Customer lifestyle category (e.g., Young Families)   |
| PREMIUM_CUSTOMER  | Customer segment based on spending level             |

### 2. `transaction_data.csv`
Contains individual transaction details, including items purchased, quantities, and spend.

---

## Key Steps
1. **Load Datasets**  
   ```python
   import pandas as pd
   behavior = pd.read_csv('purchase_behaviour.csv')
   transactions = pd.read_csv('transaction_data.csv')
