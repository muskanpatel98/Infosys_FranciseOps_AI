# FranchiseOps AI – Milestone 2

## Overview

Milestone 2 extends the work completed in Milestone 1 by transforming the authentication portal into a complete AI-powered Franchise Management platform. While Milestone 1 focused on secure user authentication, registration, password recovery, JWT session management, and OTP-based verification, Milestone 2 introduces multiple Machine Learning agents, an AI Copilot powered by Qwen, enterprise analytics, advanced security mechanisms, and an administrator dashboard for centralized management.

The application is designed as a modular enterprise system where authentication, AI, analytics, machine learning, notifications, and administration work together to provide intelligent decision support for franchise operations.

---

# What Milestone 2 Adds

Compared to Milestone 1, this milestone introduces the following major enhancements:

* Multi-Agent AI architecture
* AI Copilot using Qwen-2.5-3B
* Machine Learning models for business intelligence
* Enterprise analytics dashboard
* Admin dashboard with complete user management
* Model retraining directly from the UI
* SQLite-based model metrics tracking
* Workforce attrition prediction
* Outlet clustering and revenue prediction
* Inventory demand forecasting
* Live notification center
* Chat history persistence
* Progressive account lockout
* Dynamic password strength validation
* Enterprise role-based authentication
* Improved modular code organization
* Automatic model loading and caching
* GPU acceleration support with graceful CPU fallback

---

# Features Built

## Authentication Module

* Secure Login
* User Registration
* Forgot Password
* Security Questions
* JWT Authentication
* Password Hashing using bcrypt
* Progressive Account Lockout
* Role-Based Access Control

---

## AI Copilot

* Powered by Qwen-2.5-3B
* Uses GPU whenever CUDA is available
* Gracefully falls back to CPU if GPU is unavailable
* Maintains chat history
* Generates AI recommendations
* Supports multi-agent reasoning

---

## Agent 1 – Workforce Intelligence

Predicts employee attrition risk using multiple machine learning algorithms.

Capabilities:

* Attrition probability prediction
* Confidence interval estimation
* Employee retention recommendations
* AI-generated retention strategies

Algorithms evaluated:

* Logistic Regression
* Random Forest
* Extra Trees
* Gradient Boosting
* AdaBoost
* Support Vector Machine
* K-Nearest Neighbors

---

## Agent 2 – Outlet Intelligence

Analyzes outlet performance and predicts business revenue.

Capabilities:

* Outlet clustering
* Revenue prediction
* Business tier classification
* KMeans clustering
* Revenue forecasting

Algorithms evaluated:

* Random Forest Regressor
* Gradient Boosting Regressor
* Extra Trees Regressor
* Decision Tree Regressor
* AdaBoost Regressor
* Ridge Regression
* K-Nearest Neighbors

---

## Agent 3 – Inventory Intelligence

Forecasts inventory demand and identifies stock risks.

Capabilities:

* Inventory demand prediction
* Stock planning
* Weather-aware forecasting
* Inventory analytics

Algorithms evaluated:

* Random Forest
* Gradient Boosting
* Extra Trees
* Decision Tree
* AdaBoost
* Ridge Regression
* K-Nearest Neighbors

---

## Admin Dashboard

Administrator capabilities include:

* Add users
* Delete users
* Unlock user accounts
* Monitor login status
* View ML model metrics
* View notification history
* Retrain all ML models
* System monitoring

---

## Notifications

Supports:

* Email alerts
* SMS simulation
* In-App notifications
* Notification history

---

# Technology Stack

## Frontend

* Streamlit
* HTML
* CSS

## Backend

* Python

## Database

* SQLite

## Machine Learning

* Scikit-learn
* NumPy
* Pandas
* Joblib

## AI

* Qwen-2.5-3B
* Hugging Face Transformers
* Accelerate
* BitsAndBytes

## Security

* JWT
* bcrypt

## Visualization

* Plotly

## Deployment

* Google Colab
* ngrok

---

# System Architecture Overview

| Phase                  | Description                                                            |
| ---------------------- | ---------------------------------------------------------------------- |
| User Authentication    | Login, Registration, Password Reset, JWT Authentication                |
| Security Layer         | Password Hashing, Progressive Lockout, Role-Based Access               |
| Database Layer         | SQLite stores users, notifications, ML metrics, chat history, datasets |
| Machine Learning Layer | Three independent ML agents perform prediction and forecasting         |
| AI Layer               | Qwen-2.5-3B generates intelligent business recommendations             |
| Analytics Layer        | KPI dashboard, model metrics, retraining, visualization                |
| Notification Layer     | Email, SMS simulation and In-App alerts                                |
| Admin Layer            | User management, system monitoring and model administration            |

---

# Indian Port Coverage

| Port          | Location    | Primary Cargo                                 |
| ------------- | ----------- | --------------------------------------------- |
| Mumbai (JNPT) | Maharashtra | Containers, Export & Import Cargo             |
| Mundra        | Gujarat     | Containers, Bulk Cargo, Logistics             |
| Chennai       | Tamil Nadu  | Automobiles, Containers, Industrial Cargo     |
| Cochin        | Kerala      | Containers, Petroleum Products, General Cargo |

---

# Google Colab Secrets Setup

Open the notebook.

Open the **Secrets** panel from the left sidebar.

Create the following secrets:

* NGROK_AUTHTOKEN
* HF_TOKEN
* KAGGLE_USERNAME
* KAGGLE_KEY
* EMAIL_ID
* EMAIL_PASSWORD
* JWT_SECRET_KEY
* ADMIN_EMAIL_ID
* ADMIN_PASSWORD

Enable notebook access for every secret.

Run the configuration cell to verify that all secrets are loaded successfully.

---

# Kaggle API Setup

1. Create a Kaggle account.
2. Open **Account** settings.
3. Select **Create New API Token**.
4. Download the `kaggle.json` file.
5. Copy the username and API key into the Colab Secrets as:

   * KAGGLE_USERNAME
   * KAGGLE_KEY
6. Run the notebook to download the required datasets automatically.
7. The datasets are cached locally so they are not downloaded repeatedly.

---

# Running the Notebook

1. Open the notebook in Google Colab.
2. Enable GPU runtime (Tesla T4 recommended).
3. Install all required dependencies.
4. Configure Colab Secrets.
5. Run all setup cells.
6. Initialize the SQLite database.
7. Train all machine learning models.
8. Launch the Streamlit application.
9. Open the generated ngrok HTTPS URL.
10. Log in using the administrator credentials.

---

# Conclusion

Milestone 2 transforms FranchiseOps AI from a secure authentication portal into a complete AI-powered franchise management platform. By combining machine learning, enterprise analytics, role-based security, intelligent AI assistance, and real-time monitoring, the application provides data-driven decision support for workforce management, outlet performance analysis, inventory forecasting, and administrative control within a single integrated system.
