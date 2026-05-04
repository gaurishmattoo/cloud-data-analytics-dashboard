# Cloud-Based Data Analytics Dashboard (AWS)

## 📌 Overview

This project demonstrates a cloud-based data analytics pipeline using AWS services.

It processes raw data stored in Amazon S3 and performs analysis using AWS Glue and Amazon Athena.

---

## 🛠️ Technologies Used

* Amazon S3 – Data storage
* AWS Glue – Data catalog and crawler
* Amazon Athena – SQL-based data analysis

---

## ⚙️ Workflow

1. Upload dataset to S3 bucket
2. Create Glue database
3. Run Glue crawler to generate table
4. Query data using Athena
5. Analyze insights

---

## 📊 SQL Queries

### View Raw Data

```sql
SELECT * FROM raw_data;
```

### Revenue by Region

```sql
SELECT region, SUM(revenue) AS total_revenue
FROM raw_data
GROUP BY region;
```

### Sales by Product

```sql
SELECT product, SUM(quantity) AS total_sales
FROM raw_data
GROUP BY product;
```

### Revenue by Category

```sql
SELECT category, SUM(revenue) AS revenue
FROM raw_data
GROUP BY category;
```

### Daily Revenue

```sql
SELECT date, SUM(revenue) AS daily_revenue
FROM raw_data
GROUP BY date
ORDER BY date;
```

---

## 🖼️ Screenshots

### S3 Upload

![S3 Upload](1_s3_upload.png)

### Upload Success

![Upload Success](2_upload_success.png)

### CSV File

![CSV](3_csv_file.png)

### Glue Database

![Glue DB](4_glue_database.png)

### Glue Crawler

![Crawler](5_glue_crawler.png)

### Glue Table

![Table](6_glue_table.png)

### Athena Queries

![Raw Data](7_query_raw_data.png)
![Region](8_query_region.png)
![Product](9_query_product.png)
![Category](10_query_category.png)
![Daily](11_query_daily.png)

---

## ✅ Conclusion

This project shows how AWS can be used for scalable and serverless data analytics.

---

## 👨‍💻 Author

Gaurish Mattoo
