# REPS-Pro: Enterprise-Grade Real Estate Predictive System
![visitors](https://visitor-badge.laobi.icu/badge?page_id=page.id)

[![Ashutosh's github activity graph](https://github-readme-activity-graph.vercel.app/graph?username=HamzaAlawneh&theme=react-dark)](https://github.com/ashutosh00710/github-readme-activity-graph)



**Strategic AI Engineering Project | Developed @ MODEE**

##  Executive Overview
REPS-Pro (Real Estate Predictive System) is a production-ready machine learning framework designed to solve the problem of market valuation volatility. Unlike standard regression models, REPS-Pro incorporates a **Data Integrity Pipeline** to eliminate artificial biases, ensuring that predictions reflect true economic drivers rather than dataset artifacts.

---

##  Engineering Stack (The "Why" Behind the Tech)
| Component | Technology | Rationale |
| :--- | :--- | :--- |
| **Model Engine** | `RandomForestRegressor` | Handles non-linear relationships and high-dimensional data better than linear models. |
| **Validation** | `Shuffled K-Fold CV` | Ensures model stability and prevents data leakage or overfitting to specific clusters. |
| **Backend** | `Flask (REST API)` | Lightweight and scalable for microservices architecture. |
| **Tunnelling** | `Pyngrok / Linux-Managed` | Provides secure, temporary public access for UAT (User Acceptance Testing). |
| **Frontend** | `Corporate UI / CSS3` | Aligned with MODEE branding to bridge the gap between technical output and user experience. |

---

##  Deep Dive: The "Refinement Stage" (Amazon-Style Case Study)
### The Problem: The $500k Price Ceiling
During the EDA (Exploratory Data Analysis) phase, I identified a significant "Artificial Artifact": a price cap at $500,000 which skewed the model's perception of high-end real estate.

### The Solution: Strategic Data Filtering
I implemented a **Refinement Stage** to filter out capped values. This decision reflects a "Customer Obsession" for accuracy over "Vanity Metrics" (high scores on biased data).

**Comparison of Engineering Outcomes:**

| Metric | Baseline Model (Raw Data) | REPS-Pro (Refined Data) | Improvement Impact |
| :--- | :--- | :--- | :--- |
| **Model R² Score** | 85.0% | **81.89%** | Reduced Overfitting |
| **Bias Analysis** | High Bias at $500k | **Unbiased Prediction** | Accurate High-Value Estimates |
| **Architecture** | Monolithic Notebook | **Modular (Decoupled)** | Ready for CI/CD |
| **Data Integrity** | Contaminated with Artifacts | **Clinically Clean** | High Trust for Financial Use |

---

##  Technical System Design
The system is built on **Modular Programming** principles, separating concerns to allow for independent scaling:

1. **Preprocessing Module (`preprocess.py`):** Automates Feature Scaling and handling of missing values (imputation).
2. **Inference Module (`predict.py`):** Loads the serialized model (`.pkl`) and performs real-time computation.
3. **API Layer (`app.py`):** Manages HTTP requests/responses and error handling for invalid user inputs.

### Scenario Testing (Intuition Check)
To ensure the model "thinks" logically, I implemented scenario-based testing:
* **Elite Scenario:** High Income ($85k+) → Predicted: **$321,833**
* **Standard Scenario:** Low Income ($15k) → Predicted: **$165,956**
* **Time-Value Test:** New Build vs. Old Build → Correctly identifies the **Age-Premium**.

---

##  Future Roadmap (Scale & Innovation)
Consistent with Amazon's "Day 1" philosophy, REPS-Pro is built for continuous evolution:

* **[ ] Geospatial Intelligence:** Integrating `Leaflet.js` to enable interactive map-based coordinate selection, moving beyond manual input.
* **[ ] Containerization:** Deploying via **Docker** to ensure environment parity across AWS/Azure cloud environments.
* **[ ] Time-Series Integration:** Leveraging economic indicators (inflation, interest rates) to predict future price trends (2026-2030).
* **[ ] Model Quantization:** Optimizing inference speed for high-traffic public API gateways.

---

##  Author Information
* **Name:** Hamza Medhat Alawneh
* **Role:** AI Engineering Intern @ Ministry of Digital Economy and Entrepreneurship (MODEE)
* **Focus:** Advanced AI Architectures | Data Science | System Design
* **Contact:** https://www.linkedin.com/in/hamza-medhat-alawneh-ab622a247/
---
> *“In God we trust, all others must bring data.” – This project is a testament to data-driven decision-making in the public sector.*
