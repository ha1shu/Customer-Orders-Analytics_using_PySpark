#  Customer-Orders Analytics using PySpark

 PySpark project to analyze customer behavior and spending from order data using joins, ranks & aggregation.


##  Datasets Description

###  Customers Table

| Column            | Description                         |
|-------------------|-------------------------------------|
| customer_id       | Unique identifier for the customer  |
| name              | Full name of the customer           |
| city              | City in India                       |
| state             | State in India                      |
| country           | Country (India)                     |
| registration_date | Date of customer registration       |
| email             | Customer email                      |
| is_active         | Boolean flag (1 = active, 0 = inactive) |

###  Orders Table

| Column       | Description                           |
|--------------|---------------------------------------|
| order_id     | Unique identifier for the order       |
| customer_id  | Foreign key referencing customer_id   |
| order_date   | Date when the order was placed        |
| total_amount | Total order value in INR              |
| status       | Status of the order (e.g. 'paid')     |

---

##  Analytics Performed

-  Count of orders per customer
-  Total spending per customer
-  Customer ranking by total spend using `dense_rank()`
-  Joined view of customer order count and total spend
-  Sorted customer insights by spending and order frequency

---

##  Technologies Used

- Apache Spark (PySpark)
- Python 3
- Jupyter Notebook
- Google Cloud Platform (GCP) – optional for data hosting
- Databricks (optional environment)


 
