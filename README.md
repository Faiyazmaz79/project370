# 🎓 University Portal — CSE370 Database Systems Project
Main Contributor - Mohammad Faiyaz Mazumder
**BRAC University | Spring 2026 | Lab Group 01**

---

## 👥 Group Members 3

| Name | Student ID | Department |
|------|-----------|------------|
| Mohammad Faiyaz Mazumder  | 24101352 | CSE |
| Fabiha Islam  | 22301002 | CSE |
| Shuvo Das  | 22301003 | CSE |

---

## 📌 Project Overview

A University Portal web application designed to manage and streamline
academic activities at BRAC University. The system handles student
enrollment, grades, exam schedules, complaints, notes sharing,
reward points, lab availability, and semester fees.

---

## ✅ Features (14 Total)

### Unique Features
| # | Feature | Description |
|---|---------|-------------|
| F01 | Smart Course Recommendation | Suggests next courses based on completed prerequisites |
| F02 | Performance Analytics Dashboard | Shows highest, lowest, average grades per course |
| F03 | Department Statistics | Displays total students, courses, faculty per department |
| F04 | Lab Availability Checker | Shows real-time lab occupancy and free slots |
| F05 | Complaint System | Students can file, view, and track campus complaints |
| F06 | Notes Resource Library | Upload, download, and rate study notes with reward points |

### Basic Features
| # | Feature | Description |
|---|---------|-------------|
| F07 | Reward Points & Leaderboard | Points earned by uploading notes |
| F08 | Credit Limit Checker | Validates semester credit limits before enrollment |
| F09 | Course Enrollment | Enroll or drop courses with capacity validation |
| F10 | Classroom Capacity Checker | View available seats per course section |
| F11 | Grade Sheet | View letter grades and marks per semester |
| F12 | Exam Schedule | View midterm and final exam dates, times, rooms |
| F13 | Semester Fee Payment | Track and view payment status |
| F14 | Academic Routine | View weekly class and exam schedule |

---

## 🗄️ Database

- **DBMS:** MySQL
- **Tables:** 20 tables
- **Schema:** Based on approved EER Diagram (Chen Notation)

### Tables
| Table | Type | Description |
|-------|------|-------------|
| Department | Strong Entity | University departments |
| Faculty | Strong Entity | Faculty members |
| Student | Strong Entity | Enrolled students |
| Student_Phone | Multivalued Attribute | Student phone numbers |
| Classroom | Strong Entity (Superclass) | All rooms |
| Classroom_Lab_Room | Subclass | Lab rooms (floors 9–12) |
| Classroom_Theory_Room | Subclass | Theory classrooms |
| Course | Strong Entity | Offered courses |
| Prerequisite | Recursive Relationship | Course prerequisites |
| Enrolled_In | Relationship Table | Student ↔ Course enrollment |
| Grade | Weak Entity | Student grades per course |
| Exam | Strong Entity | Exam records |
| Section | Weak Entity | Course sections |
| Section_Timing | Weak Entity | Section schedule |
| Note | Weak Entity | Uploaded study notes |
| Reward_Points | Weak Entity | Points per student |
| Clubs | Entity | University clubs |
| Complaint | Weak Entity | Student complaints |
| Files | Relationship Table | Student ↔ Complaint |
| AcademicRoutine | Weak Entity | Student exam routine |
| Semester_Fees | Weak Entity | Fee payment records |
| AnalyticsDashboard | Derived Entity | Course performance stats |
| Smart_Recommendation | Derived Entity | Course recommendations |

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | HTML, CSS, JavaScript |
| Backend | PHP |
| Database | MySQL (phpMyAdmin) |
| Design | EER Diagram (ERDPlus + Draw.io) |

---

## 🚀 How to Run

### Requirements
- XAMPP (Apache + MySQL + PHP)
- Any modern browser

## 📊 EER Diagram

The EER Diagram was designed using **ERDPlus** and **Draw.io** as taught in CSE370.

Notation used:
- Rectangle → Strong Entity
- Double Rectangle → Weak Entity
- Oval → Attribute
- Underlined Oval → Key Attribute
- Dotted Oval → Derived Attribute
- Double Oval → Multivalued Attribute
- Diamond → Relationship
- Double Diamond → Identifying Relationship
- Circle with d → Disjoint Specialization

---

## 📝 SQL Concepts Used

- `CREATE TABLE` with Primary Keys and Foreign Keys
- `INSERT INTO` for data population
- `SELECT` with `JOIN` (INNER, LEFT)
- `GROUP BY` and `HAVING` with Aggregate Functions
- Subqueries and nested queries
- `AVG()`, `COUNT()`, `MAX()`, `MIN()`, `SUM()`

University-Portal-CSE370/
├── README.md                        # This file
├── database/
│   └── university_portal.sql        # Full schema + data
├── diagrams/
│   └── EER_Diagram.png              # Approved EER diagram
├── frontend/
│   └── index.html                   # Portal UI (HTML + CSS + JS)
└── backend/
└── backend.php                  # PHP API

