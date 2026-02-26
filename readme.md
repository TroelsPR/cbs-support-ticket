# CBS Support Ticket System

A vertical prototype for managing IT support tickets within the IT department at Copenhagen Business School (CBS). This project was developed as part of a university course to demonstrate end-to-end handling of support cases and to serve as a foundation for future iteration.

---

## Business Problem

CBS staff and students need a single place to submit, view, and track IT support requests. Without a structured system, requests can be lost in email, lack clear ownership, and make it difficult for the IT team to prioritize and assign work. This prototype addresses that by providing:

- **Ticket creation** — Users can submit support cases with title, description, category, and assignment.
- **Ticket listing** — All support tickets are visible in one view with key metadata (status, creator, assignee, affected user, category).
- **User context** — The system models three user types (IT employees, academics, students) so tickets can be created by and assigned to the right roles.

The scope is deliberately limited to core create-and-list flows to validate the concept and architecture before expanding (e.g. search, status updates, authentication).

---

## Tech Stack

- **Runtime:** Node.js  
- **Backend:** Express.js  
- **Database:** SQLite3  
- **Frontend:** Vanilla HTML, CSS, and JavaScript (no framework)  
- **API:** REST (JSON) for support tickets and user data  

---

## How to Run

**Prerequisites:** Node.js (v14 or later recommended) and npm.

1. Clone the repository and open the project directory.
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the server:
   ```bash
   npm start
   ```
4. Open a browser and go to [http://localhost:3000](http://localhost:3000).

The server runs on `localhost:3000` by default. The first run creates a local SQLite database (`db.sqlite`) and seeds it with sample tickets and users.

---

## Project Structure

| Path | Purpose |
|------|---------|
| `src/server.js` | Express app setup, route mounting, server start |
| `src/routes/` | Client-facing routes (e.g. serve `index.html`) |
| `src/api/` | REST API routes for support tickets and users |
| `src/lib/database/` | SQLite initialization and data access helpers |
| `src/public/` | Static assets: HTML, CSS, JS, images |

---

## Contributors

- [Amanda Frithjof Bonde](https://www.linkedin.com/in/amandabonde)
- [Thøger Elung-Jensen](https://www.linkedin.com/in/th%C3%B8ger-elung-jensen-b687b9249)
- [Troels Philip Rohde](https://www.linkedin.com/in/troelsprohde/)
- [Gustav Christian Søgård](https://www.linkedin.com/in/gustavsogard/)

---

*This is a university project developed for educational purposes. It is a working vertical prototype rather than a production-ready system.*
