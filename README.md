# GigHub API

> A RESTful API for managing freelance gigs, built with **FastAPI**.

This API powers a Nairobi‑based freelancing platform called **GigHub**. It allows clients to post gigs, freelancers to browse and search, and administrators to manage listings.  
The project was developed as part of **CIT 3107: Back‑End Development** and demonstrates CRUD operations, request validation, error handling, and interactive documentation.

---

## 🚀 Features

- **List all gigs** – with optional filtering by:
  - `category` (case‑insensitive)
  - `min_budget` / `max_budget`
- **View a specific gig** by its unique `id` (returns 404 if not found).
- **Search for gigs** by title (case‑insensitive, query parameter `q`).
- **Create a new gig** – auto‑generated `id`, default `status = "Open"`, and currency derived from your admission number.
- **Update a gig** – modify `budget` and/or `status` (`Open`, `In Progress`, `Closed`).
- **Delete a gig** – removes it from the in‑memory database (returns 404 if not found).
- **Swagger UI** interactive documentation (available at `/docs`).

---

## 🛠️ Technologies

- **Python 3.8+**
- **FastAPI** – web framework
- **Pydantic** – data validation (with custom validators)
- **Uvicorn** – ASGI server (development)

---

## 📁 Project Structure
