# Used car prices: should the dealer buy this car?

Regression assignment, TECH-UB 24, Fall 2026. Daniyal Malik.

`used_car_regression.ipynb` predicts a used car's sale price from its mileage, age, horsepower, accident history and number of owners with a linear regression. It compares the model with a baseline that guesses the average price for every car, then uses both to decide which of 40 auction cars to buy.

## Files

- `used_car_regression.ipynb`: the analysis. Every number on the slides comes from it.
- `used_car_sales.csv`: 240 cars the dealer sold in the last year, used to fit and test the model.
- `auction_lots.csv`: 40 cars from one recent auction, used only to test the buy/pass rule.
- `predicted_vs_actual.png`: the chart on the slides, saved by the notebook.

## Run it

Put the two CSV files in the same folder as the notebook, then run all cells:

```
pip install -r requirements.txt
jupyter notebook used_car_regression.ipynb
```

The 70/30 split uses `random_state=42`, so every run gives the same numbers.
