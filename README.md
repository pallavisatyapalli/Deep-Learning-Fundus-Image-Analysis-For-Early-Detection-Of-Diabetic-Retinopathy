
# Deep Learning Fundus Image Analysis for Early Detection of Diabetic Retinopathy

## Project Overview

**Deep Learning Fundus Image Analysis for Early Detection of Diabetic Retinopathy** is a medical imaging project that leverages deep learning techniques to automatically detect diabetic retinopathy (DR) from retinal fundus images.

Diabetic Retinopathy is one of the leading causes of blindness among diabetic patients. Early detection plays a crucial role in preventing severe vision loss. This system uses a pre-trained **Xception Convolutional Neural Network (CNN)** model to classify retinal abnormalities efficiently and accurately.

---

## Project Objectives

By completing this project, you will:

* Understand the fundamentals of Transfer Learning using Xception.
* Gain knowledge about medical image datasets.
* Learn image pre-processing and augmentation techniques.
* Build and train a deep learning classification model.
* Develop a web application using Flask.
* Integrate a trained model with a frontend UI.
* Store user data securely using IBM Cloudant DB.

---

## Real-World Applications

### 1️⃣ Early Disease Detection

Healthcare professionals can use this system to detect diabetic retinopathy in its early stages, enabling timely medical intervention.

### 2️⃣ Screening Programs

Public health organizations can implement large-scale DR screening programs using this automated solution.

### 3️⃣ Telemedicine & Remote Monitoring

Patients can upload fundus images remotely, and doctors can assess disease progression without in-person visits.

---

## 🏗 Technical Architecture

The system consists of:

* Deep Learning Model (Xception CNN)
* Image Pre-processing Pipeline
* Flask Web Application
* IBM Cloudant Database
* HTML/CSS Frontend
* Google Colab for Model Training

---

## Pre-Requisites

### Required Software & Tools

* Python 3.x
* Anaconda
* Google Colab
* IBM Cloud Account
* Kaggle Account
* Flask
* TensorFlow / Keras
* NumPy
* Matplotlib
* Cloudant Library

### Prior Knowledge Required

* Python Programming
* Deep Learning Basics
* Convolutional Neural Networks (CNN)
* Transfer Learning
* Flask Web Framework
* Basic HTML & CSS

---

## Project Structure

```
Deep-Learning-DR-Detection/
│
├── static/
│   ├── css/
│   ├── images/
│   └── uploads/
│
├── templates/
│   ├── index.html
│   ├── register.html
│   ├── login.html
│   ├── prediction.html
│   └── logout.html
│
├── model/
│   └── Updated-Xception-diabetic-retinopathy.h5
│
├── app.py
└── README.md
```

---

# Project Workflow

---

## 🟢 Milestone 1: Data Collection

* Dataset downloaded from Kaggle.
* Dataset cloned directly into Google Colab.
* Dataset extracted and prepared for training.

---

## 🟢 Milestone 2: Data Pre-Processing

* Imported necessary libraries.
* Configured `ImageDataGenerator`.
* Applied augmentation techniques:

  * Rotation
  * Scaling
  * Translation
  * Flipping
  * Normalization

---

## 🟢 Milestone 3: Model Building

We used the **Xception** pre-trained CNN model as a feature extractor.

### Steps:

1. Load Pre-trained Xception model
2. Add custom Dense layers
3. Configure optimizer & loss function
4. Train the model
5. Evaluate performance

---

## 🟢 Milestone 4: Save Model & Cloudant DB Setup

### Model Saving

The trained model is saved as:

```
Updated-Xception-diabetic-retinopathy.h5
```

### IBM Cloudant Database Setup

* Created Cloudant service in IBM Cloud
* Generated service credentials
* Connected Flask app with Cloudant
* Created database for user authentication

---

## 🟢 Milestone 5: Web Application Development

### 🔹 Frontend (HTML Pages)

* index.html
* register.html
* login.html
* prediction.html
* logout.html

### 🔹 Backend (Flask - app.py)

Features implemented:

* User Registration
* User Login Authentication
* Image Upload
* Model Prediction
* Result Display on UI
* Logout Functionality

---

## 🧠 Prediction Process

1. Image uploaded by user
2. Image loaded using `load_img()`
3. Converted to array using `img_to_array()`
4. Resized to Xception input size
5. Preprocessed for Xception
6. Model predicts class probabilities
7. Highest probability selected using `np.argmax()`
8. Result displayed on UI

---

## ▶️ How to Run the Application

### Step 1: Open Anaconda Prompt

Navigate to project folder:

```
cd project-folder-name
```

### Step 2: Run Flask App

```
python app.py
```

### Step 3: Open Browser

Go to:

```
http://localhost:5000
```

### Step 4:

* Register
* Login
* Upload retinal image
* View prediction results

---

## 📊 Output

* User Authentication System
* Retinal Image Classification
* Disease Prediction Displayed on UI
* Cloud Database Integration

---

## 🛠 Technologies Used

* Python
* TensorFlow / Keras
* Xception Model
* Flask
* HTML / CSS
* IBM Cloudant DB
* Google Colab

---

## 🔐 Database Integration

IBM Cloud Identity & Access Management is used to securely authenticate users and manage database access.

---

## 🌟 Future Enhancements

* Add multi-class DR grading
* Improve UI design
* Deploy on cloud server
* Add doctor dashboard
* Generate PDF medical reports

---

## 📌 Conclusion

This project demonstrates how deep learning and web technologies can be integrated to build a real-world healthcare solution for early detection of diabetic retinopathy. It enables automated screening, remote monitoring, and scalable deployment for medical applications.


