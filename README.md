# Spark_GCP_data_engineering
The project is built to integrate GCP, Spark, Databricks and create an eco system where big data analysis is feasible.

Dataset and GCP
An open source dataset is used for analysis and is uploaded on Google cloud Storage (GCS). The dataset is uploaded via difference methods.
1. Directly from UI by creating a bucket and uploading the file.
2. Upload via gsutil (CLI method)
3. Via python programatically, with the use of google-cloud-storage library.

Databricks and Spark:
In order to focus on main functionality of spark databricks is used as a tool.
1. Databricks is used for Apache Spark because it makes Spark easier to use, manage, and scale, especially for big data and machine learning workflows.
2. Databricks offers managed Spark Cluster hence no setup needed.
3. Databricks clusters scale up/down automatically based on workload. It also supports auto-shutdown, saving costs when you're not using resources.
4. Reads/writes from AWS S3, Azure Blob, or Google Cloud Storage (GCS) with minimal setup. Also supports Delta Lake (Databricks' own format for faster, reliable analytics on Spark).

Analysis:
1. The pipeline begins by defining explicit schemas and loading match, player, team, and ball-by-ball data into Spark DataFrames. 
2. Through feature engineering, it extracts temporal attributes, categorizes players, and computes metrics like running totals, win margins, and veteran status.
3. The project uses both PySpark transformations and Spark SQL to analyze key aspects such as toss impact, batsman contributions in victories, economical powerplay bowlers, and venue-based scoring patterns.
4. Visualizations using Matplotlib and Seaborn enhance interpretability by presenting insights like top scorers, dismissal trends, and team performances after winning tosses.
Overall, the project demonstrates the power of distributed data processing and visual storytelling to uncover strategic patterns in the dataset.
