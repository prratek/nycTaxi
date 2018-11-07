# nycTaxi
`nycTaxi_rf.ipynb` contains my work for the [New York City Taxi Fare Prediction](https://www.kaggle.com/c/new-york-city-taxi-fare-prediction) Kaggle playground competition. I employ a **Random Forest Regressor** to predict the fare of a New York City yellow taxi using data that would be available at the start of the ride.
Random Forests are a **supervised ensemble learning method** that bag together several decision trees to correct for their tendency to overfit.

**Data**: You can find that data for this project from the cometition's [`Data` tab](https://www.kaggle.com/c/new-york-city-taxi-fare-prediction/data). When running this code, I had `train.csv` and `test.csv` in a subdirectory within my working directory called `data`. If you use a different file structure or change the file names, make sure to update the `PATH` variable in the notebook and modify the `read_csv` calls accordingly.

While the goal at the end is to predict our target variable (`fare_amount`), this notebook pays particular attention to a key stength of the Random Forest – **INTERPRETATION**. I go through the following general steps:

1. **Loading** and **inspecting** the data, cleaning up non-sensical data as needed.
2. Some **basic feature engineering** using information about the pickup and dropoff locations.
3. Building a quick and dirty **Random Forest baseline**.
4. Single trees, **bagging**, and randomness.
5. **Datetime feature engineering**.

To come:
1. More on hyperparameter tuning.
2. More feature engineering (maybe) - weather, traffic speeds by time, important locations, boroughs, public holidays
3. Interpretation – feature importance, confidence intervals
4. Modular code with separate modules for different functionality that I define in the notebook.

If you have any questions, suggestiong for how this notebook can be improved, or ideas for cool things I can do with Random Forests, **feel free to reach out!**

**Credits:** This work is a result of working through the fast.ai Machine Learning 1 course. I have occasionally borrowed code snippets or ideas from the lessons on Random Forests, the code for which can be found at this [Github repo](https://github.com/fastai/fastai/tree/master/courses/ml1).
