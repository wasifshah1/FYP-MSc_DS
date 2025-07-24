# Digital Service User Behavior and Churn Analysis

A comprehensive machine learning project analyzing digital service user behavior patterns and predicting customer churn using advanced data science techniques.

## Project Overview

This project addresses three key research questions:
1. How can we group digital service users based on their usage habits?
2. How does customer background information impact churn prediction accuracy?
3. Can we improve churn prediction by combining usage patterns with personal profiles?

## Key Features

### Data Analysis
- Comprehensive exploratory data analysis
- Customer segmentation using K-means clustering
- Statistical analysis of user behavior patterns
- Data quality assessment and cleaning

### Feature Engineering
- Advanced feature creation from usage patterns
- Background information integration
- Data balancing using SMOTE technique
- Feature scaling and normalization

### Machine Learning Models
- Logistic Regression with hyperparameter tuning
- Random Forest Classifier
- XGBoost Classifier
- Model comparison and evaluation
- SHAP analysis for interpretability

## Installation

1. Clone or download the project
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter notebooks in order:
   - Start with `01_EDA_Analysis.ipynb`
   - Continue with `02_Data_Preprocessing.ipynb`
   - Finish with `03_Model_Training.ipynb`

## Usage

### Running Individual Notebooks

```bash
# Start Jupyter Lab
jupyter lab

# Or Jupyter Notebook
jupyter notebook
```

### Running Complete Analysis

```python
# Import and run complete analysis
from complete_analysis import run_full_analysis
results = run_full_analysis('Customer Churn.csv')
```

## Results Summary

### Model Performance Comparison

| Metric | Logistic Regression | Random Forest | XGBoost |
|----------|-----------------|---------------|-----------|
| CV Score | 0.9510          | 0.9962        | **0.9975**
| Accuracy | 0.8587          | 0.9603        | **0.9683**
| Precision| 0.5301          | 0.8627        | **0.8762**
| Recall   | 0.8889          | 0.8889        | **0.9293**
| F1-Score | 0.6642          | 0.8756        | **0.9020**
| AUC      | 0.9462          | 0.9861        | **0.9900**

### User Segmentation
- Identified 4 distinct user segments:
  - High-Value Users (Premium customers)
  - Budget Conscious (Cost-sensitive users)
  - Heavy Communicators (High usage customers)
  - At-Risk Users (Potential churners)

### Best Model Performance (XGBoost)
- **AUC Score: 0.9900** (Excellent discrimination ability)
- **Accuracy: 96.83%** (Outstanding overall performance)
- **Precision: 87.62%** (High reliability in churn predictions)
- **Recall: 92.93%** (Excellent at identifying actual churners)
- **F1-Score: 90.20%** (Balanced precision and recall)
- **CV Score: 99.75%** (Exceptional cross-validation performance)

### Key Insights
- Background features significantly improve prediction accuracy
- Combined feature approach outperforms usage-only models
- Customer complaints and call failures are strong churn indicators
- Usage patterns vary significantly across customer segments
- XGBoost achieved near-perfect performance with 99% AUC score

## Business Recommendations

1. Focus on customers with high complaint rates and call failures
2. Monitor usage patterns for early churn indicators
3. Implement targeted retention campaigns for high-risk segments
4. Improve service quality to reduce complaints and call failures
5. Develop personalized offers based on customer value and tenure

## Technical Requirements

- Python 3.8+
- Jupyter Notebook/Lab
- Required packages listed in requirements.txt
- Minimum 4GB RAM recommended
- 2GB free disk space

## Data Description

The dataset contains customer information including:
- Usage metrics (seconds of use, frequency, SMS usage)
- Background information (age, tariff plan, customer value)
- Service quality metrics (complaints, call failures)
- Target variable (churn status)

## Model Interpretability

- SHAP analysis for feature importance
- Model-agnostic explanations
- Business-friendly insights
- Actionable recommendations

## Methodology

### Part 1: Exploratory Data Analysis
- Data exploration and visualization
- Customer segmentation using K-means clustering
- Statistical analysis of user behavior
- Identification of key patterns and trends

### Part 2: Data Preprocessing
- Data cleaning and quality assessment
- Feature engineering and creation
- Data balancing using SMOTE
- Feature scaling and normalization

### Part 3: Model Training
- Multiple algorithm implementation
- Hyperparameter tuning with grid search
- Cross-validation and model evaluation
- SHAP analysis for interpretability

## Research Questions Answered

1. **User Segmentation**: Successfully identified 4 distinct user segments based on usage habits using K-means clustering
2. **Background Impact**: Demonstrated that background features improve churn prediction accuracy significantly
3. **Combined Approach**: Proved that combining usage patterns with personal profiles achieves exceptional prediction performance (99% AUC)

## Model Comparison Results

- **Logistic Regression**: Good baseline performance (94.62% AUC)
- **Random Forest**: Strong performance (98.61% AUC) with good interpretability
- **XGBoost**: Best performance (99.00% AUC) with superior metrics across all measures

The XGBoost model demonstrates exceptional performance with near-perfect discrimination ability and outstanding precision-recall balance.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## License

This project is for educational and research purposes.

## Contact

For questions or collaboration opportunities, please contact me.

My Email: Swasif41@gmail.com


## Acknowledgments

- Data science community for methodological guidance
- Open source libraries that made this analysis possible
- Academic research in customer churn prediction
