# ETL Pipeline: MySQL to MongoDB  

This project demonstrates a simple **ETL (Extract, Transform, Load) pipeline** that transfers data from a MySQL database into MongoDB.  

- **Extract**: Connects to MySQL using SQLAlchemy and retrieves employee records.  
- **Transform**: Cleans the data with pandas (removes duplicates, handles missing values, converts dates).  
- **Load**: Inserts data into MongoDB with upsert logic to avoid duplicates (based on `emp_id`).  

### Features  
- Environment variable support via `.env` (secure credentials management).  
- Data cleaning with pandas before loading.  
- Upsert strategy to ensure no duplicate records in MongoDB.  
- Automatic index creation on `emp_id` for efficiency.  

### Tech Stack  
- **Python** (pandas, SQLAlchemy, PyMySQL, PyMongo)  
- **MySQL** (source database)  
- **MongoDB** (target database)  

This repo is a beginner-friendly example of building data pipelines with Python.  
