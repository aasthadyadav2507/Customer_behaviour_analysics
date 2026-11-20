# 📊 Customer Behavior Dashboard
 
An interactive **Power BI** dashboard that analyzes customer purchasing behavior, revenue drivers, and subscription trends across product categories, age groups, gender, and shipping types.
 
![Dashboard Preview](images/dashboard-preview.png)
<!-- Add a screenshot of your dashboard at images/dashboard-preview.png -->
 
---
 
## 📌 Project Overview
 
Understanding *who* buys, *what* they buy, and *how much* they spend is key to improving marketing, retention, and product strategy. This dashboard turns raw customer transaction data into a single-page, filterable view so stakeholders can quickly answer questions like:
 
- Which product categories generate the most revenue?
- Which age groups spend the most?
- What share of customers are subscribed vs. not subscribed?
- How do spending and ratings differ by gender or shipping type?
---
 
## 🎯 Key Features
 
| Area | What it shows |
|------|---------------|
| **KPI Cards** | Number of Customers, Average Purchase Amount, Average Review Rating |
| **Subscription Split** | Donut chart: % of customers by subscription status |
| **Revenue by Category** | Column chart of total purchase amount per product category |
| **Sales by Category** | Column chart of customer volume per product category |
| **Revenue by Age Group** | Bar chart of total purchase amount per age group |
| **Sales by Age Group** | Bar chart of customer volume per age group |
| **Interactive Slicers** | Filter the whole page by Subscription Status, Gender, Category, and Shipping Type |
 
---
 
## 🗂️ Data Model
 
The report uses a single table, **`public.customer`**, loaded into Power BI.
 
| Field | Description |
|-------|-------------|
| `customer_id` | Unique customer identifier |
| `age_group` | Customer age bucket |
| `gender` | Customer gender |
| `category` | Product category purchased |
| `purchase_amount` | Amount spent per purchase |
| `review_rating` | Customer review rating |
| `subscription_status` | Subscribed / not subscribed |
| `shipping_type` | Shipping method chosen |
 
> The `public` schema prefix suggests the data was loaded from a **PostgreSQL** database. Update this section with your exact source (database, CSV, Kaggle dataset, etc.).
 
### Measures
 
- **Number of Customers**: count of customers
- **Average Purchase Amount**: average of `purchase_amount`
- **Average Review Rating**: average of `review_rating`
---
 
## 🛠️ Tech Stack
 
- **Power BI Desktop** (dashboard, data model, DAX measures)
- **PostgreSQL** (data source, if applicable)
- **DAX** (calculated measures)
---
 
## 🚀 Getting Started
 
### Prerequisites
- [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (latest version recommended)
- Access to the data source (see **Data Model** above)
### Run it locally
1. Clone the repository:
```bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
```
2. Open `customer_behavior_dashboard.pbix` in Power BI Desktop.
3. If prompted, update the data source credentials:
   **Home → Transform data → Data source settings**.
4. Click **Refresh** to load the latest data.
---
 
## 📁 Repository Structure
 
```
├── customer_behavior_dashboard.pbix   # Power BI report file
├── images/
│   └── dashboard-preview.png          # Dashboard screenshot
├── data/                              # (Optional) sample dataset
└── README.md
```
 
---
 
## 💡 Key Insights
 
*Replace these with your own findings from the dashboard:*
 
- 📈 Top-performing category: **\_\_\_**
- 👥 Highest-spending age group: **\_\_\_**
- 🔔 Subscribed customers make up **\_\_\_%** of the base
- ⭐ Average review rating across customers: **\_\_\_**
---
 
## 🔮 Future Improvements
 
- Add time-based analysis (monthly/seasonal trends)
- Add customer segmentation (e.g., RFM analysis)
- Add discount and payment method breakdowns
- Publish to Power BI Service with scheduled refresh
---
 
## 🤝 Contributing
 
Suggestions and improvements are welcome. Feel free to open an issue or submit a pull request.
 
---
 
## 📬 Contact
 
**Your Name**
- GitHub: [@your-username](https://github.com/your-username)
- LinkedIn: [your-profile](https://linkedin.com/in/your-profile)
---
 
⭐ If you found this project useful, consider giving it a star!
 