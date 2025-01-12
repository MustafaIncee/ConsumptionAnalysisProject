# ConsumptionAnalysisProject

# Turkish Electricity Market Forecasting

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-orange)
![Data](https://img.shields.io/badge/Data-EPIAS-green)

A deep learning project for forecasting electricity production and consumption in the Turkish electricity market using state-of-the-art transformer architectures.

## Project Overview

This project aims to predict hourly electricity production and consumption values using real-time data from EPIAS (Energy Exchange Istanbul). We implement various transformer-based models to analyze historical data patterns including total electricity generation, consumption, and detailed generation by source.

## Features

### Data Sources
- Hourly electricity consumption (2018-2024)
- Detailed generation data by source:
  - Natural Gas
  - Hydro (Dammed & River)
  - Wind & Solar
  - Coal (Import, Lignite, Black)
  - Geothermal
  - Biomass and others

### Implemented Models
- **Autoformer**: Enhanced transformer with auto-correlation mechanism
- **Informer**: Efficient transformer for long sequence forecasting
- **Pyraformer**: Pyramid attention mechanism
- **ETSformer**: Exponential smoothing inspired architecture
- **FEDformer**: Frequency enhanced decomposed transformer
- **LSTM**: Traditional deep learning baseline

### Feature Engineering
- Time-based features (hour, day, month)
- Lag features (24h, 168h, 336h)
- Rolling statistics
- Seasonal decomposition

## Results

Best performing model (Pyraformer) achieved:
- MAPE: 2.21%
- RMSE: 1173.96 MW
- MAE: 842.03 MW
- MSE: 1378191.88
- R²: 0.9657

## Installation & Usage
Clone repository
!git clone https://github.com/MustafaIncee/ConsumptionAnalysisProject.git


## Applications

This project can be valuable for:
- Power plant operators for production planning
- Energy traders for market strategies
- Grid operators for demand forecasting
- Policy makers for energy planning

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
