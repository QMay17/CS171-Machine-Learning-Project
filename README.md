# Machine Learning Models for Healthcare

**Authors:** May Sabai (017390438), Thel Nu Zaw (017891302)

## Project Description

This project focuses on developing machine learning models to classify breast tumors as either benign (non-cancerous) or malignant (cancerous). Our goal is to create an accurate classification system that can assist healthcare professionals in making timely and informed decisions about patient care.

### Key Research Questions
- What are the measurements of tumors that can cause breast cancers?
- What other key factors should be considered such as smoothness, textures, and compactness?
- How can we identify differences to help patients prevent cancer at early stages?
- Which machine learning algorithms provide the highest accuracy in classifying breast tumors?
- How do tumor size, location, and stage affect the likelihood of sperad in breast cancer patients?

## Project Outline/Plan

### Research Objectives
- Develop and compare multiple machine learning models for breast cancer classification
- Analyze the importance of different tumor characteristics in classification accuracy
- Create a robust prediction system that can aid in early cancer detection
- Evaluate model performance using appropriate metrics and validation techniques

## Data Collection Plan

### May Sabai's Data Collection
I have identified breast ultrasound image datasets that will be used for training a deep learning model. The dataset contains ultrasound images of breast tumors classified as benign, malignant, or normal. The images will be split into three subsets: training (70%), testing (15%), and validation (15%) to ensure robust model evaluation. Using ultrasound images allows for direct visual analysis of tumor characteristics and patterns that may not be captured through numerical measurements alone.

### Thel Nu Zaw's Data Collection
I have selected the Breast Cancer Wisconsin Data Set from UCI Machine Learning Repository. This dataset conatin various tumor measurements which are consistent with the features used in Kaggle dataset so that dataset can be combined to test together. The final dataset will be split into training(70%), testing(15%), and validation(15%) subsets to ensure a fair and vigorous evaluation of the models.

## Model Plans

### May Sabai's Model Approach
I plan to implement a **Convolutional Neural Network (CNN)** for breast cancer classification from ultrasound images. CNNs are particularly well-suited for this task because they can:
- Automatically extract relevant visual features from the ultrasound images
- Learn hierarchical representations of tumor characteristics
- Detect spatial patterns and textures that may indicate malignancy
- Handle the complexity of medical image analysis

The CNN architecture will include multiple convolutional layers for feature extraction, pooling layers for dimensionality reduction, and fully connected layers for classification. I will experiment with different architectures, activation functions, and regularization techniques to optimize model performance. Data augmentation techniques such as rotation, flipping, and zoom will be applied to increase the robustness of the model and prevent overfitting.

### Thel Nu Zaw's Model Approach
I will use Scikit-Learn throughout the project for both data preprocessing and model construction. First, I will apply StandardScaler to normalize all 30 numerical features so that measurements such as radius, area, and concavity are placed on comparable scales. The scaler will be fit only on the training data to prevent data leakage and then applied to the validation and test sets. For modeling, I will implement Logistic Regression as an interpretable baseline, KNN to capture local neighborhood patterns, and a Decision Tree to learn non-linear decision boundaries. I will also combine these models using a Majority Voting Ensemble to improve overall prediction stability. All models will be trained and evaluated using the same train/validation/test split in Scikit-Learn, and performance will be measured using accuracy, precision, recall, F1-score, ROC curves, and confusion matrices to ensure fair and consistent comparison across approaches. The best model will be selected based on validation and test performance and will be used for further analysis and visualization.

## Project Timeline

### Phase 1: Data Preparation (Week 1)
- [ ] Collect dataset 
- [ ] Perform exploratory data analysis 
- [ ] Split data into train/test/validation sets
- [ ] Handle missing values and outliers

### Phase 2: Model Development (Week 2)
- [ ] Implement machine learning models (CNN for image data, traditional ML for numerical data)
- [ ] Design and build CNN architecture for image classification
- [ ] Train models with appropriate data preprocessing
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
│   ├── Dataset_BUSI_with_GT/
│   ├── train/
│   ├── test/
│   ├── validate/
│   ├── test_split.csv 
│   ├── train_split.csv
│   ├── validate_split.csv
└── └── scaler.pkl
├── notebooks/
│   ├── analysis_and_visualization.ipynb
│   ├── msb_data_preprocessing.ipynb
│   ├── msb_model_construction.ipynb
│   ├── tnz_data_preprocessing.ipynb
│   ├── tnz_model_construction.ipynb
└── └── wdbc.data
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

- A comparative analysis of machine learning models for breast cancer classification (CNN for image data and traditional ML for numerical data)
- Identification of the most important features and visual patterns for tumor classification
- A robust classification system with documented performance metrics
- Insights into early-stage cancer detection factors

## Contributing

This is a collaborative project between May Sabai and Thel Nu Zaw. Each author is responsible for their respective data collection and model development components.

## License

This project is licensed under the SJSU CS171 License - see the LICENSE file for details.
