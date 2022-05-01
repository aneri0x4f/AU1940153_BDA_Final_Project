# Exploratory Data Analysis of popular song trends on Spotify using Apache Spark and plotly
# Link to Notebook: https://www.kaggle.com/code/aneridalwadi/aneri-dalwadi-bda-project?scriptVersionId=94427698
#### BDA Final Project
#### _Aneri Dalwadi AU1940153_

### Problem 
* Given the dataset containing nearly 35 million rows that is 3.5GB CSV file, the spotify wishes to perform Exploratory Data Analysis on Taylor Swift. However the process must be fast and efficient enough to work with big data, should be fault tolerant and must not give an out-of-memory error. The analysis must also show the trends of the popularity of her songs. 

### Solution
* We can fulfil the requirements using Apache Spark
* Use cases and reasons are as follows:
  * Spark is built to perform EDA on petabyte-scale data
  * It adapts to the execution plan at runtime(lazy evaluation)
  * Spark also processes everything in RAM which makes it very fast. However if no sufficient RAM is available, it is capable of executing the remaining on the disk.
  * Here we are working with a 3.4GB CSV file! Spark helps to speed up the sql queries executed on millions of rows of data here.
  * It has distributed data processing engine.
  * It can be used from multiple languages and databases as well
  * We can perform graph analytics
  * It is fault tolerent
  * Supports multiple storage formats (here csv)
  * It has pandas API as well
  * Follows SQL closely

### Implementation
* We will use spark session to enable to use:
  * DataFrame
  * Register DataFrame as tables
  * Execute SQL over tables
  * Cache tables
  * Read parquet files
 * Perform Feature extraction nd feature engineering
 * Execute spark queris for EDA
 * Plot visualizations using matplotlib
