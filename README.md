# Regression-Analysis--Price-Prediction-Dataset
We built Regression Analysis Model on 'Car Price Dataset'.
Objective : build a model using provided Dataset in order to predict car price by considering features.

there are 26 variables in dataset, out of which 25 are features(x) and 1 target(y) vriable. features columns are symboling, normalized_losses, engine_location, drive_wheels, body_style, lenght, width, height,curb_weight, engine_type, num_of_cylinders, engine_size, fuel_system, bore, stroke,compression_ratio, horsepower, peak_rpm, city_mpg, highway_mpg. Target variable is price.
there are total 205 enteries, which is not enough for a good model.
here target var has numerical and continuous data type hence we will use Regression Analysis. there are two types of relationships exist between x and y, either Linear or Non-Linear. In Linear reg, depending upon no of x variables, we build 2 kinds of models, Simple LR (1 x var; y = mx + c) and multiple LR (more than 1 x var; y = sum(mi*xi)+c ; i= x variables)
In non-Linear reg, there exist no linearity but in curved form as fun defines in the form of polynomial (y = m0x0 + m1(x1)^2 + m2(x2)^3 + m3(x3)^4 +...)
some columns were containing special character '?' and null values also. i converted '?' into NaN and then filled with proper value.
target var column had null value columns which was inappropriate to fill(due to error chances) so removed those rows from entire dataset.
Data cleaning includes checking for duplicates, nulls, label encoding (to change data type to nummeric), fillna etc. then did EDA to understand about Dataset features. next step was random sampling i.e splitting of dataset include train and test. train part used for building model while test part used for checking performance of model.
then main part of project: imported LinearRegression file from scikit-learn librabry, saved function in variable, applied on dataset. here model has been built.
predicted for y-var. found out errors, calculated parameters - rsquare, adjusted rsquare, mse on train and test both, rmse, mape.
checked for outliers by plotting graph.
