# E-commerce-product-recommendations-using-catboost
This project builds a recommendation system for an online retail dataset.The workflow involves:

Data loading & preprocessing: Importing transaction records from an Excel file
Drop rows with missing values
Convert InvoiceDate to datetime
Create a new column for total price
Filter out negative quantities

Feature engineering: Feature engineering is a technique where we engineer new features based on existing features. Features like the recency, frequency and monetary value (RFM) are created for each customer .

Modeling with CatBoost

Visualize Feature Importance: CatBoost provides feature importance which helps understand which features are contributing the most to the predictions. We are doing this too understand why model is getting overfitted.

I created an interactive GUI where users can input recency, frequency and monetary values to get a recommendation.
