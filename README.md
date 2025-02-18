# gpa_calculator

# GPA Calculator - Google Colab

## 📌 Overview
This Python script calculates the **GPA (Grade Point Average) for students** based on their grades in multiple subjects. The script reads a CSV file containing student grades, maps them to grade points, and computes GPA using a weighted average method.

## 🚀 Features
- **Supports all standard grade formats** (A+, A, B+, B, etc.)
- **Handles missing values (`NaN`) safely**
- **Uses credit-weighted average for GPA calculation**
- **Displays GPA for all students**
- **Visualizes GPA distribution with a histogram**

## 📂 Required Input File
The input should be a CSV file with the following columns:
- `DM` (Discrete Mathematics)
- `FLA` (Formal Languages & Automata)
- `CN` (Computer Networks)
- `BD` (Big Data)
- `COMM` (Communication Skills)
- `CC` (Cloud Computing)
- `CNS` (Cryptography & Network Security)
- `FS` (Full Stack Development)
- `SRWC` (Software Requirements & Costing)

## 🛠 How to Use
### 1️⃣ Upload the CSV file in Google Colab
Run the script and it will prompt you to upload your `.csv` file.

### 2️⃣ Run the Python Script
The script will:
- Read the CSV file
- Convert grades to grade points
- Calculate GPA for each student
- Display student-wise GPA
- Show a histogram of GPA distribution

### 3️⃣ View the Output
- A **table** showing student GPAs
- A **histogram** visualizing GPA distribution

## 📊 GPA Calculation Formula
\[ GPA = \frac{\sum (Grade Point \times Credit)}{Total Credits} \]

## 🔗 Example Usage in Google Colab
```python
from google.colab import files
uploaded = files.upload()

import pandas as pd
import matplotlib.pyplot as plt

# Load the uploaded file
df = pd.read_csv("SEM.csv")
# Process and calculate GPA
# (Refer to full script in this repository)
```

## 📌 Notes
- Ensure the CSV file matches the expected column structure.
- The script **automatically assigns grade points** and credits.
- The final GPA is **out of 10.0**.

## 🤝 Contributing
Feel free to modify and improve the script. Suggestions and improvements are welcome!

## 📜 License
This project is open-source and free to use.
