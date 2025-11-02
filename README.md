# ✈️ ALX Travel App

<p align="center">
  <img src="https://img.shields.io/badge/Django-4.2%2B-092E20?style=for-the-badge&logo=django&logoColor=white" alt="Django">
  <img src="https://img.shields.io/badge/DRF-FF6B6B?style=for-the-badge&logo=django&logoColor=white" alt="DRF">
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL">
  <img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black" alt="Swagger">
</p>

---

## 📜 Table of Contents
* [1. Project Overview](#1-project-overview)
* [2. Team Roles and Responsibilities](#2-team-roles-and-responsibilities)
* [3. Technology Stack Overview](#3-technology-stack-overview)
* [4. Database Design Overview](#4-database-design-overview)
* [5. Feature Breakdown](#5-feature-breakdown)
* [6. API Security Overview](#6-api-security-overview)
* [7. CI/CD Pipeline Overview](#7-cicd-pipeline-overview)
* [8. Resources](#8-resources)
* [9. License](#9-license)
* [10. Created By](#10-created-by)

---

## 1. Project Overview

**Brief Description:**  
The **ALX Travel App** is a **production-grade Django backend** powering a modern travel listing platform. This milestone delivers a **scalable, secure, and well-documented foundation** using MySQL, REST APIs, and automated Swagger documentation. Built with collaboration and future growth in mind, it follows **industry best practices** from day one.

**Project Goals:**
- Bootstrap a clean, modular Django project with `listings` app
- Secure configuration via `.env` and `django-environ`
- Enable CORS and generate interactive Swagger UI at `/swagger/`
- Prepare for async tasks with **Celery + RabbitMQ**

**Key Tech Stack:**  
`Python` `Django` `Django REST Framework` `MySQL` `Swagger (drf-yasg)`

---

## 2. Team Roles and Responsibilities

| Role                 | Key Responsibility |
|----------------------|--------------------|
| **Backend Developer** | Build models, serializers, views & API logic |
| **DevOps Engineer**   | Configure MySQL, CI/CD, Docker, and environments |
| **QA Engineer**       | Test endpoints, validate Swagger, ensure CORS compliance |
| **Technical Lead**    | Enforce architecture, review PRs, plan scalability |

---

## 3. Technology Stack Overview

| Technology               | Purpose in the Project |
|--------------------------|------------------------|
| **Django**               | Full-stack Python web framework |
| **Django REST Framework**| RESTful API development with serializers & viewsets |
| **MySQL**                | Reliable relational database for listings & bookings |
| **drf-yasg**             | Auto-generates Swagger/OpenAPI docs at `/swagger/` |
| **django-cors-headers**  | Secure frontend-backend communication |
| **django-environ**       | Load `.env` variables safely |
| **Celery + RabbitMQ**    | Async background tasks (future-ready) |

---

## 4. Database Design Overview

### Key Entities
- `Listing` – Travel destinations, hotels, tours  
- `User` – Extended Django auth (future)  
- `Review` – User ratings and feedback  
- `Booking` – Reservations (upcoming milestone)

### Relationships

```
User (1) → (Many) Listings
Listing (1) → (Many) Reviews
User (1) → (Many) Reviews & Bookings
```

---

## 5. Feature Breakdown

- **Modular Architecture** – Core logic in `listings/` app  
- **Secure Config** – `.env` + `django-environ` for secrets  
- **Interactive Docs** – Swagger UI at `/swagger/`  
- **CORS Enabled** – Ready for React/Vue/Angular frontends  
- **Git-Ready** – Clean repo with `.gitignore` and commit history

---

## 6. API Security Overview

| Measure                     | Why It Matters |
|----------------------------|----------------|
| **Environment Variables**  | No hard-coded secrets |
| **CORS Control**           | Blocks unauthorized origins |
| **DRF Validation**         | Prevents invalid/malicious data |
| **Swagger Restrictions**   | Hide docs in production |
| **Future JWT/Auth**        | Token-based access control |

---

## 7. CI/CD Pipeline Overview

> **Automate. Test. Deploy. Repeat.**

GitHub Actions runs on every push:
- Validate `requirements.txt`
- Lint with `flake8`
- Run unit tests
- Build Docker image (future)

**Tools:** GitHub Actions, Docker, MySQL

---

## 8. Resources

- [Django Docs](https://docs.djangoproject.com/)
- [DRF Guide](https://www.django-rest-framework.org/)
- [drf-yasg](https://github.com/axnsan12/drf-yasg)
- [MySQL + Django](https://docs.djangoproject.com/en/stable/ref/databases/#mysql-notes)
- [Best Practices](https://djangostars.com/blog/django-best-practices/)

---

## 9. License

MIT License

---

## 10. Created By

**Phinehas Macharia**  
[GitHub](https://github.com/MachariaP)
