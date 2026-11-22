# Students & Doctors Records API

A REST API for managing student and doctor records, built as a team project to practice back-end fundamentals: routing, CRUD operations and testing endpoints with Postman.

## Tech stack
- Node.js + Express 5
- MongoDB with Mongoose (local instance)
- Postman for endpoint testing

## Endpoints
| Method | Endpoint | Description |
| --- | --- | --- |
| GET | `/students` | List all students |
| GET | `/all` | List all students and doctors |
| POST | `/add-doctor` | Add a doctor (name, age, phone via query params) |
| POST | `/add-student-hardcoded` | Add a sample student (seed data) |
| POST | `/add-Doctor-hardcoded` | Add a sample doctor (seed data) |
| PATCH | `/updateDoctor?oldname=&newname=` | Rename a doctor |
| DELETE | `/students/:name` | Delete a student by name |

## Setup
1. Install [Node.js](https://nodejs.org) and a local [MongoDB](https://www.mongodb.com/try/download/community) instance.
2. Clone the repo and install dependencies:
   ```
   npm install
   ```
3. Make sure MongoDB is running locally (the app connects to `mongodb://localhost:27017/TASK`).
4. Start the server:
   ```
   node server.js
   ```
5. The API listens on `http://localhost:3000`. Test the endpoints with Postman.

## Team
Built with my faculty teammates: routing and CRUD split across the team, my parts were the students listing and the combined records endpoint, plus end-to-end Postman testing.
