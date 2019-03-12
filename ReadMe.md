# Database Final Project

Michael Nunziata, Diandre Clarke, George Halvatzis

### Step 1: ERD

- Based on the csv files provided in the SourceData, we built our ERD with relevant information.
    - ERD: [CourseDataERD](CourseDataERD.pdf)
    - Data Dictionary: [CourseDataDictionary](CourseDataDictionary.md)
    
### Step 2: Recreating ERD in SQL

- Our next step was to create our ERD in Jupyter as we learned in class.
- We used the CREATE TABLE and pd.to_sql functions to create our ERD and import_ tables.
- Using SQL's INSERT INTO function, we extract the data from the import tables into our created ERD tables.
- Notebook: [CourseDataETL](CourseDataETL.ipynb)

### Step 3: CourseData.db Integrity Checks

- Next, we run integrity checks on our five tables.
- We ran Domain, Entity, and Relational Integrity Checks.
- In the Relational Integrity Checks, we ran multiple queries with necessary joins to test the connections between tables and display some information we thought would be interesting.
- Notebook: [CourseDataTests](CourseDataTests.ipynb)

### Step 4: Star Schema

- Based on the ERD and SQL tables created earlier, we designed a Star Schema to make extracting data much simpler using SQL.
- We decided to exclude the course_meetings data as it caused many problems with importing and we still had other questions to explore.
- Star Schema: [Star Schema](DataWarehouseERD.pdf)

### Step 5: Data Warehouse Creation

- We used similar steps in this one as in Step 2. The only difference between the two is importing the data.
    - For the Warehouse, we used the SQL command 'attach' to open CourseData.db in this notebook. We then used this command to insert data from the first database into CourseDataWarehouse.db.
- Notebook: [CourseDataWarehouse](CourseDataWarehouse.ipynb)

### Step 6: CourseDataWarehouse.db Integrity Checks and Demo

- Just as earlier, we performed integrity checks on the Data Warehouse.
- We ran interesting queries based on questions we thought would be interesting to answer.
- Notebook: [CourseDataWarehouseTestAndDemo](CourseDataWarehouseTestAndDemo.ipynb)