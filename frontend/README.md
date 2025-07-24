# 🐾 Pet Shelter API — Learning Swagger, REST, and Full Stack Integration

This project is a **learning-focused Node.js + Express API** designed to explore and practice:
- RESTful API principles
- Layered backend architecture
- Swagger/OpenAPI documentation
- Testing with Supertest + Jest
- Front-end integration with React (using both Fetch and Axios)

It simulates a **pet shelter registry** where users can create, read, update, and delete (CRUD) pet entries — and view them through a React-based interface.

---

## 📘 What is REST?

**REST** (Representational State Transfer) is an architectural style for designing APIs that are:

- **Stateless:** Each request contains all the information needed to process it.
- **Resource-based:** Access to resources via standard HTTP methods (GET, POST, PUT, DELETE).
- **Uniform interface:** Easy for clients to interact with standardized endpoints.
- **Cacheable:** Can cache responses for improved performance.
- **Layered:** Supports proxies/gateways for scalability and abstraction.

> REST is ideal for scalable, simple, and flexible applications across web, mobile, microservices, and IoT platforms.

---

## 🧱 Project Architecture

The app follows a **layered architecture**:

📦 root
┣ 📂 db/ ← Mock DB (in-memory JSON)
┣ 📂 pets/
┃ ┣ 📂 routes/ ← Route definitions with Swagger annotations
┃ ┣ 📂 controllers/ ← Business logic for each endpoint
┃ ┗ 📂 models/ ← Interactions with the mock DB
┣ 📂 public/ ← React app front end (via Vite)
┣ 📜 app.js ← Entry point + Swagger config
┗ 📜 README.md


---

## 🔬 Features

- 📦 Express API with full CRUD operations for pets
- 🔍 Swagger docs available at `/api-docs`
- ✅ Tested with Supertest and Jest
- ⚛️ React front end with Axios and Fetch integration
- 🌐 RESTful design using layered architecture

---

## 🚀 How to Run

- 🧪 **Run the API locally:**

  ```
  bash
  npm install
  npm run dev     # or nodemon app.js
  ```

Access the API at: http://localhost:3000/pets

Access Swagger UI at: http://localhost:3000/api-docs

    Run as a full website (React front end + API):

        Start the Express API (npm run dev) in one terminal.

        In another terminal, navigate to your React app root:

        ```
        npm install
        npm run dev
        ```

    The website will run at: http://localhost:5173 and interact with the API running on port 3000.

🧪 How to Test

To run the test suite using Jest + Supertest:

```npm run test```

The test suite covers all CRUD endpoints: listing pets, retrieving by ID, editing, adding, and deleting.
📖 Learnings

This project teaches how to:

     Structure and layer an Express API

    Use Swagger to auto-document endpoints

    Integrate automated API testing

    Build and connect a front end in React

    Understand the lifecycle of full-stack development

📚 Credits

Built as part of a personal Swagger and REST API learning initiative. Inspired by best practices in full-stack architecture.