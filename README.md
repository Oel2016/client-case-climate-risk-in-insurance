# Wildfire and Excess Rain Insurance Pricing

This project is aimed at providing a tailored insurance pricing model for a client in Australia with forestry plantations. The focus is on two main perils that can damage the forests: **wildfires** and **excessive rain**. These are the primary climate risks we specialize in at Square Management.

## Structure of the Repository
The repository contains two Jupyter notebooks:

### 1. Excess of Rain Insurance Pricing (1st Notebook)
This notebook deals with the pricing of an excess of rain insurance cover for the client. The steps include:
- **Load Data**: Import and preprocess historical precipitation data.
- **Data Manipulation**: Adjust raster resolutions and filter data for forest areas.
- **Preprocessing**: Process daily precipitation data for the client's risk period (Dec-Mar).
- **Pricing**: Calculate cumulative rainfall and compute payouts based on thresholds (650mm deductible, 750mm cap).
  
### 2. Wildfire Insurance Pricing (2nd Notebook)
This notebook focuses on wildfire risk, specifically the ignition phase. The steps include:
- **Historical Ignition Points**: Collect data on historical ignition points, including temperature and vegetation type for each incident.
- **Ignition Probability Model**: Use the historical ignition data to train a classification algorithm to predict the likelihood of ignition.
  
The goal is to use this model to simulate ignition events and better understand the risk of wildfires in the client's plantations.

## Requirements:
- `xarray`
- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn` (for classification model)

## Output:
- **Excess Rain**: Historical payouts based on past precipitation data.
- **Wildfire**: An ignition probability model to forecast the likelihood of future wildfires based on environmental factors.

