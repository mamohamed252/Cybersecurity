---
Created: '"2025-01-27T11:46"'
Status: 🟡 In Progress
Links:
  - Labs
  - 00 - SQL injection
  - SQL
  - Learning Material
Deadline:
---
What is SQL?
	SQL (Structured Query Language) is a standardized language used to manage, query, and manipulate data in relational databases.

What is SQL injection (SQLi)
	SQL injection (SQLi) is a security vulnerability where attackers manipulate database queries, allowing unauthorized access to sensitive data, data modification, or even server compromise. ^1
	
Impact of SQL Injection
	A successful SQL injection attack can expose sensitive data like passwords and credit card details, cause data breaches, reputational harm, regulatory penalties, or long-term backdoor access.
Detecting SQL Injection
	Use systematic testing, such as injecting special characters, Boolean conditions, or time-delay payloads, to identify vulnerabilities. Automated tools like Burp Scanner can also help detect SQLi.

SQL Injection in Queries
	SQL injection can occur in various query sections like `WHERE`, `UPDATE`, `INSERT`, and `ORDER BY`. Attackers exploit these to manipulate database behavior.

Examples of SQL Injection
	Common techniques include retrieving hidden data, bypassing authentication, UNION attacks for extracting additional data, and blind SQL injection, where indirect indicators are used.

Second-order SQL Injection
	Occurs when developers safely store input in the database but later process it unsafely, mistakenly considering it trusted.

Examining the Database
	Attackers may identify database types, version details, and table structures using specific queries, aiding in exploiting vulnerabilities.

SQL Injection in Different Contexts
	SQLi attacks can target any input processed by SQL queries, including JSON, XML, or encoded formats, bypassing filters through obfuscation techniques.

Preventing SQL Injection
	Use parameterized queries (prepared statements) instead of string concatenation. For dynamic parts like table names, whitelist inputs or apply alternative logic.
	
References
	[[SQL Material PortSwigger#^dprnex]]
 