# Spotify_analytics-AWS

# Spotify Analytics

This project demonstrates the development of a scalable and efficient data pipeline to analyze Spotify data, focusing on albums, tracks, and artists. The pipeline leverages AWS services to manage large datasets, enabling insightful analytics and visualizations. Key features include ETL processing, ad-hoc querying, and dynamic reporting through an interactive dashboard.

## Project Overview

- **Data Ingestion:** Large datasets (albums, tracks) are ingested into Amazon S3, creating a scalable storage solution. 
  - **Dataset Source:** The data was sourced from [Kaggle](https://shorturl.at/qBUX5) and includes information on albums, tracks, and artists.
  - **Processed Files:** 
    - `albums.csv`: Contains details like album name, track duration, release date, label, and album popularity.
    - `artists.csv`: Contains artist names, popularity, follower count, and genres.
    - `track.csv`: Contains track IDs and track popularity.

- **ETL Processing:** Data is transformed using AWS Glue to ensure data quality, allowing for seamless updates and transformations.
- **Schema Discovery:** AWS Glue Crawlers automatically manage schema discovery and data cataloging, enabling the pipeline to handle dynamic data updates efficiently.
- **Ad-hoc Analytics:** Amazon Athena is used to run SQL queries on the processed data, allowing for quick and efficient exploration and analysis.
- **Interactive Dashboard:** An Amazon QuickSight dashboard provides key performance indicators (KPIs) to track artist performance, engagement metrics, and top trending genres.

## Key Insights

- Identified the top 3 trending genres from the dataset, providing valuable insights into listener preferences and emerging music trends.

## Technology Stack

- **AWS S3**: For storing structured data in a scalable data lake.
- **AWS Glue**: Used for ETL (Extract, Transform, Load) processing, ensuring data integrity and scalability.
- **AWS Glue Crawlers**: For schema discovery and dynamic cataloging of data.
- **Amazon Athena**: For running SQL queries on S3 data, enabling ad-hoc analytics.
- **Amazon QuickSight**: For building interactive dashboards and data visualizations.
- **SQL**: Used for querying the data in Athena.

## Architecture Diagram

![Architecture Diagram](https://github.com/MansiVN/Spotify_analytics-AWS/blob/main/Architecture.png)

## How It Works

1. **Ingest Data**: Large datasets are loaded into Amazon S3.
2. **Transform Data**: AWS Glue performs ETL processing, cleaning, and transforming the data for analysis.
3. **Explore Data**: Amazon Athena allows SQL-based exploration of the processed data.
4. **Visualize Data**: Insights and KPIs are visualized using an Amazon QuickSight dashboard.

## Future Enhancements

- Automating the data ingestion process using AWS Lambda and API Gateway.
- Expanding the dataset to include more metadata for deeper analytics.
- Enhancing the dashboard with more granular KPIs and filtering options.

## Dashboard 

![Architecture Diagram](https://github.com/MansiVN/Spotify_analytics-AWS/blob/main/Dashboard_Part1.png)
![Architecture Diagram](https://github.com/MansiVN/Spotify_analytics-AWS/blob/main/Dashboard_Part2.png)

## Conclusion

This project highlights the power of AWS services in creating a robust and scalable data pipeline for Spotify analytics. By leveraging the full potential of S3, Glue, Athena, and QuickSight, the pipeline supports efficient data management and insightful reporting.
