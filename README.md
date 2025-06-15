# Data Science Portfolio by Sumit Watkar

## [Project 1: Hotel Reservation Prediction](https://github.com/mltweakster/Hotel-Reservation-Prediction)

### **Overview:**

The **Hotel Reservation Prediction** project is a machine learning system that forecasts whether a hotel booking will be canceled. It enables better inventory planning, reduces revenue leakage, and supports intelligent overbooking strategies.

> 🔗 **[Live App URL](https://hrp-552900362680.us-central1.run.app/)**

### **Technologies and Tools Used:**

| Category             | Tools/Tech                                        |
|----------------------|---------------------------------------------------|
| ML & Processing      | Python, Pandas, Scikit-learn                      |
| Modeling             | Random Forest, Light Gradient Boosting Machine    |
| Experiment Tracking  | MLflow                                            |
| API & Serving        | Flask                                             |
| CI/CD                | Jenkins, GitHub                                   |
| Containerization     | Docker                                            |
| Deployment           | Google Container Registry, Google Cloud Run       |

### **MLflow Experiment Run:**

The model was trained and tracked using **MLflow** with the following metrics and hyperparameters:

![MLflow Experiment Run](https://github.com/mltweakster/Hotel-Reservation-Prediction/blob/main/research/mlflow-exp.png)

### **Jenkins CI/CD Pipeline:**

This project is integrated with a **CI/CD pipeline** using Jenkins:

### **Pipeline Stages**:

> 1. Clone GitHub Repository  
> 2. Set up Python Virtual Environment  
> 3. Install Dependencies  
> 4. Build and Push Docker Image  
> 5. Deploy to Google Cloud Run

![Jenkins Pipeline](https://github.com/mltweakster/Hotel-Reservation-Prediction/blob/main/research/jenkins-cicd.png)

### **Outcomes**

- **Accurate Cancellation Prediction**
- **Fully Automated CI/CD Pipeline**
- **Cloud-native, Serverless Deployment**
- **Portable, Dockerized App**
- **Reproducible Experiments via MLflow**

> ![Flask App Prediction](https://github.com/mltweakster/Hotel-Reservation-Prediction/blob/main/research/flask-app.png)

---


## [Project 2: Delivery Time Prediction](https://github.com/mltweakster/Delivery-Time-Prediction)

### **Overview:**  

- The Delivery Time Prediction project is a machine learning-based application designed to estimate delivery times for orders based on various factors such as distance, traffic conditions, weather, and historical data. This project helps logistics companies, e-commerce platforms, and food delivery services improve their estimated delivery times, optimize routes, and enhance customer satisfaction. 

- The application includes a FastAPI-based inference endpoint and additional APIs for analytics and insights. The development process integrates experiment tracking and pipeline reproducibility using MLFlow and DVC.  

### **Methodologies:**  

**1. Feature Engineering & Optimization:** Implemented feature engineering techniques such as distance calculations, weather impact factors, and traffic analysis to improve prediction accuracy. 

**2. Predictive Model Development:** Built a **StackingRegressor** to predict delivery times, combining **LightGBM** and **Random Forest** as base learners with **Linear Regression** as the meta-learner.

**3. Experiment Tracking:** Optimized model performance through rigorous experimentation, integrated MLFlow for model performance tracking, hyperparameter tuning, and logging experiments to ensure structured model development.  

**4. Pipeline Reproducibility:** Utilized DVC (Data Version Control) to manage datasets, version ML pipelines, and ensure reproducibility in model training and evaluation. 

**5. API Development:** Developed a FastAPI-based inference endpoint for real-time delivery time predictions and additional API endpoints to provide insights into delivery trends and performance. 

### **Technologies and Tools Used:**

* **Machine Learning & Data Processing:** NumPy, Pandas, Scikit-learn, LightGBM, Random Forest, Linear Regression
* **Experiment Tracking:** MLFlow
* **Pipeline Reproducibility:** DVC
* **API Framework:** FastAPI
* **Containerization**: Docker
* **Version Control & Deployment:** Git, GitHub, Github Actions, Amazon EC2, Amazon ECR

### **Outcomes:** 

**1. Accurate Delivery Time Estimation:** A machine learning model capable of predicting delivery times with high accuracy.  

**2. Real-time Predictions:** FastAPI-based inference endpoint enables quick delivery time estimations for end-users and businesses.  

**3. Data-Driven Insights:** Additional API endpoints provide insights into delivery trends, helping businesses optimize logistics and reduce delays.  

**4. Reproducibility and Experimentation:** MLFlow and DVC streamline experiment tracking, pipeline reproduction, and model versioning.  

**5. Enhanced Operational Efficiency:** Businesses can improve logistics, optimize delivery routes, and enhance customer satisfaction with more accurate time predictions.  

![pipeline](https://github.com/user-attachments/assets/f3391736-e0a8-45cc-806c-2d87f3e21af3)

---


## [Project 3: Sentiment Analysis](https://github.com/mltweakster/Sentiment-Analysis)

### **Overview:**
- The Sentiment Analysis project is an end-to-end machine learning application designed to classify the sentiment of YouTube video comments. By leveraging machine learning techniques, the project enables real-time sentiment prediction and provides insightful analytics on comment trends. 

- The application includes a Flask-based inference endpoint and additional APIs for sentiment analysis insights. The development process integrates robust experimentation, tracking, and pipeline reproducibility using MLFlow and DVC, ensuring a streamlined and reproducible workflow.  

### **Methodologies:**

**1. Sentiment Analysis Development:** Built a machine learning model to classify YouTube comments using text vectorization (TfidfVectorizer) and experimented with multiple models, selecting **LightGBMClassifier** for optimal performance.

**2. Experiment Tracking:** Integrated MLFlow to track model performance, hyperparameter tuning, and experiment logging for a structured development process.

**3. Pipeline Reproducibility:** Implemented DVC (Data Version Control) to manage datasets, ensure reproducibility, and maintain version control of ML pipelines.

**4. API Development:** Developed a Flask-based inference endpoint for real-time sentiment prediction and additional API endpoints to provide analytics on comment sentiments.

### **Technologies and Tools Used:** 

* **Machine Learning & NLP:** Numpy, Pandas, scikit-learn, LightGBMClassifier, TfidfVectorizer
* **Experiment Tracking:** MLFlow
* **Pipeline Reproducibility:** DVC
* **API Framework:** Flask
* **Containerization**: Docker
* **Version Control & Deployment:** Git, GitHub, Github Actions, Amazon EC2, Amazon ECR

### **Outcomes:**

**1. Robust Sentiment Prediction:** A well-optimized machine learning model capable of classifying YouTube comment sentiments accurately.  

**2. Scalable API Solution:** Flask-based inference endpoint ensures real-time sentiment classification with low latency.  

**3. Data-Driven Insights:** Additional API endpoints provide analytics and trends on comment sentiments, aiding content creators and researchers.  

**4. Reproducibility and Experimentation:** MLFlow and DVC streamline experiment tracking and pipeline reproduction, enhancing model versioning and reproducibility.  

**5. Efficient Development Lifecycle:** The integration of MLFlow and DVC reduces errors, enhances model tracking, and ensures structured development.  

---


## [Project 4: Text to Speech Generation using CICD](https://github.com/sumitwatkar/Text-to-Speech-Generation-using-CICD)

### Overview:

- The Text-to-Speech (TTS) project is a Python-based application that converts written text into clear and natural speech output. Supporting multiple languages, the application leverages the Google Text-to-Speech (GTTS) library to synthesize speech from text, making it suitable for a variety of use cases including assisting visually impaired users, language learners, and individuals who prefer to consume textual content in an auditory format.

- The project adopts continuous integration and continuous deployment (CICD) practices to streamline the development and deployment process, allowing for efficient testing and deployment of the application.

### Methodologies:

**1. Application Development**: Built the TTS application using Python and the GTTS library, optimizing the synthesis process for high-quality speech generation and implementing error handling for smooth user interactions.

**2. CICD Pipeline**: Integrated GitHub Actions for automated testing and deployment, including code linting, unit tests, and automated builds.

**3. Containerization**: Created Dockerfiles to containerize the application, ensuring consistent and efficient deployments.

**4. Infrastructure Management**: Managed deployment and infrastructure using AWS services, deploying Docker images to Amazon Elastic Container Registry (ECR) for seamless integration and hosting the application on AWS Amazon instances for scalability and flexibility.

### Technologies and Tools Used:

* **Libraries**: GTTS, numpy, pandas
* **Web Framework**: Flask
* **Version Control & CICD**: GitHub Actions
* **Containerization**: Docker
* **Deployment & Infrastructure**: Amazon EC2, Amazon ECR

### Outcomes:

**1. Streamlined Development**: The CICD pipeline automates code linting, testing, building, and deployment, offering a smooth development lifecycle.

**2. Efficient Deployment**: Automated deployment of the TTS application to Amazon EC2 instances ensures fast, consistent, and reliable deployments.

**3. Containerization**: Docker containers ensure consistent application behavior across different environments and easy deployment.

**4. Scalability**: Leverages AWS services for scalability and to handle real-time synthesis challenges.

**5. Enhanced Productivity**: CICD practices improve efficiency, reduce manual errors, and accelerate deployment cycles.

---


## [Project 5: Flight Price Prediction using Amazon SageMaker](https://github.com/sumitwatkar/Flight-Price-Prediction-using-Amazon-SageMaker)


### Overview:

- The project aims to develop and deploy machine learning models for predicting flight ticket prices using Amazon SageMaker. This involves building a robust model that can accurately forecast the cost of a flight based on the various input features. The project also leverages the power of Amazon SageMaker for efficient training, optimization of the machine learning models.

### Methodologies:

**1. Data Collection and Preprocessing**: Acquired and preprocessed extensive datasets containing historical flight information, such as prices, routes, departure and arrival times, and airlines.

**2. Exploratory Data Analysis (EDA)**: Conducted thorough EDA using pandas and numpy to uncover patterns, trends, and potential features for model development.

**3. Model Development and Fine-Tuning**: Created and optimized machine learning models, with a focus on the high-performance XGBoost algorithm for its efficiency and interpretability.

**4. Feature Engineering and Selection**: Engineered and selected impactful features from the dataset using `feature-engine` to enhance model accuracy and performance.

**5. Model Evaluation**: Assessed model performance using metrics such as mean absolute error (MAE), mean squared error (MSE), and R-squared to ensure reliability and precision.

**6. Model Deployment**: Deployed the prediction model using Streamlit, offering a user-friendly web interface where users could input flight details and receive price predictions.

### Technologies and Tools Used:

* **Libraries**: numpy, pandas, matplotlob, seaborn, scipy, feature-engine, scikit-learn
* **Machine Learning Algorithm**: Isolation Forest, Extreme Gradient Boosting (XG Boost)
* **Web Framework**: Streamlit
* **Deployment & Infrastructure**: Streamlit Cloud

### Outcomes:

**1. Accurate Price Predictions**: Developed a reliable machine learning model that predicts flight ticket prices accurately based on historical data and selected features.

**2. User-Friendly Interface**: Created a streamlined web interface using Streamlit, enabling users to input flight details and swiftly receive price predictions.

**3. Improved Model Performance**: Enhanced model accuracy through fine-tuning, feature engineering, and iterative development, leading to dependable and precise predictions.

**4. Insights into Flight Pricing**: Provided valuable insights into the factors affecting flight prices, facilitating better decision-making for travelers and airline companies.

*[Web App Link](https://flight-price-prediction-using-amazon-sagemaker.streamlit.app/)*

---


## [Project 6: ATS Resume Checker using Google Gemini](https://github.com/sumitwatkar/ATS-Resume-Checker-using-Google-Gemini)

### Overview:

- The ATS Resume Checker is a application that leverages Google's Generative AI model, Gemini-Pro, to evaluate resumes based on a given job description. The application aims to help job seekers improve their resumes by providing a percentage match and identifying missing keywords relative to the job description. By acting as a skilled and experienced ATS (Application Tracking System), the application offers insights into how well a resume aligns with the job requirements, allowing users to optimize their resumes for better chances in a competitive job market.

### Tools and Technologies Used:

* **Libraries**: python-dotenv, PyPDF2
* **Generative AI Model**: Google Gemini Pro
* **Web Framework**: Streamlit
* **Deployment**: Streamlit Cloud

### Outcomes:

**1. AI-Powered Evaluation**: The application leverages Google's Gemini model to analyze the resume in relation to the job description.

**2. Matching Percentage and Feedback**: The application provides a matching percentage that indicates the compatibility of the resume with the job description and a list of missing keywords from the resume.

*[Web App Link](https://gemini-ats-resume-checker.streamlit.app/)*

---
