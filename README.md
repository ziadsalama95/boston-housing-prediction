# Boston Housing Price Prediction

This project involves predicting housing prices using the Boston Housing Dataset. The dataset contains information about houses in Boston, including features such as crime rate, property tax rate, and the number of rooms, along with the target variable `MEDV` (Median Value of Owner-Occupied Homes).

## Project Workflow

### 1. Dataset Overview
The Boston Housing Dataset contains 506 rows and 14 columns:
- **Features**: CRIM, ZN, INDUS, CHAS, NOX, RM, AGE, DIS, RAD, TAX, PTRATIO, B, LSTAT
- **Target**: MEDV (Median Value of Homes in $1000s)

### 2. Tasks Completed

#### Exploratory Data Analysis (EDA)
- Analyzed feature distributions and checked for correlations with the target variable.
- Visualized relationships using scatter plots and heatmaps.

#### Data Preprocessing
- Identified and handled outliers using the IQR method.
- Scaled features using `StandardScaler` to ensure proper gradient descent performance.
- Split data into training and testing sets (80% train, 20% test).

#### Model Implementation
- Implemented gradient descent from scratch for linear regression.
- Visualized cost function convergence for different learning rates.
- Compared results with Scikit-learn's `LinearRegression` implementation.

#### Hyperparameter Tuning
- Experimented with learning rates (e.g., 0.001, 0.01, 0.1) to observe their impact on convergence.

#### Evaluation
- Evaluated models using:
  - **Mean Squared Error (MSE)**
  - **R-squared**
- Compared performance of the custom gradient descent implementation with Scikit-learn.

### 3. Key Findings
- Strong correlations were observed between `RM` (average number of rooms per dwelling) and `MEDV`.
- Lower learning rates (e.g., 0.01) resulted in better convergence of the cost function.
- The custom gradient descent implementation performed similarly to Scikit-learn's linear regression for this dataset.

### 4. Challenges Faced
- Handling outliers without losing important data.
- Tuning learning rates to ensure convergence without overshooting.

### 5. Lessons Learned
- Scaling features is crucial for gradient descent.
- Visualization aids in understanding data relationships and model performance.

## How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/ziadsalama95/boston-housing-prediction.git
   ```

2. Navigate to the project directory:
   ```bash
   cd boston-housing-prediction
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Open the Jupyter notebook:
   ```bash
   jupyter notebook Boston_Housing_Prediction.ipynb
   ```

5. Run all cells to see the analysis, model implementation, and results.

## Dependencies
- Python 3.8+
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Repository Structure
```
.
├── Boston_Housing_Prediction.ipynb  # Main analysis and implementation notebook
├── README.md                        # Project documentation
└── housing.csv                      # Dataset
```

## Author
[Ziad Salama](https://github.com/ziadsalama95)

## License
This project is licensed under the MIT License.
