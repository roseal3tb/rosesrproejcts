# Tuwaiq Academy — Student Information & Academic Management System

An integrated database application designed for **Tuwaiq Academy** to streamline student administrative and academic tracking. The system manages core institutional operations—including student records, course offerings, grade recording, attendance tracking, and class scheduling—providing a structured data foundation to improve administrative efficiency and academic monitoring.


## 📌 Project Overview

Managing student lifecycles and tracking academic progress manually can lead to data fragmentation and operational bottlenecks. This project provides a centralized, relational database application designed to automate and unify academic tracking for Tuwaiq Academy.

### Key Objectives

* **Centralize Data:** Standardize records for students, instructors, courses, and cohorts.
* **Track Attendance & Grades:** Provide real-time data entry and queries for attendance logs and assessment scores.
* **Manage Schedules:** Prevent timetable overlaps for instructors, classrooms, and student groups.
* **Simplify Reporting:** Enable quick reporting on student performance, attendance rates, and enrollment metrics.


## ✨ Features

* **Student Profile Management:** Tracks enrollment status, contact details, academic paths, and progress updates.
* **Course & Cohort Registration:** Handles course prerequisite mapping, batch/cohort assignments, and seat limits.
* **Attendance Tracking System:** Logs daily/session attendance status (Present, Late, Absent, Excused) with summary aggregations.
* **Gradebook & Performance Analytics:** Records assignments, quizzes, midterms, and final project grades to calculate total performance.
* **Dynamic Scheduling:** Organizes course tracks, room assignments, and lecture times across active academy bootcamps.


## 🛠️ Tech Stack & Database Architecture

* **Database / RDBMS:** PostgreSQL / MySQL / SQLite
* **Backend Framework:** *[e.g., Python (FastAPI / Django) / Node.js (Express) / Java (Spring Boot)]*
* **ORM / Database Access:** *[e.g., SQLAlchemy / Prisma / Hibernate]*
* **Frontend Interface:** *[e.g., React / Next.js / Streamlit / HTML5 & Bootstrap]*


## 🗄️ Relational Schema (ERD Overview)

```text
  ┌──────────────┐       ┌─────────────────┐       ┌──────────────┐
  │   Students   │───<   │   Enrollments   │   >───│   Courses    │
  └──────────────┘       └─────────────────┘       └──────────────┘
         │                         │                      │
         │                         │                      │
         ▼                         ▼                      ▼
  ┌──────────────┐       ┌─────────────────┐       ┌──────────────┐
  │  Attendance  │       │     Grades      │       │  Schedules   │
  └──────────────┘       └─────────────────┘       └──────────────┘

```

### Core Entities & Relationships

* **Students:** Primary user data (ID, name, email, track, enrollment date).
* **Courses / Bootcamps:** Course details, instructor mappings, and credit/hour breakdowns.
* **Enrollments:** Junction table managing many-to-many relationships between Students and Courses.
* **Attendance:** Daily transactional records linked to student IDs and specific course sessions.
* **Grades:** Detailed logs of raw scores, weighted percentages, and assessment categories.
* **Schedules:** Timetable details specifying day, time slots, instructors, and physical/virtual rooms.
