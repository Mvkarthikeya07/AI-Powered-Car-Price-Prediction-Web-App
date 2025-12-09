🚗 AI-Powered Car Price Prediction Web App
Real-Time Machine Learning Based Used Car Valuation (Flask + ML)
📌 Overview

This is a complete end-to-end Machine Learning + Web Application project, developed during my InternPe Internship.

The app predicts the price of a used car based on:

Manufacturer

KMS Driven

Fuel Type

Car Age

It includes:

✔ A fully cleaned dataset
✔ ML training pipeline (train.py)
✔ Saved ML model (model/model.pkl)
✔ Flask backend (app.py)
✔ Responsive UI (HTML + Bootstrap)
✔ AJAX-based instant predictions

This project demonstrates real-world ML deployment skills with clean structure and maintainable code.

🚀 Key Features
🔍 Machine Learning

Processes and cleans noisy car dataset

Numerical & categorical feature engineering

Regression-based price prediction

Fallback median-based estimation (never breaks)

Extendable to RandomForest, XGBoost, etc.

🌐 Web Application

Flask backend with clear routing

Clean, responsive UI using HTML, CSS, Bootstrap

Supports both Form POST and AJAX JSON prediction

Results shown instantly without page reload

Stable and error-safe production-style design

🛠 Tech Stack
Layer	Technologies
Language	Python
Backend	Flask
Frontend	HTML, CSS, Bootstrap, JavaScript
Machine Learning	NumPy, Pandas, Scikit-Learn
Built Under	InternPe Internship

📂 Project Structure

CAR-PRICE-PREDICTION/
│
├── app.py                     # Flask backend
├── train.py                   # ML training script
├── requirements.txt           # Dependencies
│
├── data/
│   └── cars.csv               # Dataset
│
├── model/
│   └── model.pkl              # Saved ML model
│
├── static/
│   ├── css/
│   │   └── styles.css         # Custom styles
│   └── js/
│       └── app.js             # AJAX prediction script
│
└── templates/
    ├── index.html             # Main user interface
    └── result.html            # Prediction results page

⚙️ Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/your-username/car-price-prediction.git
cd car-price-prediction

2️⃣ Create Virtual Environment
python -m venv venv

3️⃣ Activate Environment (Windows PowerShell)
.\venv\Scripts\activate

4️⃣ Install Dependencies
pip install -r requirements.txt

5️⃣ Train Model (Optional, if model.pkl not present)
python train.py

6️⃣ Run the Flask App
python app.py

🔗 Open in Browser

👉 http://127.0.0.1:5000/

🎮 How the App Works

User enters:

Manufacturer

KMS Driven

Fuel Type

Car Age

Data is sent to Flask via:

Normal POST form submission, or

AJAX JSON request (no page reload)

Flask processes input → applies ML model

Prediction appears:

Instantly (AJAX), or

On a new page (Form)

🧠 Machine Learning Logic
🔧 Data Cleaning

Converts kilometer strings → numeric

Normalizes manufacturer names

Fixes inconsistent fuel labels

🔮 Prediction Workflow
predicted_price = median_price * age_factor * kms_factor


Fallback ensures the app never crashes, even with unseen data.

📸 Screenshots

Add your images under /screenshots or attach them in README:

<img width="1366" height="768" alt="Screenshot (16)" src="https://github.com/user-attachments/assets/4aa95bb4-80f0-49a5-bdf3-41ec4d5c62a9" />

<img width="1366" height="768" alt="Screenshot (18)" src="https://github.com/user-attachments/assets/fbbb1d7c-5620-4db6-a8ca-2670f50f2e4a" />

<img width="1366" height="768" alt="Screenshot (19)" src="https://github.com/user-attachments/assets/c49cc610-9e4e-4462-af64-5d657e69c51c" />

📚 What I Learned

Building ML pipelines

Cleaning real-world datasets

Flask backend development

AJAX for real-time interaction

Full-stack ML deployment workflow

Production-like project structuring

🏅 Internship

This project was created as part of my InternPe Internship, focusing on:

Applied Machine Learning

ML integration with web applications

Real-time prediction systems

Flask-based deployment

📬 Contact

👨‍💻 Developer: M V Karthikeya
📩 Email: mvkarthikeya2005@gmail.com

🔗 LinkedIn: https://www.linkedin.com/in/mv-karthikeya-b26a2131b

⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub!
