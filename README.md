# DS 4420 Final Project
 Final Project for ML 2

# Objectives
Wildfires pose an increasing threat to ecosystems, human populations, and infrastructure, particularly in regions prone to extreme heat and drought. The ability to predict wildfires and estimate their severity is important for efficient resource allocation and risk mitigation. Traditional wildfire prediction models rely on meteorological data, historical fire records, and vegetation indices. However, advances in machine learning provide new opportunities to enhance the accuracy and efficiency of these predictions.

We aim to develop a dual-method ML approach to predict wildfires and their severity, leveraging convolutional neural networks (CNNs) for image-based fire detection and multilayer perceptrons (MLPs) for predictive analysis. Specifically, CNNs are applied to RGB imagery and aerial photographs of past wildfires to detect early-stage fires and assess their spatial patterns. MLPs will be used to analyze preexisting numerical data, such as temperature (C), FFMC indices, and relative humidity to estimate the magnitude of wildfire damage in terms of hectares (Canada Natural Resources). By combining these two models, we aim to build the framework for identifying fires using image data and then predicting their severities with numerical data. While these two datasets are different in location and context, they provide a complementary foundation for developing and testing the dual-model framework, with future work focusing on unifying geographic and temporal data to improve model integration.


## Repository Structure

```
DS-4420-Final-Project/
│
├── data/
│   ├── satellite/         # photos folder
        ├── test            # test data files
            ├── fire
            ├── nofire      
        ├── train          # train data files
            ├── fire
            ├── nofire      
        ├── val            # val data files
            ├── fire
            ├── nofire      
│
├── cnn_script_final.ipynb
├── mlp_script_final.Rmd 
├── DS4420_Poster_Min_Pan.pdf
├── DS4420_Poster_Min_Pan.pptx
├── DS4420_Report_Min_Pan.pdf
├── requirements.txt       # dependencies
└── README.md              # Project overview
```

## Getting Started

### Prerequisites
- Python 3.8 or higher
- Install dependencies using:
    ```bash
    pip install -r requirements.txt
    ```

### Data Collection
Download data from these sources:

1. https://www.kaggle.com/datasets/balavashan/forest-fire-dataset
2. https://www.kaggle.com/datasets/elmadafri/the-wildfire-dataset

### Running the Project
1. Run either script when data folder is complete
