## 📈 Week 1: Data Analysis & Visualization

This week, I loaded, cleaned, and merged the generation and weather datasets. I engineered new features (`hour`, `month`) and filtered for daylight hours to focus the analysis.

### Key Findings:

1.  **Sunlight vs. Power:** There is a strong, direct linear relationship between solar irradiation and power output.

<img width="859" height="547" alt="image" src="https://github.com/user-attachments/assets/3bee7433-dac3-4c31-b38c-8b7b28827ffe" />

2.  **Daily Power Curve:** The power generation follows a clear daily pattern, peaking at noon.

   <img width="868" height="547" alt="image" src="https://github.com/user-attachments/assets/e4e670ca-0ae6-401d-96a8-d470cb96412b" />

## 🤖 Week 2: Model Training & Evaluation

This week, I trained and compared two machine learning models to predict power output:

* **Linear Regression (Baseline):** R-squared = 0.9495
* **Random Forest (Champion):** R-squared = 0.9637

The Random Forest model was more accurate and will be used for the final predictions.

## 🏁 Final Results & Conclusion

To validate the model, I performed two final visualizations.

### 1. Actual vs. Predicted Power
I plotted the predicted values against the actual values to check accuracy.

<img width="859" height="547" alt="image" src="https://github.com/user-attachments/assets/48804d3b-27df-4de8-a866-46724db04f12" />

* **Observation:** The blue dots are tightly clustered around the red diagonal line.
* **Result:** The Random Forest model achieved an **R² score of 96%**, proving it is highly accurate.

### 2. Feature Importance
I analyzed which factors contributed most to the power generation.

<img width="839" height="470" alt="image" src="https://github.com/user-attachments/assets/0ac6daf5-e3f5-4237-b244-8a5698ab2b08" />

* **Observation:** The graph confirms that **Irradiation (Sunlight)** is the single most important factor for predicting solar power, followed by Temperature and Hour.

### ✅ Conclusion
The project successfully demonstrated that machine learning can be used to reliably forecast renewable energy generation. The Random Forest model was significantly better than the baseline, handling the complex relationship between weather and power output.
