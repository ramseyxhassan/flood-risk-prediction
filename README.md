# Flood Risk Prediction for Property Owners

![Flood Risk Prediction Screenshot](images/Screenshot%202025-05-16%20192058.png)

## Overview
This project focuses on developing a comprehensive flood risk prediction model for property owners in Baltimore County, Maryland. The aim is to integrate geospatial analysis with environmental and historical flood data to accurately assess flood risks, providing valuable insights for property owners, insurance companies, and local government agencies. By predicting flood vulnerability, this tool helps stakeholders make informed decisions about property investment, insurance coverage, and flood mitigation strategies.

## Project Significance
Flooding represents one of the most common and costly natural disasters in the United States. For Baltimore County specifically, changing climate patterns and increasing urbanization have heightened flood risks in recent years. This project addresses an urgent need for accurate, property-specific flood risk assessment to protect investments and potentially save lives.

## Files in the Project
- `BMC_Dataset_merged_with_FPD_nearest_geom_and_flood_probability.ipynb` - Notebook merging Baltimore County datasets with Flood Probability Data and nearest geometry calculations.
- `bmc_property_assessments_final.ipynb` - Notebook processing the Baltimore County property assessments.
- `expected_loss.ipynb` - Analysis notebook calculating the expected financial loss due to flooding events.
- `Model_Enhancement.ipynb` - Notebook dedicated to enhancing and refining the predictive model.
- `Flood Risk Prediction.pptx` - PowerPoint presentation summarizing key findings and methodology for stakeholders.

## Technologies Used
- **Python** - Primary programming language
- **Libraries**:
  - **Geopandas** - For geospatial data processing
  - **Rasterio** - For raster data analysis
  - **CatBoost** - For gradient boosting machine learning
  - **Pandas** - For data manipulation and analysis
  - **NumPy** - For numerical computing
  - **Matplotlib/Seaborn** - For data visualization
  - **Scikit-learn** - For additional ML functionality
- **Jupyter Notebooks** - For interactive data exploration and visualization
- **GIS Tools** - For spatial analysis and mapping

## Methodology
The project employs a series of Jupyter Notebooks to process and analyze data through the following key steps:

1. **Data Collection & Preprocessing**:
   - Gathering property assessment records from Baltimore County
   - Collecting historical flood data and environmental factors
   - Cleaning and preparing datasets for analysis

2. **Geospatial Analysis**:
   - Merging property assessments with flood probability data
   - Calculating proximity to water bodies and flood zones
   - Utilizing spatial analysis for risk calculation

3. **Model Development**:
   - Feature engineering to identify key risk factors
   - Developing a predictive model using machine learning techniques
   - Training and validating the model with historical data

4. **Risk Assessment**:
   - Calculating expected financial losses
   - Creating risk profiles for different property types
   - Visualizing and communicating the results effectively

## How to Use

### Prerequisites
- Python 3.7+ installed
- Git for version control
- Jupyter Notebook or JupyterLab

### Required Python Libraries
```bash
pandas>=1.3.0
numpy>=1.20.0
matplotlib>=3.4.0
seaborn>=0.11.0
geopandas>=0.10.0
rasterio>=1.2.0
scikit-learn>=0.24.0
catboost>=0.26.0
jupyter>=1.0.0
```

### Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/flood-risk-prediction.git
   cd flood-risk-prediction
   ```

2. Create and activate a virtual environment (recommended):
   ```bash
   python -m venv venv
   # On Windows
   venv\Scripts\activate
   # On macOS/Linux
   source venv/bin/activate
   ```

3. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

### Running the Analysis
1. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

2. Run the notebooks in the following recommended sequence:
   - First: `bmc_property_assessments_final.ipynb` (data preparation)
   - Second: `BMC_Dataset_merged_with_FPD_nearest_geom_and_flood_probability.ipynb` (data merging)
   - Third: `Model_Enhancement.ipynb` (model development)
   - Fourth: `expected_loss.ipynb` (risk assessment)

3. Review the PowerPoint presentation (`Flood Risk Prediction.pptx`) for a summary of findings and methodology.

## Presentation Materials
The `Flood Risk Prediction.pptx` PowerPoint file provides a comprehensive overview of this project, suitable for stakeholder presentations. It includes methodology explanations, key findings, visualizations, and recommendations based on the analysis.
