## Class 13 Notes

1. **Can you explain the basic concept of linear regression and its purpose in the context of machine learning and data analysis?**

    - Linear regression is a statistical method used to model the relationship between a dependent variable and independent variables.
        - The purpose of this is to find data points that minimize any differences between observed values and values predicted by the linear model

2. **Describe the process of implementing a linear regression model using Python’s Scikit Learn library, including the necessary steps and functions.**

    1. First you import the necessary libaries,

    ```
    from sklearn.model_selection import train_test_split
    from sklearn.linear_model import LinearRegression
    from sklearn.metrics import mean_squared_error
    ```

    2. Then you load your dataset

    3. Use `train_test_split` to divide your set into test and training.

    ```
    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
    ```

    4. Create an instance of the LinearRegression class and fit the model into the training data

    ```
    model = LinearRegression()
    model.fit(X_train, y_train)
    ```

    5. Using the trained model make a prediction on the test set,

    ```
    y_pred = model.predict(X_test)
    ```

    6. Evaluate the model's performance using a metric such as Mean Squared Error

    ```
    mse = mean_squared_error(y_test, y_pred)
    ```

3. **What is the purpose of splitting the dataset into train and test sets, and how does this contribute to the evaluation of a machine learning model’s performance?**

    - The purpose of splitting train and test sets is to help the model evaluate new and unseen data. A test set provides data that will access the strengths and weaknesses of a model, while the data would be used to train the model to be able to evaluate the test set.

    - This also helps with overfitting as potentially too much data could result in negative results as details 