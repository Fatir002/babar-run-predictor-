```markdown
# 🏏 Babar Azam T20I Run Predictor

This project uses **Linear Regression** to predict the number of runs Babar Azam might score in a T20 International (T20I) match, based on match-related features such as balls faced, 4s, 6s, and batting position.

## 📁 Project Structure

```

babar-run-predictor/
├── babar-t20i-stats.csv       # Dataset with Babar Azam's T20I match data
├── babar_model.py             # Python code to preprocess data, train, and evaluate the model
├── README.md                  # Project description and instructions (this file)

````

## 📊 Dataset

The dataset contains Babar Azam’s T20I performance stats with columns like:

- `Runs` – Runs scored (target column)
- `BF` – Balls faced
- `4s`, `6s` – Number of boundaries hit
- `Pos` – Batting position
- `Dismissal`, `Opposition`, `Ground` – Removed to simplify modeling

Note: `Runs` values with `*` (not out) are cleaned and converted to integers.

## ⚙️ Technologies Used

- Python
- pandas
- numpy
- scikit-learn

## 🚀 How to Run the Project

1. Place `babar-t20i-stats.csv` in the same folder as your Python file.
2. Install the required libraries:

```bash
pip install pandas numpy scikit-learn
````

3. Run the Python script:

```bash
python babar_model.py
```

## 📈 Model Evaluation

After training a Linear Regression model, the script prints:

* MAE (Mean Absolute Error)
* MSE (Mean Squared Error)
* RMSE (Root Mean Squared Error)
* R² Score

Output:

```
MAE: 2.55
MSE: 10.56
RMSE: 3.25
R² score: 0.98
```

## 📌 Notes

* Only numerical features are used to keep the model beginner-friendly.
* Categorical columns are dropped.
* Feature scaling is applied using `StandardScaler`.

## 🙋‍♂️ Author

**FATIR FARAZ**

```
```
