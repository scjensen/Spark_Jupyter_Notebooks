# Spark_Jupyter_Notebooks
Contains data files for the Data Science for All seminar -Spark and Jupyter Notebooks

The data files here are used in a seminar designed to introduce any students at 4-year colleges and communuity colleges to Apache Spark and Jupyter Notebooks.  The seminar uses cloud-based Databricks Community Edition accounts (thanks to Databricks for making them available).  The data files represent data on Federal government contracts in the United States from 2014 through 2018, which covers two different administrations, from two different political parties, led by presidents with very different viewpoints.  The data is from the USASpending.gov data site: https://www.usaspending.gov, but some intial wrangling has been done.  The USASpending download API is limited as to the number of records that can be downloaded in a single request and fails silently if the request exceeds the maximum file size.  For that reason, the data is initially downloaded by month.  If you want to access the USASpending data for other purposes, the Jupyter notebooks (using plain old Python, not Spark) are available from the Data Science for All website and you can modify them for your purposes.

In the seminar students wrangle and visualize the data. Each year is a separate data file in a bzip2 format, but the files within the zip file are in a PARQUET format so a table can quickly be created in Spark from the files.  We also make the files available as csv files in a bzip2 format (since Spark can work directly with that file format), but creating the tables is much faster from the PARQUET files than from the csv files, so we use that approach in the seminar; the data in the files is the same in both formats.

The notebooks for the seminar, along with slides and other materials are available from the Data Science for All website: https://www.sjsu.edu/datascienceforall

If you are an educator, we also make additional teaching notes, quiz questions, and a Canvas cartrige available to import.  Please see the Data Science for All website for details.

The seminar series (currently there are 8 seminars), is funded under NSF grant #1829622 and all of the seminar materials are available under a Creative Commons Attribution-ShareAlike 4.0 International license: https://creativecommons.org/licenses/by-sa/4.0

If you have questions regarding the seminars or the data, please contact us on the Data Science for All website.
