# Flight Ticket Price Prediction: Exploratory Data Analysis and Feature Engineering

This repository contains code that performs Exploratory Data Analysis (EDA) and feature engineering on the Flight Ticket Price Prediction dataset. The goal is to preprocess the data and extract relevant features for training a machine learning model to predict flight ticket prices accurately.

## Dataset

The dataset used for this analysis is sourced from Kaggle: [Flight Ticket Price Prediction](https://www.kaggle.com/nikhilmittal/flight-fare-prediction-mh/). The dataset is provided in two Excel files: `Data_Train.xlsx` (training data) and `Test_set.xlsx` (test data).

## Code Explanation

### Libraries Used

The following Python libraries are used for data analysis and preprocessing:

- pandas
- numpy
- matplotlib
- seaborn

### Data Preprocessing Steps

1. Importing Training and Test Datasets:
   - The training dataset is loaded using `pd.read_excel('Data_Train.xlsx')`.
   - The test dataset is loaded using `pd.read_excel('Test_set.xlsx')`.

2. Combining Datasets:
   - The training and test datasets are combined into a single dataframe using `final_df = train_df.append(test_df)`.

3. Feature Engineering:
   - The code extracts day, month, and year from the "Date_of_Journey" column.
   - Arrival and departure hours and minutes are extracted from their respective columns.
   - Duration of the flight is extracted in hours.
   
4. Encoding Categorical Features:
   - The `LabelEncoder` is used to convert categorical features (Airline, Source, Destination, Additional_Info) into numerical values.

5. Data Cleaning:
   - Incorrect duration data rows are dropped.
   
### Results and Analysis

- The preprocessing steps ensure that the dataset is ready for model training.
- Features like day, month, year, arrival and departure times, duration, and categorical features have been extracted and encoded.
- Missing values have been handled, and incorrect data rows have been removed.

### Additional Comments and Advice

- Further steps involve splitting the dataset into train and test sets for model training and evaluation.
- Feature scaling may be necessary before feeding the data to machine learning models.
- Consider exploring feature interactions and creating new features to enhance model performance.
- Experiment with different machine learning algorithms and evaluate their performance.

## Conclusion

This project demonstrates the importance of data preprocessing and feature engineering in machine learning tasks. By following these steps, the dataset is transformed into a format suitable for training predictive models.

For more details, feel free to explore the code in the Jupyter Notebook provided in this repository.

## Author

This repository is maintained by 4Pranjal. Feel free to use and modify the code for educational and research purposes.

For any questions or suggestions, you can contact me through my GitHub profile: [@4Pranjal](https://github.com/4Pranjal).

Made with ❤️ by [Pranjal Jain](https://github.com/4Pranjal)
