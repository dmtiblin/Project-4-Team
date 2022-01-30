# Housing Market Prediction Model
The effects of the COVID 19 pandemic have had a major effect on the housing market and home values/listing prices. Using zillow to determine average home values per month for multiple neighborhood, and combining that with Federal Reserve Interest Rates and data from the US Census, we train a machine learning model to predict future home values.

The final presentation can be viewed in the included powerpoint deck. 

Team Members: Bonnie Bailey, Diane Tiblin, Joseph March

## Data Sources:
- Zillow Home Value Index - Metro US: [https://www.zillow.com/research/data/](https://www.zillow.com/research/data/)
- FRED Economic Data: [https://fred.stlouisfed.org/series/FEDFUNDS](https://fred.stlouisfed.org/series/FEDFUNDS)
- US Census: [https://www.census.gov/data/developers/data-sets.html](https://www.census.gov/data/developers/data-sets.html)

## Resources:
- AWS S3 Buckets
- Census and json
- Google Colab
- Scikit-learn
- PySpark
- Pandas

## Coding:
- Pulled API data from US Census. 
- Cleaned the data by modifying headers, formatting data and converting to rates.
- Uploaded Zillow and Federal Funding data to AWS in S3 buckets.
- Pulled Zillow and Federal Funding data using PySpark.
- Cleaned MSA columns so Census data would match Zillow in order to join data frames together.
- Converted Federal Funding data into lists to join to the merged data frame with date columns.
- Removed duplicate and non-zero values from the merged data frame. Performed one-hot encoding on the categorical data.
- Scaled the data.
- Created and tested linear regression model.

## Model Performance
We tested several versions of the model before coming to our final version.

![modeldata](/images/model_data.png)

## Challenges
- Difficulty finding free data on property sales.
- Slight narrowing of our data source with the elimination of fields with null data or duplications.
- Data was limited to metropolitan areas and the suburbs surrounding.

## Results/Findings
A model can be created to predict the market value to within 99.99% accuracy within a metropolitan area.

Note: The housing market is naturally unpredictable as a result of human behavior.

## How Could We Expand The Project?
- Currently the model predicts one month ahead. With additional work the model could be expanded to predict further into the future.
- Currently the model predicts averages within a metropolitan area. With funding, data could be pulled for individual properties.

## Contacts
- Bonnie Bailey: bonnie.lyn@hotmail.com
- Diane Tiblin: tiblindm@gmail.com
- Joseph March: josephmarch@gmail.com
