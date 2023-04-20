## Consumer Complaints

## Description

In this project we analyzed data about consumer complaints received by the consumer financial protection bureau. We wanted to visualize the  following:

- The proportion of response types
- The  trend of the consumer complaints by month
- A count of the complaints by product
- The top 10 companies that received the most complaints.

The data was found from the consumer data protection bureau and we took a csv from the website that we then cleaned and uploaded to a sql database.


## Installation

What are the steps required to install your project? Provide a step-by-step description of how to get the development environment running:
   - Download CSV and place in Resources folder
   - Download and run etl.ipynb
   - Download and run create_and_load_sqlite_database.ipynb
   - Download the rest of the files app.py, app.js, and index.html
   - Run app.py so routes are live, check a route to make sure its loading.
   - View index.html in browser to view Dashboard

## Process
   First a CSV with the data is cleaned using pandas and numpy on the etl.ipynb file, then the a new clean csv file is created that features only the relevent data needed. Then SQL Alchemy is used to load clean csv file data into a PostgreSQL database table.  Then in the app.py file flask is used to create an api with multiple routes that will then be used to query the data needed for charts.
   <img width="482" alt="image" src="https://user-images.githubusercontent.com/118862894/233406114-d5fe8cab-cd1f-462d-b074-724254426038.png">


    ```

## Features & Links to data

Drop Down that filters the graphs by products.

https://www.consumerfinance.gov/data-research/consumer-complaints/search/?chartType=line&dateInterval=Month&dateRange=3y&date_received_max=2023-04-11&date_received_min=2020-04-11&lens=Overview&searchField=all&tab=Trends


