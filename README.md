## Market Basket Analysis

<p align="center">
<img width="1536" height="1024" alt="Maket Basket Analysis" src="https://github.com/user-attachments/assets/298f2866-74f3-46ee-922e-7bca40c592db" />
</p>

#### Skills:
Python (Programming Language), Association Rule, A-Priori Algorithm

#### Situation:
The data potrays daily transaction data of a store. The owner of the store inteintends to utilise the data collected from the day day-to-day operation to see the reception of all the items in the store and if there are any interesting item groups that favoured by the customers. This information would give insights to the owner in strategising the placement of the items so that it could improve the sales of those items.

#### Task:
Apply association rule mining to find insights through identifying the interesting associations between the items sold in the store and provide suggestions to the owner. Include the interpretation of the analysis outcome and recommendation to the owner based on the outcome.

#### Action:
Here is a general summary of the content in the following sections:

#### 1. Exploratory Data Analysis (EDA)
- **Data Overview and Cleaning**: Imports transaction data, renames columns and checks for missing values.
- **Basic Descriptive Analysis**: Explores the dataset structure, including unique counts of products, members and transaction dates.
- **Date Features**: The date column is converted to datetime format and new columns for year, month and day are created to analyse trends over time.
- **Frequency Analysis**: Item frequency is analysed by calculating the occurrence counts of each item, both overall and by year.
- **Visualisation**: Bar plots are created to show the top 10 best and least selling items. Additionally, a line plot of monthly sales quantities is generated to observe trends.
  
#### 2. Data Preparation
- **Transaction Baskets**: Data is organised into baskets to represent items purchased in each transaction, grouped by date and member_id.
- **One-Hot Encoding**: The basket data is transformed into a binary (0 or 1) format, where each row represents a customer transaction and each column represents an item, with 1 indicating the presence of an item in a transaction. This structure prepares the data for association rule mining.

#### 3. Methodology and Results
- **Frequent Itemsets**: The Apriori Algorithm is applied to the binary encoded data to identify frequently co-occurring items, with a specified minimum support threshold.
- **Association Rules**: Association rules are generated using various metrics (support, confidence, lift), with thresholds applied to filter for the most relevant rules.
- **Filtering Rules**: The code uses Zhang’s metric to filter and sort rules, identifying both strong positive and negative associations among items.
- **Visualisation of Rules**: Scatter plots are created to visualise the relationship between support and confidence, as well as support and lift, for the generated rules, providing insights into the item relationships.
