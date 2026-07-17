# 🧠 Human Stress Detection Based on Sleeping Habits

![Python](https://img.shields.io/badge/Python-3.10%2B-blue) ![Flask](https://img.shields.io/badge/Flask-2.3.2-00A6A6) ![scikit-learn](https://img.shields.io/badge/scikit-learn-1.2%2B-F7931E) ![Pandas](https://img.shields.io/badge/Pandas-2.0%2B-150458)

## 📌 Project Title
Human Stress Detection Based on Sleeping Habits Using Machine Learning Algorithms

## 🧾 Project Description
This project is a Flask-based web application that predicts human stress levels from sleep-related health parameters. The system uses a trained machine learning model to classify stress into five levels: Low/Normal, Medium Low, Medium, Medium High, and High.

The implementation includes a web interface for prediction, a CSV upload/preview workflow, model training in a Jupyter notebook, and a simple performance dashboard.

## ✨ Features
- Web-based stress prediction interface built with Flask
- Manual input form for eight physiological/sleep-related features
- CSV upload and preview page for dataset exploration
- Trained machine learning model loaded from a serialized file
- Performance analysis page with precision, recall, F1-score summary and confusion matrix display
- Chart page with a visualization dashboard
- Notebook-based training workflow for model development

## 🛠️ Tech Stack

| Category | Technology |
|---|---|
| Backend | Python, Flask |
| Machine Learning | scikit-learn, Random Forest Classifier |
| Data Handling | pandas, numpy |
| Visualization | matplotlib, seaborn, Google Charts |
| Frontend | HTML, Bootstrap-based templates |
| Model Serialization | pickle |

## 🏗️ Project Architecture / Folder Structure

```text
MPML12_CODE/
├── SOURCE CODE/
│   ├── app.py
│   ├── requirements.txt
│   ├── stress.pkl
│   ├── upload.csv
│   ├── Accuracy.txt
│   ├── model/
│   │   ├── stress.ipynb
│   │   ├── stress.pkl
│   │   └── DATASET/
│   │       └── SaYoPillow.csv
│   ├── static/
│   │   ├── assets/
│   │   │   ├── css/
│   │   │   ├── js/
│   │   │   └── img/
│   │   └── download.png
│   ├── templates/
│   │   ├── index.html
│   │   ├── login.html
│   │   ├── upload.html
│   │   ├── preview.html
│   │   ├── prediction.html
│   │   ├── performance.html
│   │   └── chart.html
│   └── test_data/
│       └── test.csv
```

## 🔄 Workflow
1. The training workflow is implemented in the notebook located in the model folder.
2. The notebook reads the dataset, performs exploratory analysis, trains a Random Forest Classifier, and saves the model as stress.pkl.
3. The Flask application loads the trained model and serves a web app.
4. Users can enter sleep-related measurements through the prediction form.
5. The application returns a stress label based on the trained model.
6. The performance page presents evaluation metrics and a confusion matrix visualization.

## 🤖 Machine Learning Model Details
- Model used: Random Forest Classifier
- Training notebook: model/stress.ipynb
- Serialized model file: stress.pkl
- Target classes:
  - 0 → Low/Normal
  - 1 → Medium Low
  - 2 → Medium
  - 3 → Medium High
  - 4 → High
- Reported accuracy from the repository file:
  - Training accuracy: 100%
  - Test accuracy: 97%

## 📊 Dataset Information
- Dataset file: model/DATASET/SaYoPillow.csv
- The dataset contains sleep and physiological indicators used for stress classification.
- Features used in the notebook include:
  - Snoring Range
  - Respiration Rate
  - Body Temperature
  - Limb Movement Rate
  - Blood Oxygen
  - Eye Movement
  - Number of Hours Sleep
  - Heart Rate
- Target column: Stress Level

## ⚙️ Installation & Setup
### Prerequisites
- Python 3.10.9 or compatible version

### Install dependencies
```bash
cd "MPML12_CODE/SOURCE CODE"
pip install -r requirements.txt
```

### Run the application
```bash
python app.py
```

The app starts locally and can be accessed through the Flask development server.

## ▶️ Usage
### 1. Home Page
Open the home page to access the application navigation.

### 2. Prediction
Use the prediction page to enter the required parameters and get a stress level prediction.

### 3. Upload / Preview
Use the upload page to submit a CSV file and preview the dataset contents.

### 4. Performance Analysis
Open the performance page to view evaluation metrics and the confusion matrix.

### 5. Charts
Use the chart page to explore the visualization dashboard.

## 📸 Screenshots (Placeholders)
- Home page screenshot: placeholder
- Prediction form screenshot: placeholder
- Performance analysis screenshot: placeholder
- Upload/preview workflow screenshot: placeholder

## 📈 Results / Output
The project produces the following outputs:
- Stress level prediction from user-entered values
- Parsed and previewed CSV data in the browser
- Performance metric summary for the trained classifier
- Confusion matrix visualization
- A simple chart view based on the dashboard page

## 🚀 Future Enhancements
Possible next steps for the project include:
- Adding user authentication and secure access
- Supporting batch prediction for multiple rows at once
- Connecting the app to a database for storing predictions
- Improving the chart page to display real model-based statistics
- Deploying the app to a cloud platform for public access
- Adding automated model retraining and evaluation pipelines

## ⚠️ Challenges Faced
- Bridging a notebook-based machine learning workflow with a Flask web application
- Mapping the trained model outputs to human-readable stress categories
- Integrating CSV upload and dataset preview into the web interface
- Presenting model evaluation results in an accessible UI format

## 🎓 Learning Outcomes
This project helped demonstrate:
- End-to-end development of a simple machine learning application
- Data preprocessing and model training in a notebook environment
- Model serialization and reuse in a deployment workflow
- Basic web application integration for ML inference
- Visualization of model performance for better interpretation

## 📄 License
No explicit license file was found in the repository. This project appears to be shared for educational and portfolio purposes.

## 👤 Author
Project prepared as part of a machine learning and web application development workflow.

> Update this section with your name, email, and GitHub profile if you want to use this README for a portfolio or public repository.
