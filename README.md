# Market Basket Analysis

Market Basket Analysis using the Apriori Algorithm on grocery transaction data.

## Project Overview

This project analyzes grocery transaction data to identify frequently purchased products and discover relationships between products purchased together.

The Apriori algorithm is used to generate frequent itemsets and association rules based on support, confidence, and lift.

## Dataset

The project uses the `Groceries_dataset.csv` dataset.

- Total transactions/records: 38,765
- Columns: 3
- `Member_number`
- `Date`
- `itemDescription`

## Data Preprocessing

The following steps were performed:

- Loaded the grocery transaction dataset using Pandas.
- Converted the `Date` column into datetime format.
- Checked the dataset for missing values.
- Grouped transactions by customer and date.
- Converted transactions into a binary format using TransactionEncoder.

## Exploratory Data Analysis

The analysis identified the most frequently purchased products.

Top frequently purchased items include:

- Whole milk
- Other vegetables
- Rolls/buns
- Soda
- Yogurt
- Root vegetables
- Tropical fruit
- Bottled water
- Sausage
- Citrus fruit

## Market Basket Analysis

The Apriori algorithm was used to identify frequent itemsets.

Association rules were generated using:

- Support
- Confidence
- Lift

Some generated rules include:

| Antecedent | Consequent | Support | Confidence | Lift |
|---|---|---:|---:|---:|
| Yogurt | Whole milk | 0.011161 | 0.129961 | 0.822940 |
| Rolls/buns | Whole milk | 0.013968 | 0.126974 | 0.804028 |
| Other vegetables | Whole milk | 0.014837 | 0.121511 | 0.769430 |
| Soda | Whole milk | 0.011629 | 0.119752 | 0.758296 |

## Business Insights

- Whole milk was the most frequently purchased product in the dataset.
- Other vegetables, rolls/buns, soda, and yogurt were also frequently purchased.
- Association rules helped identify relationships between products.
- Yogurt → Whole milk had the highest lift among the generated rules.
- These patterns can help businesses understand purchasing behavior and support cross-selling strategies.

## Visualization

The project includes visualizations for:

- Top 10 most purchased items
- Top association rules by lift

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Mlxtend
- Apriori Algorithm
- VS Code
- Jupyter Notebook

## Project File

The complete implementation is available in:

`Market_Basket_Analysis.ipynb`

## Conclusion

Market Basket Analysis was performed on grocery transaction data using the Apriori algorithm. The analysis identified frequently purchased products and generated association rules based on support, confidence, and lift.

The results demonstrate how transaction data can be used to understand customer purchasing patterns and support product placement and cross-selling decisions.
