
---

## 🎯 **Objective**

Design and implement a **Movie Explorer Platform** for film enthusiasts to browse and explore information about **movies**, **actors**, **directors**, and **genres**. This is a **read-only** application with no user authentication or authorization required.

---

## 🧠 **Core Functional Overview**

The application should enable users to:

* Browse a list of movies with relevant metadata.
* Filter movies by **genre**, **director**, **release year**, and **actors**.
* View detailed movie pages with cast, genres, and director.
* View actor/director profiles showing their associated movies.

---

## 🖥️ **Backend Requirements**

* **Language**: Python
* **Framework**: Use FastAPI
* **Database**: SQLite Localhost
* **API Documentation**: Must use **Swagger UI** and comply with **OpenAPI Specification**.

### 🔧 **API Design & Entities**

Design the following core entities and expose RESTful API endpoints for:

1. **Movies**
2. **Actors**
3. **Directors**
4. **Genres**

### 🔗 **Entity Relationships**

* A **movie**:

  * Belongs to **one or more genres**
  * Has **one director**
  * Has **multiple actors**
* An **actor** can be associated with **multiple movies**.
* A **director** can direct **multiple movies**.
* A **genre** can include **multiple movies**.

### 🔍 **Filtering Support**

Implement backend filtering endpoints for:

* **Movies** filtered by:

  * Genre
  * Director
  * Release year
  * Actor

* **Actors** filtered by:

  * Movie
  * Genre (based on the movies they’ve acted in)

> ⚠️ All filtering **must** be done server-side (do not rely on frontend filtering).

---

## 💻 **Frontend Requirements**

* **Framework**: Use VueJS
* **Bundler**: Prefer **Vite** for project scaffolding and builds
* **Language**: TypeScript recommended (JavaScript acceptable)
* **Styling**: Use Tailwind CSS

### 👁️ **UI Features**

Implement the following views/pages:

1. **Movie List Page**

   * Show list of movies with title, release year, genres, and director.
   * Filtering/search controls by genre, actor, or director.

2. **Movie Detail Page**

   * Show detailed info: full cast list, genres, director, and release year.

3. **Actor Profile Page**

   * Show actor bio and list of movies acted in.

4. **Director Profile Page**

   * Show director bio and list of directed movies.

---

## 📦 **Project Structure & Tooling**

* The project must be **Dockerized**:

  * Include Dockerfiles for both frontend and backend.
  * Provide Docker Compose (or clear scripts) to build and run the project.

* **README.md**:

  * Include clear setup, run, and testing instructions.
  * Include API documentation URL or location.

* **Testing**:

  * Include **unit tests** for both frontend and backend.
  * Integrate tests into the build pipeline.

* **Linting**:

  * Add linting as part of build step (ESLint, Flake8, etc.).

* **Code Style**:

  * Write modular, clean, and well-documented code.
  * Add inline documentation where logic is non-trivial.

---

## ✅ **Functional & UX Expectations**

* A fully working **full-stack** app that runs locally with simple commands.
* Responsive and user-friendly UI.
* Proper handling and UX for:

  * No results (e.g., "No movies found").
  * Invalid filters or data fetch errors.

---

## 📤 **Submission Instructions**

* Push the **complete project** to a **public GitHub repository**.
* Ensure the README is clear enough for evaluators to:

  * Clone the project.
  * Install dependencies.
  * Run the app (with or without Docker).
  * Run tests.

---
