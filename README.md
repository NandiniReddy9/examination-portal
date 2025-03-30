# OnlineExaminationPortal
# Online Examination Portal

![Django](https://img.shields.io/badge/Framework-Django-green)  
![Python](https://img.shields.io/badge/Language-Python-blue)  
[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)  

## 📌 Project Overview
An **Online Examination Portal** built with Django, enabling students to take exams securely while allowing admins to manage exams efficiently.

### ✨ Key Features:
✅ **User Authentication** - Secure login for students and admins.  
✅ **Exam Management** - Admins can create, update, and delete exams.  
✅ **Question Bank** - Supports MCQs & Descriptive Questions with randomization.  
✅ **Timed Exams** - Auto-submission when the timer expires.  
✅ **Result Evaluation** - Auto-scoring for MCQs; manual review for descriptive answers.  
✅ **Admin Dashboard** - Track student performance & generate reports.  
✅ **Security** - Prevents multiple logins & restricts cheating.

---

## 📖 Table of Contents
- [Tech Stack](#-tech-stack)
- [Setup & Installation](#-setup--installation)
- [API Reference](#-api-reference)
- [Screenshots](#-screenshots)
- [Badges](#-badges)
- [Acknowledgements](#-acknowledgements)
- [Appendix](#-appendix)

---

## 🚀 Tech Stack
### **Frontend**:
- HTML, CSS, JavaScript, Bootstrap

### **Backend**:
- Django, Django REST Framework

### **Database**:
- PostgreSQL / MySQL

### **Authentication**:
- JWT-based authentication

---

## 🛠 Setup & Installation
```bash
# Clone the repository
git clone https://github.com/NandiniReddy9/OnlineExaminationPortal
cd onlineexaminationportal

# Create a virtual environment & activate it
python -m venv venv  
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt  

# Run migrations
python manage.py migrate  

# Start the server
python manage.py runserver  
```
Open **http://127.0.0.1:8000/** in your browser to access the portal.

---

## 📡 API Reference
### **1. Authentication APIs**
| Method | Endpoint | Description |
|--------|---------|-------------|
| `POST` | `/api/auth/register/` | User registration (Student/Admin) |
| `POST` | `/api/auth/login/` | User login & token generation |
| `POST` | `/api/auth/logout/` | Logout user & invalidate token |

### **2. Exam Management APIs (Admin Only)**
| Method | Endpoint | Description |
|--------|---------|-------------|
| `POST` | `/api/exams/` | Create a new exam |
| `GET` | `/api/exams/` | Get all exams |
| `GET` | `/api/exams/{exam_id}/` | Get details of a specific exam |
| `PUT` | `/api/exams/{exam_id}/` | Update exam details |
| `DELETE` | `/api/exams/{exam_id}/` | Delete an exam |

For the full API documentation, refer to **Swagger UI/Postman.**

---

## 📷 Screenshots
All screenshots related to the project are neatly organized in a dedicated folder. Explore them to get a visual overview of the application! 🚀✨

---

## 🏆 Badges
![Build Passing](https://img.shields.io/badge/Build-Passing-brightgreen)  
![Deployment](https://img.shields.io/badge/Deployed-Heroku-blue)  
![Maintained](https://img.shields.io/badge/Maintained-Yes-green)  

---

## 🙌 Acknowledgements
- I would like to express my sincere gratitude to my mentors, instructors, and peers for their invaluable guidance.  
- Special thanks to the Django and open-source developer community for their extensive documentation and support.

---

## 📚 Appendix
### **1. Key Dependencies**
```bash
pip install django djangorestframework djangorestframework-simplejwt psycopg2 mysqlclient
```

### **2. Troubleshooting**
🔹 **Database Connection Error**: Ensure the correct database credentials in `settings.py`.  
🔹 **Authentication Issues**: Verify JWT token generation and expiration policies.  
🔹 **Static Files Not Loading**: Run `python manage.py collectstatic`.  

---

💡 *For any issues, feel free to raise an issue in the GitHub repository!* 🚀
