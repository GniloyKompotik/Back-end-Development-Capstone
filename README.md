# 3. Back-end-Development-Capstone

**Repository URL format to submit:**
`[https://github.com/c85/Back-end-Development-Capstone/blob/main/README.md](https://github.com/c85/Back-end-Development-Capstone/blob/main/README.md)`

### `README.md` Content:

```markdown
# IBM Back-End Development Capstone Application

[![Django](https://img.shields.io/badge/Django-4.2+-092E20.svg)](https://www.djangoproject.com/)
[![Docker](https://img.shields.io/badge/Docker-Enabled-2496ED.svg)](https://www.docker.com/)
[![Kubernetes](https://img.shields.io/badge/Kubernetes-Deployed-326CE5.svg)](https://kubernetes.io/)
[![Python](https://img.shields.io/badge/Python-3.9-blue.svg)](https://www.python.org/)

This repository contains the primary web application for the **IBM Back-End Development Capstone Project**. The project integrates multiple backend microservices into a unified Django web application representing the official website for the band **Djirection**.

---

## 🏗 Architecture Overview

The application utilizes a modern microservices architecture:
- **Django Main App:** Serves dynamic web pages (Band Overview, Songs, Pictures, Concerts) and communicates with microservices.
- **Pictures Microservice:** Manages photo media records, deployed on IBM Cloud Engine.
- **Songs Microservice:** Manages track catalogs, connected to MongoDB and deployed on Red Hat OpenShift.
- **Container Orchestration:** Fully containerized with Docker and deployed via Kubernetes (`kubectl`).

---

## 🌟 Pages & Features

- **Home Page (`/`):** Detailed overview of Djirection, highlighting band members and key career achievements.
- **Songs Catalog (`/songs`):** Interactive interface listing band tracks with detailed modal popups.
- **Picture Gallery (`/photos`):** Visual gallery featuring photo cards loaded dynamically.
- **Concerts Page (`/concerts`):** Upcoming tour dates and location schedules.
- **Admin Dashboard (`/admin`):** Full authentication and Django administrative portal.

---

## 🛠 Database & Migrations

To apply database migrations locally or in production:

```bash
python manage.py makemigrations
python manage.py migrate