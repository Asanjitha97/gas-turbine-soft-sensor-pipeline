Gas Turbine Emission Soft Sensor PipelineOverview.

This repository contains a machine learning pipeline that acts as a soft sensor to estimate hard-to-measure Carbon Monoxide (CO) emissions from a gas turbine. The thermodynamics of a gas turbine, compressing air, combusting fuel, and spinning turbine blades at over 3,000 RPM create complex, non-linear physical relationships. This project bridges the gap between those physical mechanical realities and data-driven modeling.   

Key Features: 
Algorithm Robustness & Anomaly Detection: Physical sensors operating in extreme environments inevitably degrade or drift. 

Data Reduction: Gas turbines utilize hundreds of sensors, causing massive multicollinearity. I applied Principal Component Analysis (PCA) to compress highly correlated physical phenomena (like overlapping exhaust pressures and turbine temperatures) down to 7 principal components, retaining 95% of the variance.  

Virtual Estimation: Trained a Random Forest Regressor on the reduced dataset to accurately predict CO emissions, circumventing the need for expensive, direct physical emission sensors.
