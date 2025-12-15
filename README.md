📈 Stock Market Analytics with Big Data & Sentiment Analysis














📌 Overview

This repository contains an end-to-end Big Data analytics pipeline that combines stock market prices with social media sentiment (Twitter) to generate short-term stock price predictions (1, 3 and 7 days).

The project integrates Hadoop, Spark, Hive, Machine Learning, NLP, and database performance analysis, demonstrating real-world data engineering and analytics skills.

🎯 Key Skills Demonstrated

Distributed data storage with HDFS

Data processing with Apache Spark

Data warehousing using Apache Hive

Sentiment analysis on tweets (NLP)

Time series forecasting (ARIMAX & LSTM)

Data integration (tweets + stock prices)

Performance benchmarking (MySQL vs Cassandra)

End-to-end analytics pipeline design

📂 Project Structure

StorageData.ipynb

Ingests tweets and stock prices from HDFS

Cleans and stores structured data in Hive

ProcessingData.ipynb

Performs EDA on tweets

Applies VADER sentiment analysis

Merges sentiment with stock prices

Builds ARIMAX and LSTM models for prediction

Comparison of Databases.ipynb

Benchmarks MySQL vs Cassandra using YCSB

Compares throughput and latency under load

🧠 Machine Learning & NLP

Sentiment Analysis:

VADER (selected over TextBlob for informal text)

Daily sentiment aggregation by company

Forecasting Models:

ARIMAX (price + sentiment as exogenous variable)

LSTM neural network for time series prediction

📈 Predictions generated for 1-day, 3-day and 7-day horizons.

🗄️ Database Performance Comparison

MySQL:

Stable latency, lower throughput

Cassandra:

Significantly higher throughput

Better suited for high-volume, write-heavy workloads

Benchmarked using YCSB with 100,000 records.

🛠️ Tech Stack

Python

Apache Spark

Hadoop (HDFS)

Apache Hive

Cassandra

MySQL

Scikit-learn

TensorFlow / Keras

Statsmodels

NLP (VADER, TextBlob)

Jupyter Notebook

🚀 How to Run
# Start Hadoop, Spark, Hive services
jupyter notebook


Configure HDFS paths and execute notebooks in order:

StorageData

ProcessingData

Database Comparison

👤 Author

Erwin Plaza Copajira
MSc Data Analytics
Data Analyst | Junior Data Scientist
📍 Ireland
