# What products are most often sold together !

## Functionality

This script accomplishes the following:

1. **Data Loading and Cleaning:**
    - Combines multiple CSV files from a specified directory into a single pandas DataFrame.
    - Cleans the data by removing rows with missing values and invalid order date entries.
    - Creates new columns for "Month" (extracted from "Order Date") and "Sales" (quantity multiplied by price).
2. **Frequent Itemset Analysis:**
    - Identifies unique orders and creates a "Grouped" column that combines product names within each order.
    - Analyzes the "Grouped" column to find the most frequent combinations (itemsets) of products purchased together.
    - Calculates the frequency of itemsets for combinations of 2, 3, and 4 products.
    - Prints the top 10 most frequent itemsets for each product combination size.
    

## Usage

1. **Prerequisites:**
    - Python 3.x with pandas, matplotlib, and itertools libraries installed.
2. **Data Preparation:**
    - Ensure your sales data is stored in separate CSV files within a designated directory.
    - Update the directory path in the `files` list within the script to point to your data location.


## Output
    - Displays the bar chart to show most frequent "2 item set"
    
The script will print the top 10 most frequent itemsets for product combinations of 2, 3, and 4. Each itemset will be displayed as a tuple with its corresponding frequency count.


