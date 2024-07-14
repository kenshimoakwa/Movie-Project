## Project Title: Predicting Movie Ratings
This analysis attempts to answer the question of what the key factors are in making a good film. We analyze movie rating data using machine learning techniques to identify key factors. The most interesting results were that Running Time (the length of the movie), budget, and release year were important factors that led to high rating scores. These factors may reveal reviewers' interesting biases and indicate to producers the factors making a film.

## Files
**"FinalMLProject_CompleteCodes.ipynb"** This is the Python script that performs the data analysis

**"Movie project  document.pdf"** This report presents the results and findings from the analysis conducted in "FinalMLProject_CompleteCodes.ipynb"

## Summary of the analysis
Data Loading: Loads the XYZ data from the provided dataset.

Data Cleaning: Preprocesses the data to handle missing values and inconsistencies.

Exploratory Data Analysis (EDA): Conducts exploratory data analysis to understand data distributions and relationships.

Modeling: Applies machine learning models to identify patterns and make predictions.

Results: Output the results, which are summarized and interpreted in report.pdf.

## Results

### Model Performance

**Random Forest Model:** The Random Forest Model was best suited with a Train Accuracy of 0.94, Train Precision of 0.942, Test Accuracy of 0.88, and Test Precision of 0.89.
Significant Predictors

**Runtime:** Runtime was found to be the second most significant predictor. Longer movies tend to receive higher critical ratings, aligning with Mark Hofmeyer's article that discusses the positive correlation between movie length and Rotten Tomato ratings.

**Vote Count and Budget:** As expected, vote count correlates with rating, and budget correlates with vote count.

**Release Year:** Surprisingly, it predicts rating, suggesting an increase in average movie ratings over time.

**Genres:** Drama and Animation significantly affect ratings, possibly due to perceived prestige or family-friendliness.
Insights on Movie Collections

**Belonging to a Collection:** Contrary to expectations, being part of a collection (e.g., sequels) is not a strong predictor of high ratings. This may be due to heightened viewer expectations and potential disappointment with sequels compared to their originals.
