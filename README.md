
# Banking Loan Analysis

Develop a basic understanding of risk analytics in banking and financial services and understand how data is used to minimise the risk of losing money while lending to customers.





## Tech Stack

*Python*

*My Sql*

*Jupyter Notebook*

*Power Bi*

## Installation

1.Install Power BI Desktop

2.Clone this repository.

3.Open the .pbix file (Banking Dashboard_new.pbix) in Power BI Desktop.

4.Update data source connections if necessary.

5.Explore dashboards interactively.
    
## Deployment

To deploy this project run

```bash
  npm run deploy
```


## Workflow
Data was extracted from MySQL using the **MySQL Python Connector** and **Jupyter Notebook**:

1. **Python Environment Setup**  
    Install required libraries:
     ```python
     pip install mysql-connector-python pandas
     ```
2. **Connect to MySQL**
   ```python
   import mysql.connector
   import pandas as pd

  Connect to MySQL database
   ```python
  cnx = mysql.connector.connect(
    host="127.0.0.1",
    port=3306,
    user="root",
    password="*******"
  )
Loading Data
df=pd.read_sql(query,cnx)
ref.ipynb file
```
3. Data Cleaning
```python
df=df.rename(columns={'ï»¿Client ID':'Client ID'})
# Check for missing values
missing_values = df.isnull().sum()
```
## Power BI Dashboard

**Home**
![alt image](https://github.com/MohTarique/Banking_Loan_Analysis/blob/main/Screenshot%20(62).png)

**Loan Analysis**
![alt image](https://github.com/MohTarique/Banking_Loan_Analysis/blob/main/Screenshot%20(63).png)

**Deposit Analysis**
![alt image](https://github.com/MohTarique/Banking_Loan_Analysis/blob/main/Screenshot%20(64).png)

**Summary**
![alt image](https://github.com/MohTarique/Banking_Loan_Analysis/blob/main/Screenshot%20(65).png)

