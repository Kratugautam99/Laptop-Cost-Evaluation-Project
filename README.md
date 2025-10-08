# Laptop Cost Evaluation Project
---

<p align="center">
  <a href="https://github.com/Kratugautam99/Laptop-Cost-Evaluation-Project">
    <img src="https://raw.githubusercontent.com/Kratugautam99/Laptop-Cost-Evaluation-Project/main/static/icon/laptop_icon.png" alt="Laptop Icon" width="200" />
  </a>
</p>

![Flask](https://img.shields.io/badge/Flask-3.1.1-important?logo=flask)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.19.0-FF6F00?logo=tensorflow)
![Python](https://img.shields.io/badge/Python-3.10.11-blue?logo=python)
![Render](https://img.shields.io/badge/Deployed_on-Render-5a5a5a?logo=render)

**Live Demo** (Render Free Tier - Please be patient) → 🌐 [https://laptop-cost-evaluation-project.onrender.com/](https://laptop-cost-evaluation-project.onrender.com/)
Or Refer Installation Guide and Usage Instructions!!

A sophisticated, lightning-fast web application that leverages machine learning to accurately predict laptop market prices based on technical specifications. Perfect for buyers, sellers, and tech enthusiasts who need instant price evaluations!

---

## 📑 Table of Contents

- [✨ Features](#-features)
- [🎯 Quick Start](#-quick-start)
- [📸 Visual Showcase](#-visual-showcase)
- [🏗️ Project Architecture](#️-project-architecture)
- [⚙️ Installation Guide](#️-installation-guide)
- [🚀 Usage Instructions](#-usage-instructions)
- [📊 Data Science Insights](#-data-science-insights)
- [🔧 Technical Stack](#-technical-stack)
- [☁️ Deployment](#️-deployment)
- [🔮 Future Roadmap](#-future-roadmap)
- [🤝 Contributing & Acknowledgments](#-contributing--acknowledgments)

---

## ✨ Features

### 🎯 Core Functionality
- **Instant Price Prediction** - Get real-time market cost estimates in seconds
- **Comprehensive Spec Analysis** - 16+ technical parameters including brand, CPU, RAM, storage, GPU, and display
- **Dual Currency Support** - Seamless INR ↔ USD conversion with live rates
- **Smart Defaults** - Intelligent pre-filling of ratings and review metrics

### 🛠 Technical Excellence
- **Optimized Performance** - CPU-only TensorFlow model for fast, lightweight inference
- **Responsive Design** - Beautiful, mobile-friendly interface
- **Production Ready** - Zero-config deployment on Render and local environments
- **Modular Architecture** - Clean, maintainable codebase

---

## 🎯 Quick Start

**Just want to try it out?** Visit our live demo:  
👉 [https://laptop-cost-evaluation-project.onrender.com/](https://laptop-cost-evaluation-project.onrender.com/)

*Note: Render's free tier may take 30-60 seconds to spin up on first visit*

---

## 📸 Visual Showcase

### 🖥️ Main Interface
<div align="center">

| Clean Form Design | Multiple Options |
|:---:|:---:|
| <img src="https://raw.githubusercontent.com/Kratugautam99/Laptop-Cost-Evaluation-Project/refs/heads/main/static/demo/1.png" width="400" alt="Main Form"> | <img src="https://raw.githubusercontent.com/Kratugautam99/Laptop-Cost-Evaluation-Project/refs/heads/main/static/demo/2.png" width="400" alt="Prediction Results"> |

</div>

### 💰 Advanced Features
<div align="center">

| Real-time Results | Currency Conversion |
|:---:|:---:|
| <img src="https://raw.githubusercontent.com/Kratugautam99/Laptop-Cost-Evaluation-Project/refs/heads/main/static/demo/3.png" width="400" alt="Currency Switch"> | <img src="https://raw.githubusercontent.com/Kratugautam99/Laptop-Cost-Evaluation-Project/refs/heads/main/static/demo/4.png" width="400" alt="Various Options"> |

</div>

<p align="center">
<em>✨ Experience accurate cost evaluations, instant currency conversion, and comprehensive specification analysis!</em>
</p>

---

## 🏗️ Project Architecture

```
Laptop-Cost-Evaluation-Project/
├── 🐍 app.py                        # Flask application entry point
├── 📊 laptop_data.csv                # Original dataset (1,000+ entries)
├── 🔬 Laptop_Regression.ipynb        # Complete EDA & model training
├── 📋 requirements.txt               # Python dependencies
├── 🎯 enviroment.yml                 # Conda environment configuration
│
├── 🤖 model/                        # ML artifacts
│   ├── laptop_cost_model.h5          # Trained TensorFlow model
│   ├── meta.json                     # Model metadata & configuration
│   └── preprocessor.joblib           # Feature preprocessing pipeline
│
└── 🎨 static/                       # Frontend assets
    ├── css/style.css                 # Responsive styling
    ├── icon/laptop_icon.png          # Brand identity
    ├── img/bg.jpg                    # Background imagery
    ├── demo/                         # Screenshots & documentation
    └── js/predict.js                 # Client-side interactivity
```

---

## ⚙️ Installation Guide

### Prerequisites
- **Python 3.10.11** - [Download here](https://www.python.org/downloads/release/python-31011/)
- Add to PATH: `C:\Users\[username]\AppData\Local\Programs\Python\Python310\python.exe`

### Environment Setup

#### 🟦 PowerShell (Recommended) 
```powershell
# Create and activate virtual environment
py -3.10 -m venv laptop-env
.\laptop-env\Scripts\Activate.ps1
```

#### 🟠 Git Bash / WSL
```bash
python3.10 -m venv laptop-env
source laptop-env/bin/activate
```

#### ⚫ Command Prompt
```cmd
py -3.10 -m venv laptop-env
.\laptop-env\Scripts\activate.bat
```

#### 🚿 Through "environment.yml" and Conda [Above Steps are Not-Required]
```console
conda env create -f environment.yml
```
---

## 🚀 Usage Instructions

1. **Clone & Setup**
   ```bash
   git clone https://github.com/Kratugautam99/Laptop-Cost-Evaluation-Project.git
   cd Laptop-Cost-Evaluation-Project
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Launch Application**
   ```bash
   python app.py
   ```

4. **Access the App**
   - Open your browser
   - Navigate to: `http://localhost:5000`
   - Start predicting laptop prices! 🎉

---

## 📊 Data Science Insights

### Dataset Overview
- **1,000+ laptop entries** with comprehensive specifications
- **16+ features** including technical specs, brand, and market data
- **Price range**: Budget to premium gaming/workstation laptops

### Machine Learning Pipeline
1. **Exploratory Data Analysis** - Feature correlation, distribution analysis
2. **Feature Engineering** - Categorical encoding, normalization
3. **Model Training** - Neural network regression with TensorFlow
4. **Performance Evaluation** - RMSE, R² scores, cross-validation

### Model Performance
- **High Accuracy** - Competitive prediction performance
- **Fast Inference** - Optimized for real-time web usage
- **Robust Preprocessing** - Handles diverse input combinations

---

## 🔧 Technical Stack

### Backend
```python
Flask==3.1.1           # Web framework
TensorFlow-cpu==2.19.0 # ML inference
scikit-learn==1.7.0    # Preprocessing
pandas==2.3.0          # Data manipulation
numpy==2.1.3           # Numerical computing
joblib==1.5.1          # Model serialization
```

### Frontend
- **HTML5** - Semantic markup
- **CSS3** - Responsive design with Flexbox/Grid
- **JavaScript** - Dynamic currency conversion & form handling

### Development Tools
- **Jupyter Notebook** - Data analysis & model development
- **Render** - Cloud deployment platform

---

## ☁️ Deployment

### Render Configuration
- **Python Version**: 3.10.11
- **Environment Variables**: Automatic PORT binding
- **Build Command**: `pip install -r requirements.txt`
- **Start Command**: `python app.py`

### Key Deployment Features
- **Path Agnostic** - Uses `PROJECT_DIR` for relative paths
- **Static Asset Optimization** - Efficient serving via Flask
- **Production Ready** - Error handling and logging

---

## 🔮 Future Roadmap

### 🚀 Enhanced Features
- [ ] **TensorFlow Lite Integration** - Ultra-lightweight model inference
- [ ] **Live Currency API** - Real-time exchange rates
- [ ] **Comparison Engine** - Side-by-side laptop comparisons
- [ ] **Batch Prediction API** - REST endpoint for multiple evaluations

### 📈 Model Improvements
- [ ] **Ensemble Methods** - Combine multiple algorithms
- [ ] **Time Series Analysis** - Price trend predictions
- [ ] **Image Recognition** - Price estimation from laptop photos

### 🌐 Platform Expansion
- [ ] **Mobile App** - React Native/iOS/Android versions
- [ ] **Browser Extension** - Price checking while shopping
- [ ] **API Marketplace** - Commercial prediction service

---

## 🤝 Contributing & Acknowledgments

### 🎯 How to Contribute
We love contributions! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/AmazingFeature`)
3. **Commit** your changes (`git commit -m 'Add AmazingFeature'`)
4. **Push** to the branch (`git push origin feature/AmazingFeature`)
5. **Open** a Pull Request

### 🙏 Special Thanks
- **Dataset Provider**: [Kaggle Laptop Prices Dataset](https://www.kaggle.com/datasets/anubhavgoyal10/laptop-prices-dataset)
- **Hosting Platform**: [Render](https://render.com/) for free tier hosting
- **Development Environment**: [Google Colab](https://colab.research.google.com/) for interactive development

### 📜 License
This project is open source and available under the [MIT License](LICENSE).

---

<div align="center">

### ⭐ Love this project? Give it a star! ⭐

**Your support helps us improve and add more features!**

[![Star History Chart](https://api.star-history.com/svg?repos=Kratugautam99/Laptop-Cost-Evaluation-Project&type=Date)](https://star-history.com/#Kratugautam99/Laptop-Cost-Evaluation-Project&Date)

*Made with 🧠 => By Kratu Gautam!*

</div>
