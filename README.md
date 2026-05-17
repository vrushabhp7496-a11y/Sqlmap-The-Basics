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

### I have added practical task from tryhackme lab :
-see screenshots below.



 
