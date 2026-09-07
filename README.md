# codeathon-assessment
**Q1**— Cleaning: Fixed missing values (UnitPrice, Sales, Profit via calculation; Cost via median; CustomerName/Region/Product via "Unknown"; 2 rows with missing dates removed). Removed duplicates. Standardized OrderDate format. Loaded into the model.handled by imputing missing values

**Q2**— Visuals: Pie Chart (orders by Region), Column Chart (Top 5 products), Line Chart (Profit trend over time).

**Q3**— DAX:

Table: EastRegionOrders = FILTER('Table', [Region]="East")
Column: ProfitCostDifference = [Profit] - [Cost]
Measure: TotalProfit = SUM([Profit])
