# Power BI horizontal composite model

This short post should show you how to combine direct query data with extracted data based on a date dimension, in Power BI. 

Let's assume you have one of the following scenarios:
 1. You have a table with transactional data, and you want to cache most of the historical data for a fast response time, but want to query the underlying compute engine (SQL Server, Azure Databricks, others) to retrieve recent transactions in near realtime
 2. You have a table with transactional data, and you want to keep the most recent data in the Power BI cache, but are happy to use the power of the underlying compute engine (SQL Server, Azure Databricks, others) for the more detailed data, in order to keep the size of the Power BI dataset small
 
The functionality that Power BI currently offers, via [composite models]() and [aggregations](), while very powerful, does not currently provide an obvious answer for these scenarios. The example below will show a workaround to solve scenario number one - with scenario number two just needing some small tweaks. 

## Source data

For this example I am using the [European Centre for Disease Prevention and Control (ECDC) Covid-19 Cases public dataset](https://www.ecdc.europa.eu/en/publications-data/download-todays-data-geographic-distribution-covid-19-cases-worldwide), and I am using the an [Azure Synapse Analytics] dedicated SQL pool(formerly known as Azure SQL Data Warehouse) as the underlying compute. The data looks like this in Power BI:



## Split into extract and direct query 

## Date dimension 

## New measure

## Results 
