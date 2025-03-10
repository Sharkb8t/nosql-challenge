## nosql-challenge

# *East Safe, Love* - NoSQL Analysis

A **NoSQL** database analysis using **MongoDB** and **Jupyter Notebook** to explore food hygiene ratings in the UK. This project supports the magazine *Eat Safe, Love* by identifying food establishments based on their ratings and hygiene scores.

## 📌 Project Overview

The UK Food Standards Agency evaluates food establishments and assigns hygiene ratings. This project:

✅ Imports and manages data in a MongoDB NoSQL database

✅ Updates the database with new establishments and cleans data types

✅ Performs exploratory analysis using PyMongo and Pandas

✅ Identifies insights for food critics and journalists

## 📂 Repository Structure
```bash
📦 nosql-challenge
│── 📁 Resources/                 # Contains the original JSON dataset
├── 📓 NoSQL_setup_starter.ipynb  # Database setup and data import
├── 📓 NoSQL_analysis.ipynb       # Exploratory data analysis
│── 📜 README.md                   # Project documentation
```

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository
```sh
git clone https://github.com/your-username/nosql-challenge.git
cd nosql-challenge
```

### 2️⃣ Install Dependencies
```sh
pip install pymongo
```

### 3️⃣ Start MongoDB
Ensure MongoDB is running locally before importing data:
```sh
mongod --dbpath /path/to/your/data/directory
```

### 4️⃣ Import the Dataset
In PowerShell/Terminal, navigate to the `Resources/` folder and run:
```sh
mongoimport --type json -d uk_food -c establishments --drop --jsonArray --file "Resources/establishments.json"
```

### 5️⃣ Open Jupyter Notebook
```sh
jupyter notebook
```

### 6️⃣ Run the notebooks in order:

1.) `NoSQL_setup_starter.ipynb`

2.) `NoSQL_analysis.ipynb`

## 📊 Analysis Breakdown:

### 📌 Part 1: Database & Jupyter Setup

- Imported JSON data into MongoDB

- Verified database creation and collections

- Reviewed an example document

### 📌 Part 2: Updating the Database

- Added a new restaurant (Penang Flavours)

- Updated missing business type IDs

- Removed establishments from Dover

- Converted incorrect data types for geolocation and rating values

### 📌 Part 3: Exploratory Analysis

- Found establishments with hygiene score = 20

- Identified highly rated establishments in London

- Located top 5 best-rated restaurants near "Penang Flavours"

- Ranked Local Authorities with the most establishments scoring hygiene = 0

## 🛠 Technologies Used

> Python (3.8+)

> MongoDB (NoSQL database)

> PyMongo (MongoDB driver for Python)

> Pandas (Data analysis)

> Jupyter Notebook (Interactive coding)

> PowerShell/Command Prompt (for data import)
