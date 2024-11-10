# McKinley Park Air Quality Monitoring Project

## Background & Objectives
In 2008, MAT Asphalt, Chicago's largest asphalt factory, began operations in McKinley Park, a working-class neighborhood on the city’s southwest side. Residents soon noticed sulfur and ammonia-like odors, leading to concerns about air quality. The community formed Neighbors for Environmental Justice (N4EJ) and installed real-time sensors, which indicated elevated particulate matter (PM) levels near the factory. Since PM data alone couldn't fully identify the source, our team began a comprehensive air monitoring project to measure a broader range of pollutants, including SO₂ and VOCs like benzene and toluene, using high-resolution mobile monitoring.

## Project Setup
We developed a mobile air monitoring system with a GPS, a Gasmet DX4040 FTIR Gas Analyzer, and a DustTrak II Monitor. This setup captures high-resolution air quality data that can help differentiate pollution from various sources, such as railyards, highways, and nearby industrial facilities.

## Data Processing & Analysis
1. **Data Import & Preparation**  
   GPS and DX4040 data were cleaned and synchronized by time, with outliers and initial unstable measurements removed. DX4040 timestamps were formatted, and GPS duplicates were managed by averaging coordinates. To align the data, a continuous GPS time series was created and matched to DX4040 intervals.

2. **Chemical Concentration Mapping**  
   Using rasterized means to standardize chemical concentration values, we created spatial maps to visualize pollutant distributions across the neighborhood.

3. **Comparison of Operating vs. Non-Operating Periods**  
   Using Wilcoxon rank-sum tests, we compared chemical concentrations when the factory was operating (Nov 2023) versus not operating (Feb 2024). Higher levels of 2-Ethyltoluene, Carbon Tetrachloride, and trans-1,3-Dichloropropene were observed during operation.

4. **Directional Analysis Relative to Wind**  
   Data collected downstream from the prevailing wind showed higher levels of certain pollutants, including Ethylbenzene, suggesting the factory’s impact on local air quality.

5. **Distance-Based Analysis**  
   Linear regression models assessing the relationship between factory distance and chemical concentrations indicated a weak correlation, suggesting other factors may contribute to pollutant dispersion.

This project enhances understanding of air quality issues in the McKinley Park neighborhood, and the system we developed can be adapted for use in other settings. Detailed methodology and findings are available in the full report.
