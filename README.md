# 📶 Wi-Fi Attendance App

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Backend: Django](https://img.shields.io/badge/Backend-Django%204.1-blue.svg)
![Frontend: Android](https://img.shields.io/badge/Frontend-Android%20App-green.svg)
![API](https://img.shields.io/badge/API-RESTful-orange.svg)

---

## 📋 Project Overview

**Wi-Fi Attendance App** is a complete attendance tracking system built with a **Django REST API backend** and an **Android frontend**. It allows students or employees to mark attendance automatically when connected to authorized Wi-Fi networks.

The system is designed to reduce proxy attendance, ensure presence validation via Wi-Fi networks, and simplify record management.

---

## 🌐 Key Features

- 📶 Wi-Fi network check for trusted location authentication
- ✅ Attendance logging via mobile app when connected to valid Wi-Fi
- 🔐 Secure login via Django's authentication system
- 🗃️ Admin dashboard for attendance record management
- 🔌 API-based communication between Android app and Django backend
- 🧪 SQLite for backend data storage

---

## 🛠️ Tech Stack

| Layer     | Technology                     |
|-----------|--------------------------------|
| Frontend  | Android (Java/Kotlin)          |
| Backend   | Django 4.1, Django REST Framework |
| Database  | SQLite                         |
| DevOps    | Gradle for Android, pipenv/venv for Django |

---

## 📂 Project Structure

```

Wi-Fi-Attendance-App/
├── backend/
│   ├── attendance/                     # Django project root
│   │   ├── settings.py
│   │   ├── urls.py
│   │   ├── wsgi.py
│   │   └── asgi.py
│   ├── attendance\_app/                # Custom app for attendance
│   │   └── urls.py, models.py, views.py
│   └── manage.py
├── android\_app/
│   ├── app/src/...                    # Android frontend code (Java/Kotlin)
│   ├── build.gradle
│   ├── gradle.properties
│   └── settings.gradle

````

---

## ▶️ How to Run

### 🖥 Django Backend

1. **Navigate to project root**:
```bash
cd Wi-Fi-Attendance-App/backend
````

2. **Create virtual environment and install dependencies**:

```bash
python -m venv venv
source venv/bin/activate
pip install django djangorestframework
```

3. **Run server**:

```bash
python manage.py migrate
python manage.py runserver
```

Server will start at `http://127.0.0.1:8000/`

---

### 🤖 Android App

1. Open `android_app/` in **Android Studio**
2. Connect your phone or use an emulator
3. Build and run the app
4. Ensure both phone and backend are on the same network (for API communication)

---

## 📦 Features in Progress (Optional Enhancements)

* 📍 Add GPS fallback when Wi-Fi is unavailable
* 📈 Export attendance logs (CSV, PDF)
* 📲 Push notifications or alerts for missed attendance
* 👨‍🏫 Teacher-side interface to manage attendance manually

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙋‍♂️ Contact

Built with ❤️ by Hittanshu Bhanderi
Connect via [LinkedIn](https://www.linkedin.com/in/hittanshubhanderi/)

---
