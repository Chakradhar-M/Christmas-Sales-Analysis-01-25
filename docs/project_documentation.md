<h1 align="center">🎄 Holiday Season Sales Analysis</h1>

<div style="display: flex; justify-content: space-between; padding: 10px; background-color: #f4f4f4; border-radius: 8px;">
  <h4>📅 Date: Jan 2025</h4>
  <h4>🛠️ Tools Used: Power BI, Excel, Figma</h4>
  <h4>🏷️ Domain: Retail / E-commerce Analytics</h4>
</div>

---

### 📌 Background

In the retail and e-commerce world, the holiday season is the busiest and most critical time of the year. Events like **Christmas** and **Black Friday** drive huge spikes in shopping activity, with customers expecting deals, fast shipping, and gift-ready services. These high-volume sales periods are very different from **regular shopping weeks**, not just in terms of revenue but also in customer behavior, product preferences, and service expectations.

Understanding how customer preferences, promotional success, and operational metrics vary across these key periods is essential for businesses to plan better and deliver a smooth, satisfying experience. In this project, we explore sales and behavior data across three major phases: **Christmas**, **Black Friday**, and **non-holiday (regular)** periods, offering a deeper look into how consumer habits shift during peak times.

---

### 🎯 Objective

The goal of this project is to compare **Christmas**, **Black Friday**, and **regular sales periods** to:

✔️ Analyze sales trends and volume differences across each period  
✔️ Understand which product categories perform best during holidays vs. regular days  
✔️ Explore how promotions, discounts, and express shipping influence buying decisions  
✔️ Examine differences in customer demographics, satisfaction, and return rates  
✔️ Identify seasonal patterns that can help improve future holiday planning

By visualizing these insights in a Power BI dashboard, the analysis helps businesses understand what works best during peak seasons and how to better serve their customers during future holiday events.

---

###  📂 Essential Project Links  

