# Multiple Linear Regression from Scratch

Multiple linear regression implemented with **batch gradient descent in NumPy**, without an ML library, to predict a building's energy consumption.

- **Features:** building type (residential / commercial / industrial), square footage, number of occupants, appliances used, average temperature, weekday or weekend
- **Target:** energy consumption
- Categorical features are one-hot encoded and inputs normalized; gradient descent runs until the change in MSE loss falls below a tolerance.
- The notebook includes a short derivation of why gradient descent converges for the MSE loss, then compares predicted against actual values on a held-out test set.

## Files

- [`Linear_regression.ipynb`](Linear_regression.ipynb) — derivation, implementation and evaluation
- [`train_energy_data.csv`](train_energy_data.csv), [`test_energy_data.csv`](test_energy_data.csv) — data

## Run it

```bash
pip install numpy pandas matplotlib seaborn jupyter
jupyter notebook Linear_regression.ipynb
```

**Stack:** Python, NumPy, Pandas, Matplotlib, Seaborn
