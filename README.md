🚗 AI-Powered Car Price Prediction Web App
Real-Time Machine Learning-Based Used Car Valuation (Flask + ML)
<p align="center"> <img src="https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python"> <img src="https://img.shields.io/badge/Flask-Web%20Framework-black?style=for-the-badge&logo=flask"> <img src="https://img.shields.io/badge/ML-Scikit--Learn-orange?style=for-the-badge&logo=scikitlearn"> <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge"> </p>
📌 Overview

This project is a complete end-to-end Machine Learning + Web Application, developed during my InternPe Internship.

The system predicts the price of a used car based on:

Manufacturer

Kilometers Driven

Fuel Type

Age of the Car

It includes:

✔ Cleaned real-world dataset
✔ ML training pipeline (train.py)
✔ Saved ML model (model/model.pkl)
✔ Flask backend (app.py)
✔ Responsive UI with Bootstrap
✔ AJAX-based instant predictions (no page reload)

A production-ready deployment structure ensures modularity, clarity, and scalability.

🚀 Key Features
🔍 Machine Learning

Cleans and preprocesses noisy car dataset

Handles numerical + categorical features

Regression-based prediction

Median fallback for stable results

Fully extendable (RandomForest, XGBoost, etc.)

🌐 Web Application

Flask backend with organized routing

Modern UI (HTML + CSS + Bootstrap)

Supports:

Form POST prediction

AJAX JSON prediction

Page does not reload in AJAX mode

Error-safe design for stable user experience

🛠 Tech Stack
Layer	Technology
Language	Python
Backend	Flask
Frontend	HTML, CSS, Bootstrap, JavaScript
ML Libraries	NumPy, Pandas, Scikit-Learn
Environment	Virtualenv
Developed During	InternPe Internship
📂 Project Structure
CAR-PRICE-PREDICTION/
│── app.py                   # Flask backend
│── train.py                 # ML model training script
│── requirements.txt         # Dependencies
│
├── data/
│   └── cars.csv             # Dataset
│
├── model/
│   └── model.pkl            # Trained ML model
│
├── static/
│   ├── css/
│   │   └── styles.css       # Styling
│   └── js/
│       └── app.js           # AJAX logic
│
└── templates/
    ├── index.html           # Main UI
    └── result.html          # Result page

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

5️⃣ Train the Model (Optional)
python train.py

6️⃣ Run the Flask App
python app.py

7️⃣ Open in Browser

👉 http://127.0.0.1:5000/

🎮 How the App Works
🖊 User Inputs:

Manufacturer

KMS Driven

Fuel Type

Car Age

📡 Data Sent To Server Via:

Form POST

AJAX JSON (instant)

⚙ ML Logic Executes:

Cleans input

Applies regression model

Calculates final predicted price

📤 Output is Displayed:

Instantly with AJAX

On result page with form submission

🧠 Machine Learning Logic
🔧 Data Cleaning

Converts kilometer strings → clean numeric

Normalizes manufacturer names

Standardizes fuel labels

Removes outliers for stability

🔮 Prediction Formula (Fallback Mode)
predicted_price = median_price * age_factor * kms_factor


Ensures 100% uptime even with unseen inputs.

📸 Screenshots

<img width="1366" height="768" alt="Screenshot (16)" src="https://github.com/user-attachments/assets/fbfc4a87-7713-4caa-a8da-9cd54c172603" />

<img width="1366" height="768" alt="Screenshot (18)" src="https://github.com/user-attachments/assets/f9344be3-b20a-43fb-b661-52ed2a425799" />

<img width="1366" height="768" alt="Screenshot (19)" src="https://github.com/user-attachments/assets/4ee16a5f-b7c0-4776-b8cc-4fb4749f072e" />

📚 What I Learned

Building ML pipelines

Handling & cleaning real-world datasets

Building Flask backends

AJAX for real-time UX

Deploying ML models in web apps

Writing production-quality project structure

🏅 Internship

This project was created during my InternPe Internship, where I focused on:

Practical machine learning

Real-time prediction systems

End-to-end ML deployment

Flask development

📬 Contact

👨‍💻 Developer: M V Karthikeya
📩 Email: mvkarthikeya2005@gmail.com

🔗 LinkedIn: https://www.linkedin.com/in/mv-karthikeya-b26a2131b

🖼️ Image Comparison Web App

A Computer Vision–powered Flask web application that compares two images using SSIM, ORB Feature Matching, and K-Means Color Clustering to generate a detailed similarity analysis with visual outputs.

🚀 Overview

The Image Comparison Web App uses multiple classical Computer Vision algorithms to evaluate and visualize the similarity between two images. The application includes a modern UI and produces:

✔ SSIM structural similarity score

✔ ORB keypoint feature matching

✔ Dominant color extraction (K-Means)

✔ Common color comparison

✔ SSIM heatmap visualization

✔ ORB feature match image

🎯 Key Features 🔍 SSIM — Structural Similarity

Measures luminance, contrast & structure

Outputs a similarity score (0–1)

Generates a similarity heatmap

🧠 ORB — Feature Matching

Detects keypoints (corners, edges)

Computes descriptors

Generates a feature-match visualization

Computes a normalized match score

🎨 K-Means Color Clustering

Extracts top dominant colors

Compares theme similarity

Finds common colors

🌐 Full Web UI

Clean Bootstrap interface

Live image preview

Instant results dashboard

🧠 Tech Stack

Frontend: HTML, CSS (Bootstrap), JavaScript Backend: Python, Flask Computer Vision: OpenCV, scikit-image, scikit-learn, NumPy

📁 Project Structure Image-Comparison-WebApp/ │ ├── app.py ├── requirements.txt │ ├── utils/ │ ├── init.py │ ├── image_utils.py # SSIM + ORB + preprocessing │ └── color_utils.py # K-Means clustering │ ├── templates/ │ ├── index.html # Upload page │ └── result.html # Results dashboard │ └── static/ ├── css/ ├── js/ └── outputs/ # Auto-generated results

⚙️ How It Works

User uploads Image A and Image B

Flask backend saves inputs

App performs:

SSIM structural similarity

ORB keypoint detection & matching

K-Means dominant color extraction

App generates visuals:

SSIM heatmap

ORB match image

Results are displayed in a clean dashboard

▶️ Run Locally 1️⃣ Install Requirements pip install -r requirements.txt

2️⃣ Run the App python app.py

3️⃣ Open Browser http://127.0.0.1:5000/

📸 Sample Outputs

🖥️ Home Page (Upload Screen) Screenshot (22)

🖼️ Images Selected Screenshot (23)

📊 Comparison Results Screenshot (24)

🔍 SSIM Difference Visualization Screenshot (25)

🧠 ORB Feature Matching Screenshot (26)

🧩 Algorithms Used 🔸 SSIM — Structural Similarity

Analyzes: luminance, contrast, structure.

🔸 ORB — (Oriented FAST + Rotated BRIEF)

Keypoint detection

Descriptor extraction

Feature matching

🔸 K-Means Clustering

Groups color pixels

Extracts dominant colors

Compares color similarity

🚀 Future Enhancements

Add CLIP / ResNet deep-learning similarity

Drag-and-drop image upload

Background removal + object-based matching

Deploy on Render/Heroku

🤝 Contributing

Pull requests are welcome! Fork → Improve → Submit PR

📬 Contact

Developer: M V Karthikeya Connect on LinkedIn anytime.

📜 License

This project is licensed under the MIT License.

⭐ Support

If you like this project, please give it a ⭐ on GitHub!
