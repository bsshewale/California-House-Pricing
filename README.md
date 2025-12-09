# 🏡 California House Pricing – End-to-End ML Project
### Software and tools requirements
1. Github
2. Heroku
3. VS code
4. GitCLI

---

This project builds a **Machine Learning regression model** to predict California housing prices using the famous **California Housing dataset**.
The project includes **data preprocessing, model training, evaluation, serialization (pickle), and Flask deployment**, making it a complete ML pipeline ready for production.

---

## 🚀 Features of This Project

### 🔍 1. Data Preprocessing

* Handling missing values
* Feature scaling using **StandardScaler**
* Train-test splitting
* Saving the scaler as `scaler.pkl`

### 🤖 2. ML Model Development

* Linear Regression model
* Model evaluation using MAE, MSE, RMSE
* Model export as `model.pkl`

### 🌐 3. Flask API Deployment

A Flask web app that:

* Loads the trained model
* Loads the scaler
* Accepts new input features
* Returns predicted house price as JSON

### 🧰 4. Tools & Technologies

| Tool / Library    | Purpose               |
| ----------------- | --------------------- |
| Python            | Core development      |
| Pandas, NumPy     | Data manipulation     |
| Scikit-learn      | ML modeling           |
| Flask             | Deployment            |
| Pickle            | Saving model & scaler |
| GitHub            | Version control       |
| VS Code           | Editor                |
| Postman / Browser | API testing           |

---

## 📁 Project Structure

```
California-House-Pricing/
│
├── model.pkl
├── scaler.pkl
├── app.py
├── requirements.txt
├── README.md
├── venv/
└── notebook.ipynb
```

---

## 📊 Dataset Features

The model predicts `Price` using the following features:

| Feature Name   | Description                 |
| -------------- | --------------------------- |
| **MedInc**     | Median income in the area   |
| **HouseAge**   | Age of the house            |
| **AveRooms**   | Avg number of rooms         |
| **AveBedrms**  | Avg number of bedrooms      |
| **Population** | Population of the area      |
| **AveOccup**   | Avg occupants per household |
| **Latitude**   | Geo Latitude                |
| **Longitude**  | Geo Longitude               |

---

## ▶️ Running the Project

### **1️⃣ Create Virtual Environment**

```
python -m venv venv
```

### **2️⃣ Activate Environment**

**Windows (PowerShell)**:

```
venv\Scripts\activate
```

**Git Bash / CMD:**

```
source venv/Scripts/activate
```

### **3️⃣ Install Requirements**

```
pip install -r requirements.txt
```

### **4️⃣ Run the Flask App**

```
python app.py
```

Server will run at:

```
http://127.0.0.1:5000
```

---

## 🌐 API Usage

### **POST /predict**

#### Request Body (JSON)

```json
{
  "MedInc": 8.3,
  "HouseAge": 25,
  "AveRooms": 6.5,
  "AveBedrms": 1.1,
  "Population": 450,
  "AveOccup": 3.2,
  "Latitude": 37.5,
  "Longitude": -122.3
}
```

#### Response (JSON)

```json
{
  "prediction": 245000
}
```

---

## 🧪 Model Evaluation (Example)

| Metric | Value  |
| ------ | ------ |
| MAE    | 34,500 |
| MSE    | 2.4M   |
| RMSE   | 1580   |

---



### Web App / Postman Testing

![Screenshot 2025-12-06 200103](https://github.com/user-attachments/assets/92a901d2-5511-4ba8-9e96-58200b2c0758)

![Screenshot 2025-12-06 211812](https://github.com/user-attachments/assets/bebedd2f-2f50-42ce-b6ea-e455bfeb542c)

---

## 📦 Deployment (Optional Sections)

If you deployed the model:

### Heroku Deployment

Include:

* Procfile
* runtime.txt
* steps to deploy

---

## 📝 Future Improvements

* Add multiple model options (Random Forest, XGBoost)
* Build a React-based frontend
* Add CI/CD pipeline
* Logging & monitoring

---

## 🧑‍💻 Author

**Bharat Shewale**
*Data Scientist | ML Engineer | AI Enthusiast*
📧 [bsshewale1630@gmail.com](mailto:bsshewale1630@gmail.com)

---


