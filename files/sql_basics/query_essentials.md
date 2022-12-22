# Query Essentials

A SQL query comprises a few essential elements:

* choosing a data source (`from` clause), 
* selecting columns from that source (`select` statement), and
* filtering the data returned (`where` clause).

These elements manifest in a query like this:

``` sql
select
    column_1, 
    column_2
from
    table_name
where
    column_1 > 50
;
```

This page provides a brief description of each essential component. More depth is given in the pages that follow.

## Choosing a data source

BigQuery databases store information in a structured, columnar format. Information is stored as rows in tables. Tables are composed of columns, and datasets are composed of tables. 

When extracting information from BigQuery, you first specify the table from which you will grab data. This is done using the [`from` clause](https://cloud.google.com/bigquery/docs/reference/standard-sql/query-syntax#from_clause).