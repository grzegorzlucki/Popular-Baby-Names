# Popular Baby Names Prediction

This project focuses on predicting the year of birth based on baby names, gender, ethnicity, and other attributes using machine learning models.

## Data
The data used for this analysis is sourced from the [Popular Baby Names dataset](https://catalog.data.gov/dataset/popular-baby-names). You can download the dataset from the provided link. The dataset contains the following columns:

- `Year of Birth`: Year when the baby was born
- `Gender`: Gender of the baby (1 for FEMALE, 0 for MALE)
- `Ethnicity`: Ethnicity code (0 for HISPANIC, 1 for WHITE, 2 for ASIAN, 3 for BLACK)
- `Name`: Unique index representing the baby's name
- `Count`: Number of babies with the given name in a specific year
- `Rank`: Ranking of the name based on the count

## Data Preprocessing

- Converted `Gender` column to binary (1 for FEMALE, 0 for MALE).
- Extracted the first word from the `Ethnicity` column.
- Encoded `Ethnicity` as follows: 0 for HISPANIC, 1 for WHITE, 2 for ASIAN, 3 for BLACK.
- Mapped unique names to indices for better representation in the model.

## Machine Learning Models

### Decision Tree Classifier

- Used a Decision Tree Classifier to predict the `Year of Birth`.
- Achieved an accuracy score of approximately 80.28% on the test data.

### Random Forest Classifier

- Explored the Random Forest Classifier as an alternative model.
- Obtained the same accuracy score of approximately 80.28% on the test data.

## Conclusion

Both the Decision Tree Classifier and the Random Forest Classifier yielded similar accuracy scores of 80.28%. The models perform reasonably well in predicting the year of birth based on the given attributes. Further fine-tuning and feature engineering could potentially enhance the model's performance.
