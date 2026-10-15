<div align="center">

# DevMatch
### Great ideas need the right team.

[![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)](https://fastapi.tiangolo.com/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Python 3.10+](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Status](https://img.shields.io/badge/Status-Live-success?style=for-the-badge)](https://syncbuild.tech)

**DevMatch** is a skill-based team-matching platform built for BIT Sindri. It bridges the gap between campus builders by dynamically scoring compatibility between student skill sets and open project roles across branches and batches.

[🌐 Live Deployment](https://devmatch-f1it.onrender.com/) · [📑 API Docs](https://syncbuild.tech/docs) · [🐞 Report Bug](https://github.com/balmukundpandey407/DevMatch/issues)

</div>

---

## Why DevMatch?

* **Skill-Based Matching Engine:** Computes dynamic match scores, highlighting shared tech stacks and ideal role fits.
* **Role-First Recruitment:** Project leads get ranked student recommendations tailored to each open position.
* **Smart Discovery & Filtering:** Search and filter active projects across branches by tags, domain, and availability.
* **Interdisciplinary Collaboration:** Seamlessly connect developers, designers, and domain leads across departments.
* **Interactive API Documentation:** Native Swagger UI interactive documentation to test and inspect endpoints.

---

## System Architecture & Tech Stack

```
┌─────────────────┐       JSON / REST       ┌──────────────────────┐
│  Client UI      │ ◄─────────────────────► │  FastAPI Backend     │
│  (Vanilla JS)   │                         │  (Asynchronous Core) │
└─────────────────┘                         └──────────┬───────────┘
                                                       │
                                              Async Engine / ORM
                                                       │
                                            ┌──────────▼───────────┐
                                            │ Neon PostgreSQL DB   │
                                            │ (Relational Schemas) │
                                            └──────────────────────┘
```

* **Core Engine & APIs:** Python, FastAPI (Asynchronous routes, Pydantic data validation)
* **Database & Storage:** PostgreSQL (Hosted on NeonDB with normalized relational schemas)
* **API Documentation:** Swagger UI & ReDoc (`/docs` & `/redoc`)
* **Deployment:** Production server hosted at `syncbuild.tech`

---

## Quick Start (Local Setup)

### 1. Clone the Repository
```bash
git clone [https://github.com/balmukundpandey407/DevMatch.git](https://github.com/balmukundpandey407/DevMatch.git)
cd DevMatch
```

### 2. Configure Environment Variables
Create a `.env` file in the root directory:
```bash
DATABASE_URL=postgresql://USER:PASSWORD@HOST:5432/DATABASE
SECRET_KEY=your_secure_random_secret_key
```

### 3. Install Dependencies & Run
```bash
pip install -r requirements.txt
uvicorn app.main:app --reload
```

* **Local Application:** `http://127.0.0.1:8000`
* **Interactive API Docs:** `http://127.0.0.1:8000/docs`

---

## 👥 Team SYNCTHINK

Built during **Hacktoberfest Hack Day (BIT Sindri)**:

* **Balmukund Pandey** — *Backend Architecture, Database Schemas & REST APIs*
* **Pranjal Aman** — *Frontend UI & Client-Side Integration*

---

## Author
   
   BALMUKUND PANDEY
