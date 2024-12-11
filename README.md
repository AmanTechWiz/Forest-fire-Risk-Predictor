# Forest Fire Risk Predictor

## Overview
The **Forest Fire Risk Predictor** is a web application built using Flask that predicts the Fire Weather Index (FWI) based on various weather-related inputs. It leverages machine learning to assist in estimating the risk of forest fires, providing a valuable tool for environmental monitoring and risk management.

## Features
- **Interactive UI**: Easy-to-use interface for inputting weather data.
- **Machine Learning Integration**: Predicts FWI using pre-trained models (Ridge/Lasso Regression).
- **Scalable**: Ready for deployment on local or cloud platforms.
- **Lightweight**: Built with Python and Flask for efficient performance.

## Application Preview

![Application UI](image-link-placeholder)

## Installation

Follow these steps to set up and run the project on your local machine:

### Prerequisites
- Python 3.7+
- pip (Python package installer)

### Clone the Repository
```bash
https://github.com/your-username/forest-fire-risk-predictor.git
cd forest-fire-risk-predictor
```

### Install Dependencies
Install all the required Python packages using pip:
```bash
pip install -r requirements.txt
```

### Run the Flask Application
```bash
python application.py
```

The application will run locally on `http://127.0.0.1:5000/`.

## Usage
1. Open the application in your browser.
2. Input the following parameters:
   - **Temperature** (in Celsius)
   - **Relative Humidity (RH)** (in %)
   - **Wind Speed (Ws)** (in km/h)
   - **Rain** (total rainfall in mm)
   - **FFMC** (Fine Fuel Moisture Code)
   - **DMC** (Duff Moisture Code)
   - **ISI** (Initial Spread Index)
   - **Classes** (Fire/No Fire)
   - **Region**
3. Click on the `Predict Forest Fire Risk` button.
4. View the predicted Fire Weather Index (FWI).

## File Structure
```
forest-fire-risk-predictor/
|
├── static/              # Static files (CSS, JS, Images)
├── templates/           # HTML templates for Flask app
├── application.py       # Main Flask application file
├── scaler.pkl           # Pre-trained scaler model
├── ridge.pkl            # Pre-trained Ridge regression model
├── lasso.pkl            # Pre-trained Lasso regression model
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation
```

## Technologies Used
- **Backend**: Flask, Python
- **Frontend**: HTML, CSS
- **Machine Learning**: Ridge Regression

## Dataset
The dataset contains weather observations and FWI components, including:
- Temperature
- Relative Humidity
- Wind Speed
- Rain
- FFMC, DMC, ISI indices

The dataset was used to train the models to predict the Fire Weather Index.

## Contributions
Contributions are welcome! If you'd like to add new features, fix bugs, or improve the documentation, feel free to create a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

