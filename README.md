# 🎥 iStream Platform

> A full-stack YouTube-inspired video streaming platform built with **Python** and **Django**, featuring secure authentication, video uploads, adaptive streaming, likes/dislikes, and cloud media optimization powered by ImageKit.

![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python)
![Django](https://img.shields.io/badge/Django-6.0-darkgreen?logo=django)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-In%20Development-orange)

---

## 📖 Project Overview

iStream Platform is a modern video-sharing application inspired by YouTube. The project demonstrates how to build a scalable media platform using Django while integrating cloud-based media storage and optimization through ImageKit.

This project emphasizes clean architecture, authentication, media management, responsive UI, and production-ready backend development practices.

---

## ✨ Features

### Authentication

- User Registration
- Secure Login & Logout
- Session-based Authentication
- Password Validation
- Protected Routes

### Video Management

- Upload Videos
- Video Metadata Management
- Automatic Thumbnail Generation
- Video Optimization
- Adaptive Video Streaming
- Cloud Media Storage

### Engagement

- Like Videos
- Dislike Videos
- View Counter
- Video Detail Pages

### User Experience

- Responsive Interface
- Modern UI Components
- Reusable Templates
- Static Asset Management

---

## 🛠 Tech Stack

### Backend

- Python 3.13
- Django 6
- SQLite (Development)

### Cloud Services

- ImageKit.io
    - Video Uploads
    - Thumbnail Generation
    - Video Optimization
    - Streaming URLs
    - Watermarked Images

### Frontend

- HTML5
- CSS3
- Django Templates

### Package Management

- uv
- pyproject.toml

---

## 📁 Project Structure

```text
iStream-Platform/
│
├── youtube_/
│   ├── config/
│   │   ├── settings.py
│   │   ├── urls.py
│   │   ├── asgi.py
│   │   └── wsgi.py
│   │
│   ├── accounts/
│   │   ├── models.py
│   │   ├── views.py
│   │   ├── forms.py
│   │   ├── urls.py
│   │   └── templates/
│   │
│   ├── videos/
│   │   ├── models.py
│   │   ├── views.py
│   │   ├── urls.py
│   │   ├── imagekit_client.py
│   │   └── templates/
│   │
│   ├── static/
│   ├── templates/
│   ├── manage.py
│   └── db.sqlite3
│
├── pyproject.toml
├── uv.lock
└── README.md
```

---

## ⚙️ Installation

### Clone the repository

```bash
git clone https://github.com/Ayyah-Coded/iStream-Platform.git
```

```bash
cd youtube_
```

---

### Install dependencies

```bash
uv sync
```

---

### Activate the virtual environment

Windows

```bash
.venv\Scripts\activate
```

Linux / macOS

```bash
source .venv/bin/activate
```

---

### Configure Environment Variables

Create a `.env` file inside the project root.

```env
IMAGEKIT_PRIVATE_KEY=your_private_key

IMAGEKIT_PUBLIC_KEY=your_public_key

IMAGEKIT_URL_ENDPOINT=https://ik.imagekit.io/your_id
```

---

### Apply database migrations

```bash
uv run manage.py migrate
```

---

### Create an admin user

```bash
uv run manage.py createsuperuser
```

---

### Run the development server

```bash
uv run manage.py runserver
```

Open

```
http://127.0.0.1:8000
```

---

## 🗄 Database Design

### User

Stores authentication information using Django's built-in User model.

### Video

Stores

- title
- description
- owner
- video URL
- thumbnail URL
- likes
- dislikes
- views
- timestamps

### VideoLike

Stores user reactions.

Supports

- Like
- Dislike

Prevents duplicate reactions from the same user.

---

## ☁️ ImageKit Integration

The application integrates with ImageKit for:

- Video Uploads
- CDN Delivery
- Adaptive Streaming
- Thumbnail Generation
- Watermarking
- Optimized Media URLs

---

## 🔒 Authentication Flow

```
Register
      │
      ▼
Login
      │
      ▼
Authenticated Session
      │
      ├──────────────┐
      ▼              ▼
Upload Video     Like Videos
      │              │
      ▼              ▼
Logout
```

---

## 🚀 Future Improvements

- Comments
- Subscriptions
- Playlists
- Watch History
- Notifications
- Search Engine
- Video Categories
- Recommendations
- Live Streaming
- REST API
- Docker Support
- PostgreSQL
- Redis Caching
- Celery Background Tasks
- AWS Deployment

---

## 📸 Screenshots

Coming Soon

---

## 🧪 Testing

Run the test suite

```bash
uv run manage.py test
```

---

## 📈 Learning Objectives

This project demonstrates proficiency in:

- Django Framework
- Authentication Systems
- ORM & Database Design
- Cloud Media Services
- Backend Architecture
- MVC Design Pattern
- CRUD Operations
- Static & Media Management
- Session Management
- Production-ready Project Structure

---

## 🤝 Contributing

Contributions are welcome.

1. Fork the repository

2. Create a feature branch

```bash
git checkout -b feature/new-feature
```

3. Commit changes

```bash
git commit -m "Add new feature"
```

4. Push

```bash
git push origin feature/new-feature
```

5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Yahaya Hayatullahi**

Backend & Full-Stack Software Developer

- Python
- Django
- Node.js
- TypeScript
- PostgreSQL
- Docker
- Kubernetes
- AWS

---

⭐ If you found this project useful, consider giving it a star.
