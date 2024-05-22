# DMARKAS-PROJECT

## Table of Contents

-[Project Overview](#project-overview)
-[Results/Findings](#resultsfindings)

### Project Overview

  This data analysis project will investigate the sales volumes and trends of the company during the first 5 months of 2024. This will help us make data-driven recommendations and gain a deeper understanding of the companies performance. 

### Data Sources

Sales Data

### Tools

-Excel -Data Cleaning
-PostgreSQL -Data Analysis

### Exploratory Data Analysis

-what is the overall sales trend?
-which products are top sellers?
-what are the peak sales periods?

### Data Analysis

```
SELECT DISTINCT (dmarkasrep.store_name), sales_rep_name, sales_by_store.amount_sold
FROM dmarkasrep
JOIN sales_by_store
ON sales_by_store.store_name = dmarkasrep.store_name
WHERE sales_rep_name = ''
GROUP BY dmarkasrep.store_name, sales_rep_name, sales_by_store.amount_sold
```

###  Results/Findings
