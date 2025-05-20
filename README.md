# Physiologically Realistic Simulation of Diabetes and Insulin Optimization

This project models a 24-hour simulation of a diabetic individual's glucose and insulin dynamics. It integrates meal absorption, liver glucose production, and real-time insulin dosing optimization to realistically capture daily physiological behavior.

## What This Project Does

- Simulates diabetic glucose-insulin regulation using a simplified physiological model
- Generates meals from a real nutrition dataset and categorizes them as healthy, balanced, or cheat
- Models glucose absorption based on glycemic load over time
- Triggers insulin only when glucose exceeds a threshold, and optimizes the dose using numerical minimization
- Logs glucose, insulin, dose amounts, and meal events
- Plots physiological signals and annotates meal timing

## Dataset Used

This simulation uses the following dataset for meal composition:

**Food Nutrition Dataset by Utsav Dey**  
https://www.kaggle.com/datasets/utsavdey1410/food-nutrition-dataset

The dataset includes detailed nutritional information and is used to construct realistic synthetic meals. It is automatically downloaded using `kagglehub`.

> Note: A second dataset (`diabetes_merged_date-time-sorted.csv`) containing real diabetes logs has been uploaded but is not yet integrated into the simulation.

## Example Output

The simulation produces a plot showing:

- Glucose levels over time
- Insulin doses computed by the optimizer
- Meal events and annotations

## Future Work

Planned improvements include:

1. **Integrating Real Patient Data**  
   Use logged insulin and glucose values from a real diabetic dataset to drive the simulation and validate predictions.

2. **Modeling Insulin Pharmacokinetics**  
   Simulate delayed absorption for different types of insulin (e.g., basal vs bolus).

3. **Meal-to-Dose Matching**  
   Build a smarter system for predicting ideal insulin dose based on meal contents.

4. **Multi-Day Simulation**  
   Extend to 48–72 hour simulation and analyze cumulative trends (e.g., A1c, insulin load).

5. **Interactive Deployment**  
   Build a Colab or web interface for exploration and teaching purposes.

## Requirements

- Python 3.7+
- `numpy`, `matplotlib`, `scipy`, `pandas`, `scikit-learn`, `kagglehub`

## Author

Daivarsi
