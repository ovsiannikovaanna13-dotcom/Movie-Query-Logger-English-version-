# 🎬 Movie Query Logger

A Python CLI project for searching movies in a MySQL database (sakila), saving queries to MongoDB, and analyzing query statistics.

---

## 📌 Features

- **Movie search:** by keyword, by genre & year range  
- **Query logging:** save results to MongoDB automatically  
- **Analytics:** view recent queries & top 5 popular queries  
- **Interactive CLI:** easy-to-use console interface  

---

## 🛠️ Technologies Used

- Python 3  
- Jupyter Notebook  
- MySQL (sakila)  
- MongoDB  
- PyMongo  
- mysql-connector-python  
- Aggregation Pipeline (MongoDB)

---

## 🗄️ MySQL Connection

```python
import mysql.connector

conn = mysql.connector.connect(
    host='ich-db.edu.itcareerhub.de',
    port='3306',
    user='ich1',
    password='password',
    database='sakila'
)

cursor = conn.cursor()

---

## 🔌 MongoDB Connection

```python
from pymongo import MongoClient

client = MongoClient(
    "mongodb://<username>:<password>@mongo.itcareerhub.de/?readPreference=primary&ssl=false&authMechanism=DEFAULT&authSource=ich_edit"
)

db = client["ich_edit"]
collection = db["final_project_dam130625_H_Ovsiannikova"]
