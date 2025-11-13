# 🏠 Adult Home Management System

## 📘 Overview
The **Adult Home Management System** is a Django-based web application designed to streamline daily operations in Adult Family Homes.  
It digitizes records, tracks inventory, manages staff schedules and payroll, and sends timely medication refill reminders — helping caregivers and administrators save time, improve accuracy, and enhance resident care.

---

## 🚩 Problem Statement
Many Adult Family Homes still rely on **manual systems** such as physical calendars, handwritten records, and phone-based communication for medication refills and schedules.  
This leads to:
- Missed medication doses due to late refill orders  
- Tedious recordkeeping (Medical Administration Records, vital signs, incidents, etc.)  
- Repetitive payroll tracking and calculations  
- Risk of data loss when physical documents are misplaced  

---

## 💡 Proposed Solution
The Adult Home Management System provides a **centralized digital platform** to handle:
1. **Digital Recordkeeping:**  
   Store and manage Medical Administration Records (MARs), vital signs, incident reports, and daily narratives.
2. **Medication Refill Reminders:**  
   Automatically alert caregivers when medicine inventory is running low.
3. **System Calendar:**  
   Maintain digital scheduling for meetings and activities with visibility for past, present, and future events.
4. **Inventory Management:**  
   Track supplies, auto-generate shopping lists, and notify employers when stock is low.
5. **Payroll Automation:**  
   Automatically calculate salaries based on workdays logged by employees.

---

## ⚙️ Features
| Category | Description |
|-----------|-------------|
| 🧾 Recordkeeping | Digitize and access all medical and incident records easily |
| 💊 Medication Reminders | Get alerts before medications run out |
| 🗓️ Calendar System | Schedule and view all meetings and events |
| 📦 Inventory | Manage resident and home inventory levels |
| 👷 Staff Management | Record staff attendance and automate payroll |
| 🔐 Authentication | Secure role-based access (Admin, Caregiver, Employer) |

---

## 🧠 System Architecture
**Framework:** Django (Python)  
**Database:** SQLite (for prototype) / PostgreSQL (for production)  
**Frontend:** HTML, CSS, Bootstrap / Tailwind CSS  
**Hosting (Deployment):** Render / Railway / PythonAnywhere  

### 🏗️ Django Apps
| App | Purpose |
|------|----------|
| `residents` | Manage resident info, medical records, and incidents |
| `staff` | Manage staff profiles, work logs, and payroll |
| `inventory` | Track medicines and home supplies |
| `events` | Handle scheduling, reminders, and activity tracking |

---

## 🧩 Project Structure
adult_home_mgmt/
│
├── adult_home_mgmt/ # Project configuration files
├── residents/ # Resident management (records, incidents)
├── staff/ # Employee management & payroll
├── inventory/ # Medicine & supply tracking
├── events/ # Calendar and scheduling
│
├── templates/ # Shared templates
├── static/ # CSS, JS, images
├── db.sqlite3 # Local development database
└── manage.py # Django management script

---

## 🚀 Getting Started

### 1️⃣ Clone the repository
```bash
git clone https://github.com/Emmanuel-K0ech/adult-home-mgmt.git
cd adult-home-mgmt

2. Create and activate virtual environment
python3 -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

3. Install Dependancies
pip install -r requirements.txt

4. Run migrations
python manage.py makemigrations
python manage.py migrate

5. Start Development server
python manage.py runserver

visit Visit http://127.0.0.1:8000 in your browser 🚀

🧩 Example Features to Test

Add Resident: Enter name, room number, and medical info.

Log Vital Signs: Record daily vitals.

Add Event: Schedule staff meetings or medication reminders.

Inventory Alert: See low-stock medicine notifications.

Payroll Summary: Check computed salary from workdays × rate.

🔒 Security Considerations

Role-based access for Admin, Caregiver, and Employer

Encrypted user passwords (Django auth system)

Future upgrades: SSL, user activity logs, and audit trails

🧰 Future Enhancements

Integration with Django REST Framework for mobile access

Real-time notifications via WebSockets

PDF/CSV export for reports (MARs, payroll, incidents)

Email or SMS reminders for medication and events

Cloud storage for resident photos and files

📈 Benefits

✅ Reliable digital records accessible anytime
✅ Increased task efficiency
✅ Reduced paperwork and manual errors
✅ Improved data security and accountability

🚧 Challenges & Solutions
Challenge	Proposed Solution
Transition from paper to system	Staff training sessions
Data security & privacy	Implement Django authentication and encrypted storage
Learning curve for staff	Simple, intuitive UI design
🧩 Development Roadmap

 Week 1: Project setup and base templates

 Week 2: Models, Admin, CRUD operations

 Week 3: Core functionality (records, reminders, events)

 Week 4: Authentication & Payroll

 Week 5: UI polish, testing, and deployment

💻 Tech Stack

Backend: Django (Python)
Frontend: HTML5, CSS3, Bootstrap
Database: SQLite / PostgreSQL
Version Control: Git & GitHub
Deployment: Render / Railway

🧑‍💻 Author

Emmanuel Kipchumba Koech
Computer Science Graduate | ALX Software Engineer | Cybersecurity Enthusiast
🔗 GitHub Profile

📜 License

This project is licensed under the MIT License
.

🙌 Acknowledgments

Django Documentation

Corey Schafer’s Django Tutorials

Traversy Media Django Crash Course
