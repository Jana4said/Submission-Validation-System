# Submission Validation System

This project implements a **student submission system** built with **Deno**, featuring both **client-side and server-side validation**.  
It ensures data integrity, prevents duplicate uploads, and integrates with an **SQLite database** for secure record storage.

---

## Features
- Validates filenames, student IDs, and question formats  
- Ensures correct number of questions (e.g., 5 or 6)  
- Implements **server-side validation** to prevent invalid JSON uploads  
- Detects and blocks duplicate student submissions  
- Supports database schema updates for additional questions  
- Generates submission analysis (total submissions, empty answers count)  
- Provides detailed error handling with status codes (`400 Bad Request`, `409 Conflict`)  

---

## Core Concepts
- Client and server validation logic  
- Regular expressions for filename verification  
- Handling JSON requests in Deno  
- Database schema management and SQL queries  
- Preventing duplicates via `COUNT(*)` checks in SQLite  
- Generating structured HTML reports dynamically  

---

## File Overview
| File | Description |
|------|--------------|
| `comp2406-assign3-janasaid.txt` | Implementation summary, validation logic, and testing documentation |

---

##  Technologies Used
- **JavaScript (Deno Runtime)**  
- **SQLite Database**  
- **HTML/CSS (Client Interface)**  
- **Regex Validation**  
- **Server-side JSON Parsing**

---
**Gana Said**  
Bachelor of Computer Science (AI Stream) – Carleton University  
📧 [janasaid@cmail.carleton.ca](mailto:janasaid@cmail.carleton.ca)

---

## How It Works
1. The client uploads a `.txt` submission file.  
2. The server validates filename, structure, and content.  
3. Valid submissions are stored in the SQLite database.  
4. The system rejects duplicates or malformed submissions.  
5. Analysis page displays submission stats and empty answers.

---
*This project demonstrates full-stack development using Deno, SQLite, and strong validation techniques.*
