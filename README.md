# Student Performance Prediction

This project focuses on predicting students' final grades (`G3`) using various demographic, academic, and social factors. The dataset used for this analysis is sourced from [Kaggle's Student Performance Dataset](https://www.kaggle.com/datasets/impapan/student-performance-data-set).

## Project Structure
1. **Exploratory Data Analysis (EDA)**:
    - Understanding data distribution and feature relationships.
    - Visualizations to explore correlations with the target variable.

2. **Baseline Machine Learning Model**:
    - Built a regression model using `RandomForestRegressor` as a baseline.
    - Evaluated model performance with metrics like MAE, MSE, and R².

3. **Error Analysis**:
    - Investigated model weaknesses by analyzing residuals.
    - Identified overestimations, underestimations, and impactful features.

## Key Features
- Predict students' final grades (`G3`) based on:
  - Demographic details (e.g., `age`, `address`, `famsize`).
  - Academic performance (e.g., `G1`, `G2`, `studytime`).
  - Social and parental factors (e.g., `famsup`, `Medu`, `Fedu`).

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/your-repo-name.git
    ```
2. Navigate to the project directory:
    ```bash
    cd your-repo-name
    ```
3. Install required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
1. Run the analysis script to explore the dataset and build models.
2. Evaluate model performance using the provided metrics and visualizations.
3. Modify the pipeline to improve predictions based on error analysis insights.

## Results
- **Baseline Model**: Achieved an R² score of 0.83 with a `RandomForestRegressor`.
- **Insights**:
  - High residual errors for low grades (extreme cases).
  - Study time and parental support significantly influence predictions.

## Contributions
Feel free to fork this project and create pull requests. Contributions are welcome to improve the pipeline or explore advanced modeling techniques.

## License
This project is licensed under the MIT License.

## Acknowledgments
- Dataset by [Kaggle](https://www.kaggle.com/datasets/impapan/student-performance-data-set).
- Developed with `Python`, `scikit-learn`, `pandas`, and `matplotlib`.
"""
