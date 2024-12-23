![Project Banner](assets/accident.png)

# Traffic Accident Severity Prediction from Chicago Road Accidents Data 2024

This project focuses on predicting the severity of traffic accidents based on historical data. The primary goal is to accurately classify instances of "High" severity while minimizing misclassification of "Low" severity cases. The project addresses class imbalance issues and employs various classification techniques, including Logistic Regression, to achieve optimal results.

---

## Objectives

1. Accurately predict traffic accidents with "High" severity.
2. Minimize the misclassification of "Low" severity as "High."
3. Handle dataset imbalance effectively (70% "High" and 30% "Low").

---

## Key Features

- **Dataset**: Historical traffic accident data.
- **Techniques Used**:
  - Logistic Regression
  - ROC Curve Analysis
  - Threshold Optimization (Youden's J Statistic)
- **Performance Metrics**:
  - Sensitivity (True Positive Rate)
  - Specificity (True Negative Rate)
  - AUC (Area Under the Curve)

---

## Workflow

1. **Data Preprocessing**:
   - Addressed class imbalance using oversampling/undersampling.
   - Engineered features for model training.
2. **Model Training**:
   - Logistic Regression with stepwise feature selection.
   - Evaluated multiple thresholds to balance sensitivity and specificity.
3. **Threshold Selection**:
   - Optimal threshold determined using Youden's J Statistic from ROC analysis.
   - Emphasis on maximizing sensitivity due to project objectives.
4. **Model Evaluation**:
   - Compared training and testing results to validate model performance.

---

## Results

### Final Threshold: **0.54**

| Metric      | Training | Testing |
| ----------- | -------- | ------- |
| Sensitivity | 80.71%   | 80.29%  |
| Specificity | 59.40%   | 24.00%  |

### Observations

- High sensitivity aligns with the primary goal of correctly predicting "High" severity cases.
- Specificity is lower in testing, reflecting trade-offs in imbalanced datasets.

---

## Visualizations

1. **ROC Curve**: Highlights the trade-off between sensitivity and specificity, with AUC as a key metric.
2. **Bar Charts**: Comparison of sensitivity and specificity between training and testing datasets.

---

## Files in Repository

- **`data/`**: Contains processed dataset files.
- **`notebooks/`**: Jupyter Notebooks or R Markdown files with code and analysis.
- **`README.md`**: Project overview and documentation (this file).

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Sarztak/traffic-accident-prediction.git
   ```
2. Install necessary dependencies:
   - R: Install required libraries using `install.packages()`.
3. Run the preprocessing script:
   ```bash
   Rscript notebooks/Traffic Crashes 2024 EDA.Rmd
   ```
4. Train and evaluate the model:
   ```bash
   Rscript notebooks/Traffic Crashes Modelling.Rmd
   ```

---

## Conclusion

This project demonstrates the application of classification techniques to predict traffic accident severity effectively, even in the face of imbalanced datasets. The chosen threshold ensures high sensitivity, aligning with the project's objective of accurately identifying high-severity cases.

---

## Future Work

- Explore additional features for improved model accuracy.
- Apply ensemble methods for better performance.
- Incorporate real-time prediction pipelines.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- Inspiration from city traffic accident data.
- Libraries and tools: R, ggplot2, pROC.
- Guidance from instructors and peers.

---

