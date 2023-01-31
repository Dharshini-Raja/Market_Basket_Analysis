# Market_Basket_Analysis
Market Basket Analysis (MBA) is an accidental transaction pattern that purchasing some
products will affect the purchasing of other products. By performing certain techniques, 
we could overcome the problem that we faced before. We will find a patterns that shows which 
items are frequently purchased together so that we could apply a discounts into a particular items 
more accurately. 

Dataset:
	The dataset used is about an online retail store in UK. This data is downloaded from UCI Repository
Using the read_csv() function in pandas library, import the csv. With 541909 instances and 8 features, 
the dataset holds the sales data for over an year. 

EDA:
	Null values are identified and dropped leading to 406829 rows. If there are negative numbers in 
quantity column, then the entry is removed to ensure that the transaction is not a cancelled one. A pie chart 
depicting the country column is visualized. After grouping according to the transaction, the data is encoded
into binary data that shows whether an item is bought(1) or not(0). Then, the transaction that has more than
one items bought is taken into consideration.

Applying Apriori Algorithm:
	Apriori algorithm is simply used to find the frequently bought items in the dataset. Install 
mlxtend to apply this algorithm. After applying apriori algorithm, frequently bought item is found by 
applying association rules to have knowledge about items that is more effective when sold together. To
find that, the lift value must be looked upon as hiigher the lift value, higher the association between the 
items.

Item placements, products bundling and customer recommendation and discounts are the business insights generated
by MBA.
