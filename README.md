# sqlcheatsheet
SQL Cheat Sheet/ Notes
# sqlcheatsheet
SQL Cheat Sheet/ Notes
<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
<!-- 

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url] -->

<a href="jkdasfhlks.com"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"><a>

<!-- PROJECT LOGO -->
<br/>
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="images/logo.png" alt="Logo" width="180" height="80">
  </a>
  

  <h3 align="center">SQL Cheat Sheet</h3>

  <p align="center">
    SQL Notes to recall sql methods and functions
    <br />
    <!-- <a href="https://github.com/othneildrew/Best-README-Template"><strong>Explore the docs »</strong></a> -->
    <!-- <br /> -->
    <!-- <br />
    <a href="https://github.com/othneildrew/Best-README-Template">View Demo</a>
    ·
    <a href="https://github.com/othneildrew/Best-README-Template/issues">Report Bug</a>
    ·
    <a href="https://github.com/othneildrew/Best-README-Template/issues">Request Feature</a> -->
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#insert">INSERT</a>
      <ul>
        <li><a href="#built-with">Insaerting Multiple Records</a></li>
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
 