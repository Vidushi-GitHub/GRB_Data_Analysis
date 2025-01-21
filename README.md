# GRB Data Analysis Using 3ML

This repository provides a comprehensive guide for performing Gamma-Ray Burst (GRB) data analysis using the Multi-Mission Maximum Likelihood (3ML). 
It is designed to facilitate the complete analysis of Fermi data, from light curve extraction to spectrum fitting.

### 1. **Light Curve Extraction and Analysis**
This part of the code demonstrates how to extract and analyze the composite light curve for Fermi's various detectors, including NaI, BGO, LLE and LAT detectors.

The steps involved are:
- **Extraction and Plotting**: The code extracts data from multiple Fermi detectors and plots the composite light curve, providing a visual overview of the GRB's time evolution.
- **Time-Resolved Binning**: Using 3ML commands, the code performs time binning for more detailed analysis of the GRB over different time intervals.
- **PHAII File Generation**: The binned data is then written to a PHAII type file, which is used for subsequent spectral analysis.

### 2. **Spectrum Analysis**
This part of the code focuses on spectral analysis of the Fermi GBM and LLE data, includes:
- **Data Input**: The code can read Fermi's GBM + LLE data files using the 3ML plugin, making the data input process straightforward.
- **Model Fitting**: The spectral data is fitted using empirical models, such as **Band Model**, **BandHighecut Model**.
- **Bayesian Blocks Analysis**: The code incorporates Bayesian blocks for time-segmented analysis, tracing the evolution in lightcurve.
- **Fit Parameter Evolution**: The code generates plots that show the evolution of fit parameters over time and stores these results for further analysis.

## Requirements
- **3ML**: Python based tool for data analysis and modeling.
- **Fermi Data**: Data files from Fermi's GBM, LLE and LAT detectors.
- **Python**: The programming language used for analysis.

## Conclusion
This repository provides an easy-to-follow implementation of GRB data analysis using 3ML, enabling users to perform both light curve and spectrum analysis on Fermi data.
