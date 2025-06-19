
# 🧠 Medical Diagnosis & Reporting App

A full-stack medical web application for **diabetes prediction** using machine learning. Built with **Streamlit**, this app empowers doctors to quickly upload patient data, generate live predictions, create PDF reports, and email results—automating a complete diagnosis workflow.

---

## 🚀 Features

- 🔐 **Secure role-based login** (Doctor/Patient) using `streamlit_authenticator`
- 📊 **CSV upload and real-time data preview** with bar, pie, and scatter plots
- 🤖 **ML prediction** using Random Forest (via `scikit-learn`)
- 📄 **Dynamic PDF generation** via `FPDF`, with input summary and results
- 📧 **Email reports** to patients using Gmail API + OAuth 2.0
- 🗃️ **SQLite storage** for timestamped history, with date-range filtering
- 🗺️ **Geospatial data visualization** using Pydeck (map of cases across India)

---

## 🏥 Use Case

This application is designed to assist healthcare professionals in:
- Rapidly predicting diabetes from patient input
- Managing patient records and history
- Automatically generating and emailing PDF reports
- Visualizing disease trends geographically

It enhances **efficiency, accuracy, and communication** in a real-world clinical setting.

---

## 🛠️ Tech Stack

| Category              | Tools Used                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| Frontend Framework    | Streamlit                                                                  |
| Programming Language  | Python                                                                     |
| Machine Learning      | scikit-learn, Pandas, NumPy                                                 |
| Visualization         | Matplotlib, Pydeck                                                          |
| Authentication        | streamlit-authenticator                                                    |
| Reporting             | FPDF (PDF generation)                                                      |
| Email Integration     | Gmail API, OAuth 2.0                                                       |
| Database              | SQLite                                                                     |
| Dev Tools             | Git, VS Code, GitHub                                                       |

---

## 📷 Screenshots



| Dashboard | Prediction Report | Geospatial Map |
|----------|-------------------|----------------|
| ![](screenshots/dashboard.png) | ![](screenshots/pdf_report.png) | ![](screenshots/geo_map.png) |

---

### ✅ Requirements



- ✅ Python 3.8 or higher
- ✅ pip (Python package installer)
- ✅ Git (for version control)
- ✅ Virtual environment manager (optional but recommended)
- ✅ Gmail API credentials file (`credentials.json`) for OAuth 2.0
- ✅ Internet connection (for accessing Gmail API and downloading dependencies)

### 📁 Folder Structure Overview

medical-diagnosis-app/
│
├── app.py # Main Streamlit app
├── requirements.txt # List of dependencies
├── README.md # Project documentation
├── credentials.json # Gmail OAuth 2.0 credentials
├── screenshots/ # Screenshots for README
├── reports/ # Generated PDF reports
├── database/ # SQLite DB and backup scripts
├── utils/ # Utility functions (auth, plotting, etc.)
└── .gitignore # Files/folders to ignore in version control


### 🔌 Setup Instructions

1. **Clone the Repository**

```bash
git clone https://github.com/your-username/medical-diagnosis-app.git
cd medical-diagnosis-app
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt


###Setup Gmail API Credentials

Go to Google Cloud Console

Enable the Gmail API

Create OAuth 2.0 Credentials (Desktop App type)

Download credentials.json and place it in your project folder

On first run, a token will be generated and stored for future email sending.

#### Run the Application
streamlit run app.py


🚀 Advanced Usage
🧪 Testing: Add unit tests for core components in a /tests folder.
🐳 Docker Support (coming soon): Easily containerize for production.
🌐 Streamlit Cloud Deployment: Push to GitHub and deploy instantly.
🔐 Session Management: Auto-logout after session expiry.
📅 Date Filtering: Filter patient data across time using interactive UI.












