# Predictive Maintenance System using NASA C-MAPSS Dataset

---

## Table of Contents

- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Dataset Information](#dataset-information)
- [How to Run the Project](#how-to-run-the-project)
- [Key Features Implemented](#key-features-implemented)
- [Future Enhancements](#future-enhancements)
- [Example Use Cases](#example-use-cases)
- [License](#license)

---

## Project Overview

This project implements a **Predictive Maintenance System** using the [NASA C-MAPSS Turbofan Engine Degradation Dataset](https://data.nasa.gov/docs/legacy/CMAPSSData.zip). The objective is to analyze engine sensor data, identify degradation stages, perform fault classification, and support Remaining Useful Life (RUL) prediction workflows.

The notebook demonstrates a complete machine learning workflow for predictive maintenance, including:

- Data loading and preprocessing
- Sensor feature engineering
- Clustering-based degradation stage labeling
- Exploratory Data Analysis (EDA)
- Fault stage visualization
- Machine learning preparation for predictive maintenance tasks

This project is highly relevant for:

- Industrial AI
- AIOps for manufacturing
- Aircraft engine health monitoring
- Predictive maintenance systems
- Reliability engineering
- Data-driven anomaly detection

---

## Technologies Used

| Category             | Technologies        |
| -------------------- | ------------------- |
| Programming Language | Python 3.8+         |
| Notebook Environment | Jupyter Notebook    |
| Data Processing      | Pandas, NumPy       |
| Visualization        | Matplotlib, Seaborn |
| Machine Learning     | Scikit-learn        |
| Clustering           | KMeans              |
| Dataset              | NASA C-MAPSS        |

---

## Project Structure

```text
Predictive-Maintenance-System/
│
├── predictive_maintenance_system.ipynb   # Main analysis notebook
├── README.md                             # Project documentation
├── requirements.txt                      # Python dependencies
└── dataset/
    ├── train_FD001.txt
    ├── test_FD001.txt
    ├── RUL_FD001.txt
    └── ...
```

---

## Dataset Information

This project uses the **NASA C-MAPSS** (Commercial Modular Aero-Propulsion System Simulation) dataset. The dataset contains simulated turbofan engine degradation data collected from multiple engine units operating under different conditions. Each engine unit starts with normal operating conditions and gradually develops faults over time.

### Dataset Includes

- Engine operational settings
- Multiple sensor measurements
- Engine cycles until failure
- Remaining Useful Life (RUL) information

### Dataset Download

Download the dataset directly from NASA:

**URL:** [https://data.nasa.gov/docs/legacy/CMAPSSData.zip](https://data.nasa.gov/docs/legacy/CMAPSSData.zip)

### Steps to Set Up the Dataset

#### 1. Download the Dataset

Open the NASA dataset link and download the ZIP file to your local system.

#### 2. Extract the ZIP File

- **Windows:** Right-click the ZIP file → Select *Extract All*
- **macOS / Linux:**

  ```bash
  unzip CMAPSSData.zip
  ```

#### 3. Dataset Files

After extraction, you will find files such as:

```text
train_FD001.txt  train_FD002.txt  train_FD003.txt  train_FD004.txt
test_FD001.txt   test_FD002.txt   test_FD003.txt   test_FD004.txt
RUL_FD001.txt    RUL_FD002.txt    RUL_FD003.txt    RUL_FD004.txt
```

#### 4. Create the Dataset Folder

Inside your project directory, create a folder named `dataset/` and move all extracted files into it:

```text
Predictive-Maintenance-System/
│
├── predictive_maintenance_system.ipynb
└── dataset/
    ├── train_FD001.txt
    ├── test_FD001.txt
    ├── RUL_FD001.txt
    └── ...
```

---

## How to Run the Project

### 1. Clone the Repository

```bash
git clone <your-github-repo-link>
cd Predictive-Maintenance-System
```

### 2. Create a Virtual Environment (Recommended)

```bash
python -m venv venv

# Activate on macOS/Linux
source venv/bin/activate

# Activate on Windows
venv\Scripts\activate
```

### 3. Install Required Libraries

Using `requirements.txt`:

```bash
pip install -r requirements.txt
```

Or manually:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 4. Set Up the Dataset

Follow the [Dataset Information](#dataset-information) steps above to download and place the dataset files in the `dataset/` folder.

### 5. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `predictive_maintenance_system.ipynb` and run all cells sequentially.

---

## Key Features Implemented

### Data Preprocessing

- Missing value handling
- Low variance sensor removal
- Feature scaling
- Sensor normalization

### Clustering-Based Degradation Labeling

- KMeans clustering
- Multi-stage degradation classification
- Engine health stage grouping

### Exploratory Data Analysis

- Sensor trend visualization
- Failure stage analysis
- Cluster distribution plots
- Correlation analysis

### Predictive Maintenance Workflow

- Fault progression understanding
- Health monitoring foundation
- RUL modeling preparation

---

## Future Enhancements

Potential future improvements include:

- [ ] Deep Learning models for RUL prediction
- [ ] LSTM-based sequence prediction
- [ ] Transformer models for time-series analysis
- [ ] Real-time anomaly detection
- [ ] Streamlit dashboard deployment
- [ ] Integration with industrial IoT systems
- [ ] Explainable AI (XAI) for maintenance insights

---

## Example Use Cases

This project can be adapted for:

- Aircraft engine maintenance
- Manufacturing equipment monitoring
- Industrial IoT analytics
- Smart factory systems
- Predictive failure analysis
- Reliability engineering research

---



> **Dataset credit:** NASA Prognostics Center of Excellence — C-MAPSS Turbofan Engine Degradation Simulation Dataset.
