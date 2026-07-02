# 📚 Learning Log — Django Web Application

> A full-stack Django web application that allows users to organize their learning journey by creating topics and recording personal notes for each topic. Built while following _Python Crash Course_ and extended with modern Django development practices.

![SQLite](https://img.shields.io/badge/Database-SQLite-blue)
![Bootstrap](https://img.shields.io/badge/Frontend-Bootstrap-purple)
![License](https://img.shields.io/badge/License-MIT-green)

---

# ✨ Features

- 👤 User registration and authentication
- 🔐 Secure login/logout functionality
- 📖 Create personalized learning topics
- 📝 Add multiple journal entries for each topic
- ✏️ Edit previously created entries
- 🔒 User-specific data isolation
- 📱 Responsive interface using Bootstrap
- ⚡ Lightweight SQLite backend
- 🏗 Clean Django project structure

---

---

## 📸 Application Preview

The project includes an interactive Django web application that enables users to create learning topics, record personal notes, and manage their learning journey through a clean and intuitive interface.

<p align="center">
  <img src="artifacts/Screenshot 2026-07-02 181713.png" alt="Learning Log Application" width="900"/>
</p>

<p align="center">
  <img src="artifacts/Screenshot 2026-07-02 181732.png" alt="Learning Log Application" width="900"/>
</p>

<p align="center">
  <img src="artifacts/Screenshot 2026-07-02 181727.png" alt="Learning Log Application" width="900"/>
</p>

---

# 🏗 Project Structure

```text
learning_log/
│
├── learning_logs/          # Main Django application
│   ├── migrations/
│   ├── templates/
│   ├── forms.py
│   ├── models.py
│   ├── urls.py
│   └── views.py
│
├── users/                  # Authentication app
│   ├── templates/
│   ├── urls.py
│   └── views.py
│
├── ll_project/             # Django project settings
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── static/
├── artifacts/              # Screenshots
├── db.sqlite3
├── manage.py
├── requirements.txt
└── README.md
```

---

# ⚙️ Technology Stack

| Layer          | Technology                                                |
| -------------- | --------------------------------------------------------- |
| Backend        | Django                                                    |
| Language       | Python                                                    |
| Database       | SQLite                                                    |
| Frontend       | HTML, CSS, Bootstrap                                      |
| Templates      | Django Template Language                                  |
| Authentication | Django Authentication System                              |
| Deployment     | Django Development Server (or Render/Railway if deployed) |

---

# 🗄 Database Design

The application uses three primary models:

### User

Stores registered user accounts.

### Topic

Represents a learning subject created by a user.

Example:

- Python
- Machine Learning
- Django
- Data Science

Each topic belongs to exactly one authenticated user.

### Entry

Stores notes associated with a topic.

Each topic can contain multiple entries, allowing users to build a chronological learning journal.

---

# 🚀 Getting Started

## 1. Clone the repository

```bash
git clone https://github.com/yourusername/learning-log.git

cd learning-log
```

---

## 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it

Windows

```bash
venv\Scripts\activate
```

Linux/macOS

```bash
source venv/bin/activate
```

---

## 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 4. Apply migrations

```bash
python manage.py migrate
```

---

## 5. Create an administrator account

```bash
python manage.py createsuperuser
```

---

## 6. Run the development server

```bash
python manage.py runserver
```

Open

```
http://127.0.0.1:8000/
```

---

# 🔐 Authentication

The application uses Django's built-in authentication framework.

Users can

- Register
- Log in
- Log out
- Create private topics
- Manage only their own entries

Unauthorized users cannot access or modify another user's data.

---

# 📈 Learning Objectives

This project demonstrates practical experience with:

- Django project architecture
- URL routing
- Models and migrations
- ORM relationships
- Forms and validation
- Class-based and function-based views
- Template inheritance
- User authentication
- CRUD operations
- Static files
- Database migrations
- MVC/MVT design principles

---

# 💡 Future Improvements

- Rich text editor for notes
- Search functionality
- Tags and categories
- Markdown support
- REST API using Django REST Framework
- PostgreSQL support
- Docker containerization
- Cloud deployment (Render/AWS)
- Dark mode
- Profile management

---

# 📄 License

This project is released under the MIT License.

---

# 🙏 Acknowledgements

- Eric Matthes for the excellent learning resource _Python Crash Course_.
- The Django Software Foundation for maintaining the Django framework.

---
