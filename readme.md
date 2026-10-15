# Overview

As a software engineer, my goal is to deepen my practical knowledge of full-stack web architectures, RESTful API design, and component-based frontend development using JavaScript. I developed this project to explore how a lightweight Node.js/Express backend integrates seamlessly with a reactive Vue.js client while maintaining a secure, clean separation of concerns.

The **Vue Events Bulletin Board** is a responsive single-page web application designed for publishing and managing community event announcements. It provides real-time event creation, browsing, and deletion with instant UI updates, powered by an Express REST API backend and a reactive Vue.js interface.

The primary purpose was to demonstrate core full-stack JavaScript principles:
- **RESTful API Architecture:** Implementing clean HTTP endpoints (`GET`, `POST`, `DELETE` on `/api/events`) with Express routing and JSON payloads.
- **Reactive Frontend State:** Utilizing Vue.js two-way data binding (`v-model`), dynamic DOM rendering (`v-for`), and asynchronous client-server communication.
- **Separation of Concerns:** Structuring the application cleanly into public assets (`/public`), view templates (`/views`), and modular backend controllers (`/backend`).
- **Containerization:** Packaging the entire runtime and dependencies into a lightweight Docker container for portable and consistent deployment.

[Software Demo Video](https://youtu.be/_CnbBcZKfvg)


# Development Environment

- **IDE / Editor:** Visual Studio Code
- **Runtime & Package Manager:** Node.js (LTS) & npm
- **Containerization Platform:** Docker
- **Version Control:** Git & GitHub

The project is developed using **Full-Stack JavaScript (Node.js & Client-side JS)**.

Key libraries and frameworks utilized include:
- **`express`**: Lightweight web framework for server routing, middleware pipeline, and RESTful API endpoints.
- **`vue`**: Progressive JavaScript framework powering the reactive single-page interface with two-way data binding.
- **`vue-resource`**: HTTP request library enabling asynchronous communication between Vue and the Express REST API.
- **`ejs`**: Embedded JavaScript template engine configured to serve static and rendered HTML pages.
- **`body-parser` & `method-override`**: Express middleware for parsing incoming JSON / URL-encoded bodies and handling RESTful request methods.
- **`morgan`**: HTTP request logger middleware for runtime monitoring and debugging.
- **`bootstrap`**: CSS framework providing a responsive grid layout and structured UI components.

# Useful Websites

- [Node.js Official Documentation](https://nodejs.org/en/docs/) - Core API reference for the Node.js runtime environment and module architecture.
- [Express.js Guide & Routing](https://expressjs.com/en/guide/routing.html) - Documentation on Express routing, static asset serving, and middleware integration.
- [Vue.js v1 Guide](https://v1.vuejs.org/guide/) - Documentation on reactive data binding, directives (`v-model`, `v-for`), and component lifecycles.
- [Docker Getting Started Guide](https://docs.docker.com/get-started/) - Reference guide for containerizing Node.js applications with multi-layer Dockerfiles.
- [MDN Web Docs - Express & REST APIs](https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Server-side/Express_Nodejs) - In-depth tutorials on designing and consuming RESTful web services.

# Future Work

- **Persistent Database Integration:** Replace the current in-memory events array (`events.js`) with a persistent database (e.g., PostgreSQL with Prisma or MongoDB) to guarantee data persistence across server restarts.
- **Migration to Modern Vue (Vue 3 + Vite):** Modernize the client application from legacy Vue 1.x and Vue-Resource to Vue 3 (Composition API) with Vite and Axios for enhanced performance and build optimization.
- **User Authentication & Authorization:** Implement JWT (JSON Web Tokens) or OAuth-based authentication to secure endpoints and restrict event editing/deletion to authorized owners.
- **Payload Validation & Error Handling:** Add a schema validation layer (e.g., Zod or Joi) on the backend to validate event titles, date strings, and details with descriptive client-facing error responses.