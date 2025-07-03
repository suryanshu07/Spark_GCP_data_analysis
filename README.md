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

Project:
The analysis does a thorough study of taxi dataset to identify key trends and insights about durations, fare, peak hours, and popular pickup and drop-off areas.

Findings and highlights:
1. Average Fare by Hour: Fares tend to be higher in the early morning hours (4-6 AM), with the lowest fares around 7 PM, likely due to competition during peak demand times.
2. Trip Duration Patterns: Peak demand occurs between 6 PM and 10 PM, aligning with the most frequent pickup hours.
3. Popular Locations: Certain GPS coordinates show high pickup and drop-off frequencies, identifying hotspots that could inform targeted marketing or service allocation.
4. Fare and Distance Relationship: A moderate correlation exists between trip fare and distance, as expected, while trip duration and fare show a weaker correlation due to variability in traffic and route efficiency.
