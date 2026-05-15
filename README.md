Predictive Maintenance System using NASA C-MAPSS Dataset
Project Overview
This project implements a Predictive Maintenance System using the NASA C-MAPSS Turbofan Engine Degradation Dataset. The objective is to analyze engine sensor data, identify degradation stages, perform fault classification, and support Remaining Useful Life (RUL) prediction workflows.
The notebook demonstrates a complete machine learning workflow for predictive maintenance, including:
•	Data loading and preprocessing
•	Sensor feature engineering
•	Clustering-based degradation stage labeling
•	Exploratory Data Analysis (EDA)
•	Fault stage visualization
•	Machine learning preparation for predictive maintenance tasks
This project is highly relevant for:
•	Industrial AI
•	AIOps for manufacturing
•	Aircraft engine health monitoring
•	Predictive maintenance systems
•	Reliability engineering
•	Data-driven anomaly detection
 
 Technologies Used
Category	Technologies
Programming Language	Python
Notebook Environment	Jupyter Notebook
Data Processing	Pandas, NumPy
Visualization	Matplotlib, Seaborn
Machine Learning	Scikit-learn
Clustering	KMeans
Dataset	NASA C-MAPSS
 
 Project Structure
Predictive-Maintenance-System/
│
├── predictive_maintenance_system.ipynb
├── README.md
├── requirements.txt
└── dataset/
    ├── train_FD001.txt
    ├── test_FD001.txt
    ├── RUL_FD001.txt
    └── ...
 
Dataset Information
This project uses the NASA C-MAPSS (Commercial Modular Aero-Propulsion System Simulation) dataset.
The dataset contains simulated turbofan engine degradation data collected from multiple engine units operating under different conditions.
Each engine unit starts with normal operating conditions and gradually develops faults over time.
Dataset Includes
•	Engine operational settings
•	Multiple sensor measurements
•	Engine cycles until failure
•	Remaining Useful Life (RUL) information
 
**Dataset Download Link**
Download the dataset directly from NASA:
url for NASA C-MAPSS Dataset: https://data.nasa.gov/docs/legacy/CMAPSSData.zip
 
**Steps to Access and Use the Dataset**
1.	Download the Dataset
Open the NASA dataset link:
https://data.nasa.gov/docs/legacy/CMAPSSData.zip
Download the ZIP file to your local system.
 
2.	Extract the ZIP File
After downloading:
Windows
•	Right-click the ZIP file
•	Select Extract All
macOS / Linux
unzip CMAPSSData.zip
 
3.	Dataset Files
After extraction, you will see files such as:
train_FD001.txt
train_FD002.txt
train_FD003.txt
train_FD004.txt

test_FD001.txt
...

RUL_FD001.txt
...
 
4. Create Dataset Folder
Inside your project directory, create a folder named:
dataset/
Move all extracted dataset files into this folder.
Final structure:
Predictive-Maintenance-System/
│
├── predictive_maintenance_system.ipynb
├── dataset/
│   ├── train_FD001.txt
│   ├── test_FD001.txt
│   ├── RUL_FD001.txt
│   └── ...
 
**How to Run the Project**
1. Clone the Repository
git clone <your-github-repo-link>
cd Predictive-Maintenance-System
 
2. Install Required Libraries
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
Or using requirements.txt:
pip install -r requirements.txt
 
3. Launch Jupyter Notebook
jupyter notebook
Open:
predictive_maintenance_system.ipynb
Run all notebook cells sequentially.
 
 Key Features Implemented
 Data Preprocessing
•	Missing value handling
•	Low variance sensor removal
•	Feature scaling
•	Sensor normalization
 Clustering-Based Degradation Labeling
•	KMeans clustering
•	Multi-stage degradation classification
•	Engine health stage grouping
Exploratory Data Analysis
•	Sensor trend visualization
•	Failure stage analysis
•	Cluster distribution plots
•	Correlation analysis
Predictive Maintenance Workflow
•	Fault progression understanding
•	Health monitoring foundation
•	RUL modeling preparation
 
 Future Enhancements
Potential future improvements include:
•	Deep Learning models for RUL prediction
•	LSTM-based sequence prediction
•	Transformer models for time-series analysis
•	Real-time anomaly detection
•	Streamlit dashboard deployment
•	Integration with industrial IoT systems
•	Explainable AI (XAI) for maintenance insights
 
 Example Use Cases
This project can be adapted for:
•	Aircraft engine maintenance
•	Manufacturing equipment monitoring
•	Industrial IoT analytics
•	Smart factory systems
•	Predictive failure analysis
•	Reliability engineering research
 

