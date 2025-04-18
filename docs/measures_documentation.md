
##  DAX Measures Table

|  **Measure Name**     |  **Measure Function** |  **DAX Formula** |
|--------------------------|-------------------------|--------------------|
| **Avg Delivery Time**     | Calculates the average delivery duration across all transactions. | `AVERAGE(xmas_data[Delivery Time])` |
| **Avg Rating**            | Returns the average customer satisfaction rating. | `AVERAGE(xmas_data[Customer Satisfaction])` |
| **Sales ($)**             | Computes the total revenue after discounts. | `SUM(xmas_data[Final Price])` |
| **Sales Volume**          | Sums up the total quantity of products sold. | `SUM(xmas_data[Quantity])` |
| **Transactions**          | Counts the number of unique sales transactions. | `COUNT(xmas_data[Transaction ID])` |

