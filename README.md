# Machine Learning Models for Healthcare

**Authors:** May Sabai (017390438), Thel Nu Zaw ()

## Project Description

This project focuses on developing machine learning models to classify breast tumors as either benign (non-cancerous) or malignant (cancerous). Our goal is to create an accurate classification system that can assist healthcare professionals in making timely and informed decisions about patient care.

### Key Research Questions
• What are the measurements of tumors that can cause breast cancers?
• What other key factors should be considered such as smoothness, textures, and compactness?
• How can we identify differences to help patients prevent cancer at early stages?

## Project Outline/Plan

### Research Objectives
- Develop and compare multiple machine learning models for breast cancer classification
- Analyze the importance of different tumor characteristics in classification accuracy
- Create a robust prediction system that can aid in early cancer detection
- Evaluate model performance using appropriate metrics and validation techniques

## Data Collection Plan

### May Sabai's Data Collection
I have identified two datasets from Kaggle with consistent variables that will be combined to create a comprehensive dataset. The combined dataset will be split into three subsets: training (70%), testing (15%), and validation (15%) to ensure robust model evaluation. The datasets contain various tumor measurements including radius, texture, perimeter, area, smoothness, compactness, concavity, concave points, symmetry, and fractal dimensions.

### Thel Nu Zaw's Data Collection
*[To be completed by partner]*

## Model Plans

### May Sabai's Model Approach
I plan to implement and compare three different machine learning algorithms:
- **Logistic Regression**: For its interpretability and effectiveness with binary classification
- **K-Nearest Neighbors (KNN)**: To leverage local patterns in the data
- **Decision Tree**: For its ability to create clear decision boundaries and feature importance analysis

I have chosen not to use Multi-Layer Perceptron (MLP) or Convolutional Neural Networks (CNN) for this project because the dataset consists of numerical measurements rather than images, and these deep learning approaches would require significantly more computational resources without providing proportional benefits for this type of tabular data classification problem.

### Thel Nu Zaw's Model Approach
*[To be completed by partner]*

## Project Timeline

### Phase 1: Data Preparation (Week 1)
- [ ] Collect dataset 
- [ ] Perform exploratory data analysis 
- [ ] Split data into train/test/validation sets
- [ ] Handle missing values and outliers

### Phase 2: Model Development (Week 2)
- [ ] Implement Logistic Regression model
- [ ] Implement K-Nearest Neighbors model
- [ ] Implement Decision Tree model
- [ ] Perform hyperparameter tuning for each model

### Phase 3: Model Evaluation (Week 3)
- [ ] Compare model performance using appropriate metrics
- [ ] Analyze feature importance
- [ ] Create visualizations for model comparison
- [ ] Document findings and recommendations

### Phase 4: Documentation and Finalization (Week 4)
- [ ] Finalize model selection
- [ ] Create comprehensive documentation
- [ ] Prepare presentation materials
- [ ] Submit final project deliverables

## Repository Structure

```
Projects/
├── README.md
├── .gitignore
├── LICENSE
├── data/
│   ├── train/
│   ├── test/
│   └── validate/
├── notebooks/
│   ├── msb_data_preprocessing.ipynb
│   ├── msb_model_construction.ipynb
│   ├── msb_analysis_and_visualization.ipynb
│   ├── tnz_data_preprocessing.ipynb
│   ├── tnz_model_construction.ipynb
│   └── tnz_analysis_and_visualization.ipynb
└── requirements.txt
```

## Getting Started

### Prerequisites
- Python 3.8+
- Jupyter Notebook
- Required Python packages (see requirements.txt)

### Installation
1. Clone the repository
2. Install required packages: `pip install -r requirements.txt`
3. Run the notebooks in sequence

## Expected Outcomes

- A comparative analysis of three machine learning models for breast cancer classification
- Identification of the most important features for tumor classification
- A robust classification system with documented performance metrics
- Insights into early-stage cancer detection factors

## Contributing

This is a collaborative project between May Sabai and Thel Nu Zaw. Each author is responsible for their respective data collection and model development components.

## License

This project is licensed under the SJSU CS171 License - see the LICENSE file for details.
