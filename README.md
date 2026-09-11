# Invigilation Management System

A Django-based web application designed to simplify and manage examination invigilation activities in educational institutions. The system helps administrators manage faculty, exams, timetables, invigilation assignments, leaves, notifications, and reports through a centralized platform.

> **Academic Project** — Developed/adapted for learning and academic purposes.

---

## 📌 Project Overview

Managing examination invigilation manually can be time-consuming and may lead to scheduling conflicts, uneven workload distribution, and communication delays.

The **Invigilation Management System** provides a centralized solution for:

* Faculty management
* Exam scheduling
* Invigilation allocation
* Faculty timetable management
* Leave management
* Notifications
* Workload monitoring
* Reports and analytics

The system provides separate interfaces and workflows for **Administrators** and **Faculty**.

---

## 🎯 Objectives

* Reduce manual effort involved in assigning invigilation duties.
* Avoid assigning faculty to duties that conflict with their timetable or leave.
* Support cross-department invigilation allocation.
* Provide faculty with clear visibility of their assigned duties.
* Improve communication through notifications and reminders.
* Maintain records of important system activities.

---

## ✨ Features

### 👨‍💼 Administrator

* Faculty profile management
* Batch faculty creation
* Exam creation and scheduling
* Exam hall management
* Invigilation allocation
* Allocation suggestions
* Faculty timetable management
* Leave request management
* Notifications and reminders
* Workload reports
* Department statistics
* Audit/action logs

### 👩‍🏫 Faculty

* Personal dashboard
* View invigilation assignments
* Accept or decline assignments
* View timetable
* Apply for leave
* Track leave requests
* View notifications
* View personal workload information

---

## 🧠 Smart Invigilation Allocation

The system supports intelligent allocation of faculty members by considering factors such as:

* Faculty availability
* Teaching timetable
* Leave status
* Department
* Previous workload
* Examination schedule

Cross-department allocation can also be used to reduce potential assignment bias.

---

## 🔄 Main Workflow

```text
Create Exam
     ↓
Configure Exam Halls
     ↓
Check Faculty Availability
     ↓
Generate Allocation Suggestions
     ↓
Assign Invigilators
     ↓
Notify Faculty
     ↓
Faculty Accepts / Declines
     ↓
Track Allocation & Workload
     ↓
Generate Reports
```

---

## 🛠️ Technology Stack

| Category           | Technology                       |
| ------------------ | -------------------------------- |
| Backend            | Python, Django                   |
| Frontend           | HTML, CSS, Bootstrap, JavaScript |
| Database           | SQLite                           |
| Charts & Analytics | Chart.js                         |
| Authentication     | Django Authentication            |
| Email              | SMTP / Django Email Backend      |
| Version Control    | Git & GitHub                     |

---

## 📂 Project Structure

```text
Invigilation-System/
│
├── accounts/                 # User and faculty management
├── exams/                    # Exam and invigilation management
├── leaves/                   # Leave management
├── notifications/            # Notification functionality
├── timetable/                # Faculty timetable management
├── invigilation_system/      # Main Django project configuration
│
├── templates/                # HTML templates
├── TIME TABLES/              # Department timetable files
├── Requirements and execution/
│   ├── EXECUTION_PROCESS.txt
│   └── SOFTWARE_REQUIREMENTS.txt
│
├── manage.py                 # Django management script
├── requirements.txt          # Python dependencies
├── .env.example              # Environment variable template
├── .gitignore                # Git ignored files
└── README.md                 # Project documentation
```

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Swathi-13k/Invigilation-System.git
cd Invigilation-System
```

### 2. Create a Virtual Environment

#### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

#### Linux / macOS

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables

Create a `.env` file based on `.env.example`.

Example:

```env
SECRET_KEY=your-secret-key
DEBUG=True
ALLOWED_HOSTS=localhost,127.0.0.1
```

If email functionality is required, configure the required SMTP settings in the environment file.

> **Note:** Never upload real passwords, API keys, email passwords, or other secret credentials to GitHub.

### 5. Apply Database Migrations

```bash
python manage.py migrate
```

### 6. Create an Admin Account

```bash
python manage.py createsuperuser
```

Follow the instructions shown in the terminal.

### 7. Start the Development Server

```bash
python manage.py runserver
```

### 8. Open the Application

Open the following address in your browser:

```text
http://127.0.0.1:8000/
```

---

## 🔐 Security

The application uses Django's built-in security mechanisms and includes features such as:

* User authentication
* Role-based access
* Password management
* OTP verification workflows
* CSRF protection
* Audit logging
* Environment-based configuration

Sensitive configuration values should be stored in `.env` and should **not** be committed to GitHub.

---

## 📊 Reports & Analytics

The system provides reporting functionality for monitoring:

* Faculty workload
* Department statistics
* Invigilation allocation
* Assignment responses
* Allocation activity

These reports help administrators monitor examination-related activities more efficiently.

---

## 📱 Responsive Interface

The application uses a responsive web interface designed to work across:

* Desktop computers
* Laptops
* Tablets
* Mobile devices

---

## 🎓 Academic Context

This project is suitable for educational institutions that need to manage:

* Multiple departments
* Faculty members
* Semester-based courses
* Examination schedules
* Examination halls
* Faculty availability
* Invigilation duties
* Leave requests

---

## 👩‍💻 Project Contribution

This repository contains an adapted academic version of an existing invigilation-management project.

My work on this repository focuses on understanding, configuring, testing, documenting, and extending the application as part of my academic/project learning.

Specific contributions should be described based on the features actually implemented or modified.

---

## 📚 Learning Outcomes

Through this project, the following concepts can be practiced:

* Django web application development
* Python programming
* Database management
* CRUD operations
* Authentication and authorization
* HTML/CSS/Bootstrap
* JavaScript
* Git and GitHub
* Project configuration
* Web application testing
* Software documentation

---

## 🚀 Future Enhancements

Possible future improvements include:

* Cloud deployment
* PostgreSQL database integration
* Advanced allocation optimization
* Mobile application support
* Improved analytics dashboards
* Automated conflict detection
* Additional notification channels
* Role-specific access controls

---

## 📌 Project Status

**Status:** Academic / Development Project

The application is intended for learning, demonstration, and academic project purposes. Further testing and configuration are required before considering deployment in a real institutional environment.

---

## 📄 License

This repository does not currently include a separate license file. Usage and redistribution should follow the permissions and attribution requirements of the original project and its contributors.
