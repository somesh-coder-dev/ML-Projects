
# 🌾 Crop Recommendation System using ML


This project predicts the most suitable crop based on soil nutrients and climatic conditions using a Random Forest ML model, and  helps farmers make informed decisions to maximize their yield and profitability.





## ✨Features

- **User-Friendly Interface:** A simple web form to input soil and environmental data.

- **Instant Predictions:** Get an immediate crop recommendation based on the input values.

- **Data-Driven:** Built on a dataset of agricultural data to ensure accurate recommendations.

- **Scalable:** The Flask backend is lightweight and easy to deploy.

## ⚙️ How It Works

The application follows a simple workflow:

1. **User Input:** The user enters values for Nitrogen, Phosphorous, Potassium, Temperature, Humidity, pH, and Rainfall on the web interface.

2. **Data Processing:** The Flask backend receives this data.

3. **Model Prediction:** The pre-trained machine learning model (model.pkl) is loaded and used to predict the most suitable crop based on the input features.

4. **Display Result:** The recommended crop name is rendered on the results page and displayed to the user.
## 🧠 Model & Dataset

**The Model:**

- The prediction model is a **Random Forest Classifier** from the **scikit-learn** library. This ensemble model was chosen for its high accuracy and robustness in handling various types of input data. The complete model training and evaluation process can be found in the **Crop_RecommendationV2.ipynb** Jupyter Notebook.

**The Dataset:**

- The model was trained on the **Crop_RecommendationV2.csv** dataset, which contains 2200 data points. The features used for training include:

  - **N:** Ratio of Nitrogen content in soil

  - **P:** Ratio of Phosphorous content in soil

  - **K:** Ratio of Potassium content in soil

  - **temperature:** Temperature in degrees Celsius

  - **humidity:** Relative humidity in %

  - **ph:** pH value of the soil

  - **rainfall:** Rainfall in mm

The dataset covers 22 different crops, which serve as the target labels for the classification model.


## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

---

### ✅ Prerequisites

You need to have **Python (version 3.8 or newer)** and **pip** installed on your system.

---

### 📦 Installation

**Clone the repository:**

```bash
git clone https://github.com/somesh-coder-dev/ML-Projects.git
cd ML-Projects/Crop\ Prediction
```

**Create and activate a virtual environment:**

🪟 **Windows:**

```bash
python -m venv venv
.\venv\Scripts\activate
```

🐧 **macOS / Linux:**

```bash
python3 -m venv venv
source venv/bin/activate
```

**Install the required dependencies:**

```bash
pip install -r requirements.txt
```

---

### 🏃‍♂️ Running the Application

Once the installation is complete, run the Flask app:

```bash
python app.py
```

Now, open your web browser and navigate to:

```
http://127.0.0.1:5000
```

---

## 📁 Project Structure

Here is an overview of the key files in this project:

```
├── static/                     # Static files (CSS, images)
├── templates/                  # HTML templates
├── Crop_RecommendationV2.ipynb # Jupyter Notebook for model dev
├── Crop_RecommendationV2.csv   # Dataset used for training
├── Procfile                    # Heroku deployment file
├── app.py                      # Main Flask application
├── model.pkl                   # Trained ML model
├── model.py                    # Model training (optional)
└── requirements.txt            # Python dependencies
```

---

## 🗺️ Roadmap

Here are some ideas for future improvements:

- [ ] **Add More Models** – Try XGBoost, SVM, etc.
- [ ] **API Endpoints** – Create REST API for integration
- [ ] **Data Visualization** – Show charts/graphs for predictions
- [ ] **Batch Predictions** – Allow CSV upload for bulk prediction

---

## 🤝 Contributing

Contributions are what make the open-source community amazing. Any help is appreciated!

1. Fork the Project  
2. Create your Feature Branch  
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. Commit your Changes  
   ```bash
   git commit -m "Add some AmazingFeature"
   ```
4. Push to the Branch  
   ```bash
   git push origin feature/AmazingFeature
   ```
5. Open a Pull Request

---

## 👤 Author

**Somesh Mishra**  
GitHub: [@somesh-coder-dev](https://github.com/somesh-coder-dev)

Feel free to reach out with any questions or feedback!