| 🧭 Resource | 🔗 Access |
|------------|----------|
| <img src="https://github.com/Chakradhar-M/PBI_Images/blob/main/Portfolio_Icons/database.png?raw=true" width="20" style="vertical-align:middle;"> **Data Source** | 👉 [Click to View Data Source](https://zoomcharts.com/en/microsoft-power-bi-custom-visuals/challenges/fp20-analytics-december-2024) |
| <img src="https://github.com/Chakradhar-M/PBI_Images/blob/main/Portfolio_Icons/power-bi.png?raw=true" width="22" style="vertical-align:middle;"> **Power BI Live Report** | 📊 [View Interactive Dashboard](https://app.powerbi.com/view?r=eyJrIjoiNmI2MzkzZmItNWQ4MC00Y2MzLWI3YjEtYjc3YWY5MDk1ODk2IiwidCI6IjQ2NTRiNmYxLTBlNDctNDU3OS1hOGExLTAyZmU5ZDk0M2M3YiIsImMiOjl9) |
| <img src="https://github.com/Chakradhar-M/PBI_Images/blob/main/Portfolio_Icons/youtube.png?raw=true" width="20" style="vertical-align:middle;"> **Project Presentation** | 🎬 [Watch Presentation](#) |
| <img src="https://github.com/Chakradhar-M/PBI_Images/blob/main/Portfolio_Icons/linkedin.png?raw=true" width="22" style="vertical-align:middle;"> **LinkedIn Post** | 🔗 [Read on LinkedIn](https://www.linkedin.com/posts/chakradhar-mantena_holiday-sales-and-trends-dashboard-activity-7284234216077148161-08g2?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD9y4SkBuDMCUOFBEF1QAO3K3-8MrRRtZZk) |

📌 **Tip:** Right-click or Ctrl + Click to open links in a new tab.

---

### 📊 Sample Raw Data

<div style="overflow-x:auto;">

<table>
  <thead>
    <tr>
      <th>Transaction&nbsp;ID</th>
      <th>Date</th>
      <th>Time</th>
      <th>Customer&nbsp;ID</th>
      <th>Age</th>
      <th>Gender</th>
      <th>Location</th>
      <th>Longitude</th>
      <th>Latitude</th>
      <th>Store&nbsp;ID</th>
      <th>Online&nbsp;Order&nbsp;Flag</th>
      <th>Product&nbsp;ID</th>
      <th>Product&nbsp;Name</th>
      <th>Category</th>
      <th>Quantity</th>
      <th>Promotion&nbsp;Applied</th>
      <th>Gift&nbsp;Wrap</th>
      <th>Shipping&nbsp;Method</th>
      <th>Payment&nbsp;Type</th>
      <th>Delivery&nbsp;Time</th>
      <th>Weather&nbsp;during&nbsp;transaction</th>
      <th>Event</th>
      <th>Return&nbsp;Flag</th>
      <th>Customer&nbsp;Satisfaction</th>
      <th>Unit&nbsp;Price</th>
      <th>Total&nbsp;Price</th>
      <th>Discount&nbsp;Amount</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>24/12/2020</td>
      <td>07:27:59</td>
      <td>441</td>
      <td>27</td>
      <td>Other</td>
      <td>Ontario</td>
      <td>51.2538</td>
      <td>-85.3232</td>
      <td>37</td>
      <td>TRUE</td>
      <td>106</td>
      <td>Toys_Product</td>
      <td>Toys</td>
      <td>5</td>
      <td>FALSE</td>
      <td>FALSE</td>
      <td>Standard</td>
      <td>Credit&nbsp;Card</td>
      <td>5</td>
      <td>Snowy</td>
      <td>None</td>
      <td>FALSE</td>
      <td>5</td>
      <td>96.79</td>
      <td>483.93</td>
      <td>0</td>
    </tr>
    <tr>
      <td>2</td>
      <td>18/11/2022</td>
      <td>14:36:39</td>
      <td>340</td>
      <td>43</td>
      <td>Male</td>
      <td>British&nbsp;Columbia</td>
      <td>53.7267</td>
      <td>-127.6476</td>
      <td>24</td>
      <td>TRUE</td>
      <td>816</td>
      <td>Clothing_Product</td>
      <td>Clothing</td>
      <td>1</td>
      <td>TRUE</td>
      <td>TRUE</td>
      <td>Express</td>
      <td>Credit&nbsp;Card</td>
      <td>3</td>
      <td>Sunny</td>
      <td>None</td>
      <td>TRUE</td>
      <td>2</td>
      <td>95.28</td>
      <td>95.28</td>
      <td>0</td>
    </tr>
    <tr>
      <td>3</td>
      <td>26/12/2019</td>
      <td>20:23:50</td>
      <td>31</td>
      <td>25</td>
      <td>Other</td>
      <td>Quebec</td>
      <td>46.8131</td>
      <td>-71.2075</td>
      <td>92</td>
      <td>FALSE</td>
      <td>508</td>
      <td>Clothing_Product</td>
      <td>Clothing</td>
      <td>2</td>
      <td>FALSE</td>
      <td>FALSE</td>
      <td>Standard</td>
      <td>Credit&nbsp;Card</td>
      <td>2</td>
      <td>Rainy</td>
      <td>Christmas&nbsp;Market</td>
      <td>FALSE</td>
      <td>4</td>
      <td>52.37</td>
      <td>104.74</td>
      <td>0</td>
    </tr>
  </tbody>
</table>

</div>

🔗 Check out the **Data Dictionary** here 👉 [Click Here](https://github.com/Chakradhar-M/Christmas-Sales-Analysis-01-25/blob/main/dataset/data_dictionary.md)

---

### 📊 **Key Performance Indicators (KPIs)**

1️⃣ **Sales ($)**

Represents the total revenue generated from customer purchases after applying discounts. This metric helps in assessing overall earnings and the effectiveness of promotions during the holiday season.

2️⃣ **Sales Volume**

Measures the total number of products sold. It gives insights into product demand and helps identify top-selling categories and purchasing behavior trends.

3️⃣ **Transactions**

Indicates the total number of unique sales transactions recorded. It provides an overview of customer activity and engagement during the festive period.

---
