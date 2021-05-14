# Data Engineer Live Session

## General Instructions
 - Read this page carefully
 - Ask all questions you can think of
 - Ask for help when you get stock
 - Search for guide and solutions online
 - Speak out load what you are planning to do


## Preparation
- If you need to code, store the code in a github repository
- If you want to use a cloud provider, use GCP, use a Google account not used before in GCP
- You may choose to work locally and not use a Cloud
- You may need an IDE
- You may use Jupyter Lab to run Python
- For a local DB you may use SQLite

## Data Analysis Exercise
### 1) Data Analysis on Big Query
- Use a public Big Query data set for analysis
- Login into GCP and enable Big Query
- Once logged in, click on this [data-to-insights](https://console.cloud.google.com/bigquery?p=data-to-insights&d=ecommerce&t=web_analytics&page=table)
- The definitions of the **data-in-insights** is [here](https://support.google.com/analytics/answer/3437719?hl=en)
- Use the dataset `data-to-insights.ecommerce.web_analytics`
### Answer the following:
- How many unique visitors do we have?
- How many of the visitors made a purchase?
- Out of the total visitors who visited our website, what % made a purchase?
### 2) Data Analysis locally
- Use the `cereal.csv` dataset provided for analysis
- Use Python or SQL
### Answer the following:
- Show the first 10 rows
- Show all the columns *for python only*
- Does an increase in sugar lead to a higher rating?
- Visualize *for python only*
- Show the top 10 cereals with the major combination of sugars and carbo.
- Show the average of sodium among cereals with a rating higher than 38.
