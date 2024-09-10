![image](https://github.com/user-attachments/assets/6ddfe199-2980-4218-ba19-6582a95a8446)


# Retail Dataset
Using Kaggle and a publicaly available dataset [Retail Transactions: Online Sales Dataset](https://www.kaggle.com/datasets/shashanks1202/retail-transactions-online-sales-dataset), I performed data cleaning, processed the data for prediction models, and evaluated predictions using both Prophet and Linear Regression. 
<br>
<br>
The results were visualized with Matplotlib and Seaborn, and the detailed analysis and findings are documented in this [notebook](https://github.com/CameronCSS/Retail_Profit_Predictions/blob/master/Retail_Profit_Predictions.ipynb)



## Data Cleaning/Processing Steps


- **Data Integration:** Combine data from multiple sources and resolve conflicts or discrepancies

- **Deal with Duplicates:** Identify and remove duplicate rows to prevent skewed results

- **Fix or Remove NA Values:** Impute missing values or remove rows/columns with NA values based on their impact

- **Correct Incorrect Data:** Address data entry errors and inconsistencies

- **Handling Missing Values:** Drop the rows alltogether OR  Use techniques like forward/backward fill, or interpolation to fill values

- **Fix Data Types:** Convert columns to appropriate data types

- **Fix Random Column Names or Drop Unused Columns:** Standardize column names and remove irrelevant columns to simplify the dataset.

- **Handling Outliers:** Identify and address outliers through removal, or transformation

- **Standardizing Formats:** Ensure consistency in date formats, numerical formats, and categorical names/labels

- **Data Validation:** Perform consistency checks and cross-validation against reliable sources
  
- **Data Aggregation:** Summarize data at different levels if needed (e.g., aggregating daily data to monthly)
  
- **Documenting Data Cleaning Steps:** Keep a record of the data cleaning steps performed to ensure reproducibility and to provide clarity for your future self or other team members.

- **_Optional_: Convert Categorical Values to Numeric:** For ML you can convert Categorical values to Numeric (To train ML models)



## Conclusions:

- FB Prophet model shows simiar results to basic Linear regression with small sample sizes

- With such small sample sizes (Only 3 Years) AND the data seeming to be generated we cannot trust these predictions.

- This data and testing proves how much value ML models put into Deviation, whereas a human may take into account many other factors, such as the Fact that 85123A was a Top product in all three years but both models predicting it going DOWN

#### With more years data available the Deviation would not hold as much weight on the final prediction results
