# 📊 Dataset

This folder contains the retail sales dataset used for the analytics dashboard and business intelligence project.

---

## 📁 Tables Included

- **sales_data** → Order-level transaction details with revenue and profit
- **regions** → Regional information and geography  
- **products** → Product details, categories, and pricing  
- **customers** → Customer demographics and purchase history  
- **deliveries** → Delivery tracking and status information  
- **ratings** → Customer satisfaction ratings and feedback  
- **payment_methods** → Payment mode details and transaction info  

---

## 📊 Data Schema

### 📋 sales_data Table
- `order_id` – Unique order identifier  
- `customer_id` – Customer reference  
- `product_id` – Product reference  
- `order_date` – Date of transaction  
- `quantity` – Items ordered  
- `revenue` – Total order revenue  
- `profit` – Profit amount  
- `region_id` – Region identifier  
- `category` – Product category  
- `payment_method` – Mode of payment  

### 📍 regions Table
- `region_id` – Unique region identifier  
- `region_name` – Region name  
- `market_segment` – Geographic segment  
- `sales_manager` – Assigned manager  

### 🏷️ products Table
- `product_id` – Unique product identifier  
- `product_name` – Product name  
- `category` – Product category  
- `sub_category` – Sub-category  
- `price` – List price  
- `cost` – Product cost  
- `margin` – Profit margin  

### 👥 customers Table
- `customer_id` – Unique customer identifier  
- `customer_name` – Customer name  
- `city` – City location  
- `region_id` – Associated region  
- `customer_segment` – Segment classification  
- `registration_date` – Customer registration date  

### 🚚 deliveries Table
- `delivery_id` – Unique delivery identifier  
- `order_id` – Associated order  
- `delivery_date` – Actual delivery date  
- `expected_date` – Expected delivery date  
- `delivery_status` – On-time / Late / Early  
- `shipping_mode` – Shipping method  
- `delivery_days` – Days taken for delivery  

### ⭐ ratings Table
- `rating_id` – Unique rating identifier  
- `order_id` – Associated order  
- `customer_id` – Customer who rated  
- `rating_score` – 1-5 rating  
- `feedback` – Customer feedback text  
- `rating_date` – Date of rating  

### 💳 payment_methods Table
- `payment_id` – Unique payment identifier  
- `order_id` – Associated order  
- `payment_type` – Credit card / Debit / Cash / Online  
- `payment_status` – Completed / Pending / Failed  
- `transaction_amount` – Amount processed  

---

## 📈 Data Statistics

- **Total Records:** 50,000+ transactions  
- **Date Range:** Jan 2022 - Present  
- **Geographic Coverage:** 25+ regions  
- **Product Range:** 500+ SKUs  
- **Customer Base:** 10,000+ unique customers  
- **File Size:** <50MB (optimized for GitHub)  

---

## 🔄 Data Quality

✅ **Data Cleaning Applied:**
- Removed duplicate records  
- Handled missing values  
- Standardized date formats  
- Validated numeric ranges  
- Checked referential integrity  

✅ **Data Validation:**
- Revenue > 0 for all valid orders  
- Delivery dates logical (expected > actual or actual = expected)  
- Ratings within 1-5 range  
- Customer IDs match across tables  

---

## 💾 Data Usage

These datasets are used to build:
- Power BI dashboards (Executive, Regional, Product, Delivery)  
- Business intelligence reports  
- Performance analytics  
- Trend analysis  
- KPI tracking  

---

## 🔐 Privacy & Security

- Personally identifiable information (PII) minimized  
- Customer names anonymized in sensitive environments  
- Financial details aggregated at reporting level  
- Access controlled to authorized personnel only  

---

## 📥 How to Use

### Loading Data in Power BI
1. Open Power BI Desktop  
2. Click "Get Data" → "Excel"  
3. Select relevant `.xlsx` or `.csv` files  
4. Load data into Power Query  
5. Perform transformations as needed  
6. Create relationships between tables  

### Loading Data in Excel
1. Open Excel  
2. Import CSV files using "Data" → "From Text"  
3. Create pivot tables for analysis  
4. Use VLOOKUP for cross-table references  

### Loading Data in SQL
1. Create database tables matching schema  
2. Import CSV files using bulk insert or ETL tools  
3. Create indexes for performance  
4. Establish foreign key relationships  

---

## 🔄 Data Refresh Schedule

- **Frequency:** Daily (typically overnight)  
- **Method:** Automated ETL pipeline  
- **Retention:** 3 years historical data  
- **Archival:** Quarterly backup to cold storage  

---

## 📌 Important Notes

- Data is structured for **analytical use** (star schema ready)  
- Supports **time-series analysis** with date dimension  
- Enables **cohort analysis** with customer dimensions  
- Optimized for **aggregation queries** and dashboarding  

---

## ⚡ Performance Tips

- Use date filters to reduce query volume  
- Aggregate data at appropriate granularity  
- Index key columns (order_id, customer_id, region_id)  
- Cache frequently used calculations  

---

## 🆘 Data Issues & Support

**Reporting Issues:**
- Contact data team for quality issues  
- Verify source data before reporting  
- Document discrepancies with specifics  

**Technical Questions:**
- Email: ankitkumar473mail@gmail.com  
- Reference: Data Schema v1.0  

---

## 📚 Additional Resources

- Data Dictionary: See table descriptions above  
- Schema Diagram: Available in project documentation  
- ETL Process: Documented in technical specs  
- Data Lineage: Maintained in metadata repository  

---

## 📅 Dataset Information

**Dataset Version:** 1.0  
**Last Updated:** 2026-05-06  
**Maintained By:** Analytics Team  
**Format:** CSV / XLSX  

---
