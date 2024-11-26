# Hotel Booking Analysis: Machine Learning Project
![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
![scikit-learn](https://img.shields.io/badge/scikit--learn-Latest-orange)
![License](https://img.shields.io/badge/License-MIT-green)
![Author](https://img.shields.io/badge/Author-Malikus%20Syafaadi%20Nurfaza-blue)

## Overview 
This project implements advanced machine learning techniques to analyze hotel booking patterns, providing valuable insights for the hospitality industry. Part of the IDCamp Machine Learning program by Dicoding, this analysis combines clustering and classification approaches to understand and predict customer booking behaviors.

### Project Objectives
1. Segment hotel customers using unsupervised learning techniques
2. Develop predictive models for booking pattern classification
3. Extract actionable business insights from the analysis

## Methodology

### 1. Data Analysis and Preprocessing
- Dataset: Hotel Booking Demand dataset from Kaggle
- Features: Both categorical (hotel type, customer type) and numerical (lead time, ADR)
- Preprocessing steps:
  - Data cleaning and normalization
  - Feature engineering
  - Handling missing values
  - Encoding categorical variables

### 2. Clustering Analysis
#### Implementation
- Algorithm: K-Means Clustering
- Validation: Silhouette Score Analysis
- Feature Selection: Focused on booking behavior indicators

#### Results
- **Silhouette Score: 0.58** (exceeding requirement of 0.55)
- **Identified Clusters:**
  - Cluster 0 (36,107 bookings): Budget-conscious travelers
    * Short lead times
    * Lower ADR
    * Minimal special requests
  - Cluster 1 (50,548 bookings): Premium guests
    * Extended lead times
    * Higher ADR
    * Multiple special requests

### 3. Classification Analysis
#### Model Development
Implemented three different algorithms:
1. **Random Forest Classifier**
   - Ensemble learning approach
   - Optimal for complex patterns
   - Feature importance ranking

2. **Logistic Regression**
   - Baseline linear model
   - Interpretable results
   - Efficient computation

3. **Support Vector Machine**
   - Non-linear classification
   - Kernel-based approach
   - High-dimensional handling

#### Performance Metrics

| Model | Accuracy | F1-Score | Precision | Recall |
|-------|----------|----------|-----------|---------|
| Random Forest | 100.00% | 100.00% | 100.00% | 100.00% |
| Logistic Regression | 99.99% | 99.99% | 100.00% | 99.99% |
| SVM | 99.91% | 99.91% | 99.91% | 99.91% |

*All models exceeded the minimum requirement of 87% accuracy*

## Key Findings and Business Insights

### 1. Customer Segmentation
- Clear distinction between budget and premium segments
- Booking lead time strongly correlates with spending patterns
- Special requests indicate customer value potential

### 2. Predictive Patterns
- Advance bookings typically indicate higher revenue
- Weekend stays show distinct behavioral patterns
- Seasonal trends affect booking preferences

### 3. Business Recommendations
- Implement segment-specific pricing strategies
- Optimize resource allocation based on booking patterns
- Develop targeted marketing campaigns per segment

## Project Structure
```
submission/
├── [Clustering]_Submission_Akhir_BMLP_Malikus_Syafaadi_Nurfaza.ipynb    # Clustering analysis
├── [Klasifikasi]_Submission_Akhir_BMLP_Malikus_Syafaadi_Nurfaza.ipynb   # Classification analysis
├── clustering_results.csv      # Clustering output
├── hotel_bookings.csv         # Original dataset
├── requirements.txt           # Project dependencies
├── LICENSE                    # MIT License
└── README.md                  # Project documentation
```

## Technical Requirements
- Python 3.7+
- Key Dependencies:
  ```
  numpy>=1.21.0
  pandas>=1.3.0
  scikit-learn>=1.0.0
  matplotlib>=3.4.0
  seaborn>=0.11.0
  jupyter>=1.0.0
  notebook>=6.4.0
  ```

## Installation and Usage

1. Clone the repository:
```bash
git clone [repository-url]
```

2. Create and activate virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Run Jupyter notebooks:
```bash
jupyter notebook
```

## Author
**Malikus Syafaadi Nurfaza**
- GitHub: [@Malikusfz](https://github.com/Malikusfz)
- LinkedIn: [Malikus Syafaadi Nurfaza](https://www.linkedin.com/in/malikussyafaadinurfaza/)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Dicoding and IDCamp for the learning opportunity
- Hotel Bookings dataset providers
- scikit-learn community for excellent documentation
