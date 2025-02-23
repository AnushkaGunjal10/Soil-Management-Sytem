# Soil Management System

## Overview
The Soil Management System is a Streamlit-based web application that provides crop recommendations based on soil characteristics using Google's Gemini API. It also stores recommendations in a MySQL database.

## Features
- Takes soil characteristics as input (soil type, nitrogen, phosphorus, potassium, pH, moisture).
- Uses the Gemini API to generate crop recommendations.
- Stores recommendations in a MySQL database.
- Custom UI with color themes and borders for better user experience.

## Technologies Used
- Python
- Streamlit
- Google Gemini API
- MySQL
- HTML & CSS (for UI customization)

## Installation & Setup

### Prerequisites
Ensure you have the following installed:
- Python (>=3.7)
- MySQL Database
- Streamlit
- Google Generative AI SDK

### Install Dependencies
```bash
pip install streamlit mysql-connector-python google-generativeai
```

### Configure API Key
Replace `your_gemini_api_key` in `API_KEY` with your valid Google Gemini API key.

### Configure MySQL Database
Update the database connection details in the script:
```python
conn = mysql.connector.connect(
    host="your_db_host",
    user="your_db_user",
    password="your_db_password",
    database="your_db_name"
)
```

Ensure that a MySQL database named `your_db_name` exists.

### Run the Application
```bash
streamlit run soil_management.py
```

## Usage
1. Open the web app in a browser.
2. Select soil type and enter required values.
3. Click **Get Crop Recommendation** to receive suggestions.
4. Recommendations will be displayed in a bordered yellow box.

## Customization
- Change background color by modifying `background-color` in the CSS section of the script.
- Adjust the UI elements by editing Streamlit components.

## License
This project is for educational purposes. Modify and use as needed!

