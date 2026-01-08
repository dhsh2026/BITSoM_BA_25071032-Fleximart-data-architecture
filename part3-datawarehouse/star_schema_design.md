## Star Schema Design

### Fact Table
fact_sales
- sale_id
- product_id
- customer_id
- date_id
- store_id
- quantity
- total_amount

### Dimension Tables
dim_product (product_id, name, category, brand)
dim_customer (customer_id, name, region)
dim_date (date_id, day, month, year)
dim_store (store_id, city, state)

### Justification
The star schema improves query performance for analytical workloads
by minimizing joins and enabling efficient aggregations.
