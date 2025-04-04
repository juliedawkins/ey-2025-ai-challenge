# EY 2025 Open Science AI and Data Challenge: Cooling Urban Heat Islands

### Final Results: Top 50 on Final Leaderboard of 23,000 Model Submissions, R-Squared: 0.973

#### Discussion and Thoughts on Final Model
Though my model had a high R-squared and strong predictive power, it lacked interpretability—a key limitation. The final model used 196 variables, many of which were spatial features at varying buffer distances (e.g., building density at 50, 100, 150 meters) or raw spectral bands, which are not easily interpretable or directly actionable for urban designers. Still, this project deepened my understanding of geospatial modeling and the tradeoffs between model accuracy and interpretability. It also demonstrated my ability to handle complex spatial data and build a highly predictive machine learning pipeline from satellite imagery. 

#### Contents
Preprocessing: Loads the .tiff file, extracts relevant features, and sets up the spatial data.
Modeling: Applies a machine learning model (in this case, XGBoost) to predict UHI index values.
Output: Saves a raster of predicted values for further analysis or visualization.

#### Notes
Only the s2.tiff file was uploaded to avoid potential licensing or privacy issues with other datasets. All external data used in the notebook should be presumed to be either public or derived from open satellite imagery.

#### Dependencies
rasterio
numpy
scikit-learn
rtree
pandas
shapely

#### Usage
To run the notebook:
Ensure you have the s2.tiff file in your working directory.
Open the notebook in Jupyter or VSCode.
Execute all cells in order.

