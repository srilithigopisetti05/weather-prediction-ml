🌦 Weather Predictor for Farmers
Hey there! Welcome to the Weather Predictor Project — a machine learning system that predicts hailstorms and rainfall in advance to give farmers a heads-up and help protect their crops. Think of it as your digital crop bodyguard. 🌱💧

🎯 Project Objective
Predict hail and rain using weather data.
Serve predictions via a simple API.
Help farmers make timely decisions to save their crops.
🧐 Problem Statement
Unexpected weather events like hailstorms can *destroy crops in hours. Traditional forecasts aren’t always localized or timely, leaving farmers vulnerable. This project solves that problem with *machine learning + real-time alerts.

🛠 Tools & Technologies
Python 3.x – main programming language
Pandas & NumPy – data preprocessing
Scikit-learn – ML models
Joblib – save/load models
Flask – API server
Git & GitHub – version control
📂 Folder Structure
---data -raw -processed ---models ---notebooks ---src -alerting_py -data_ingest.py -serve_model.py -train_model.py ---requirements.txt ---test_api.py

🚀 How to Run
Clone the repo git clone https://github.com//weather-warning-system-ml.git cd weather-warning-system-ml

Create & activate virtual environment~ python -m venv venv

Windows
venv\Scripts\activate

Mac/Linux
source venv/bin/activate

Install dependencies~ pip install -r requirements.txt

Process the data ~ python src/data_ingest.py

Train the models~ python src/train_model.py

Run the API~ python src/serve_model.py

Test the API ~ python test_api.py

💡 Example API Request~ import requests

url = "http://127.0.0.1:8080/predict" data = {"temp": 32, "humidity": 70, "pressure": 1005,"uwind": 3,"vwind": 2, "rain": 1,"shear_sfc300": 10,"hour": 14,"dayofyear": 200}

response = requests.post(url, json=data) print(response.json())

Expected response: {"prediction": 0} 0 = No hail/rain, 1 = Hail/rain predicted ✅
📈 Expected Outcomes~ -Cleaned & processed weather data. -Trained ML models for hail and rain predictions. -Flask API serving real-time predictions. -Farmers can get timely alerts.\
Conclusion ~ This project bridges course theory with real-world application, using ML to solve agricultural problems. Farmers get early warnings, and we get to see theory in action.
