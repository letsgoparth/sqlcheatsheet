# sqlcheatsheet
SQL Cheat Sheet/ Notes

<a name="readme-top"></a>

<a href="https://www.linkedin.com/in/itsparthverma"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"><a>

<br/>
<div align="center">
  <a href="https://www.mysql.com">
    <img src="images/logo.png" alt="Logo" width="180" height="80">
  </a>
  

  <h3 align="center">SQL Cheat Sheet</h3>

  <p align="center">
    SQL Notes to recall sql methods and functions
    <br />
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#insert">INSERT</a>
      <ul>
        <li><a href="#Inserting-single record">Inserting single record</a></li>
        <li><a href="#Inserting-with-reference-to-fields">Inserting with reference to fields</a></li>
        <li><a href="#inserting-multiple-records">Inserting Multiple Records</a></li>
      </ul>
    </li>
    <li>
      <a href="#insert">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#copy-table">Copy Table</a></li>
    <li><a href="#roadmap">Update</a></li>
    <li><a href="#contributing">Delete</a></li>
    <li><a href="#license">Select</a></li>
    <li><a href="#contact">Limit</a></li>
    <li><a href="#acknowledgments">Alias</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## Insert
### Inserting single record

  ```sql
  INSERT INTO customers
  VALUES(‘Chester’, ‘Bennington’,’199901-01’)
  ```
### Inserting with reference to fields

  ```sql
  INSERT INTO customers(
      id,
      first_name,
      last_name)

  VALUES(
    1,
    ‘Mike’,
    ‘Shinoda’)

  ```
### Inserting Multiple Records
  ```sql
  INSERT INTO customers(
    First_name,
    Last_name,
    Instrument)
  VALUES
    (‘Mike’, ’Shinoda’, ’Producer’),
    (‘Joe’, ‘Hann’, Turntables’),
    (‘Rob’, ’Bourdon’, Drums’),

  ```


<p align="right">(<a href="#readme-top">back to top</a>)</p>


## Copy Table

### Copying table as it is

```sql
CREATE TABLE orders_archived AS
SELECT * FROM orders
```
### Copying with condition

```sql
CREATE TABLE orders_archived
SELECT * 
FROM orders
WHERE order_date <’2019-01-01’
 ```

## Update


```sql
UPDATE invoices
SET
payment_total = 0,
payment_date = ‘2019-03-01’
WHERE invoice_id = 1
```
 
