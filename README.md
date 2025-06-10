# Kanban Board with JWT Authentication

## Overview

This project is a Kanban board application that includes secure user authentication using JSON Web Tokens (JWT). The application features:

- A login page for user authentication.
- Secure API endpoints that require a valid JWT for access.
- A Kanban board displaying tasks sorted into three columns: To Do, In Progress, and Done.
- Client-side JWT storage in `localStorage` for secure and persistent authentication.

This project was completed as part of a full-stack challenge to demonstrate skills in authentication, Express APIs, and full-stack deployment.

---

## Challenge User Story

**As a member of an agile team,**  
I want a Kanban board with a secure login page  
**so that** I can securely access and manage my work tasks.

---

## Acceptance Criteria

✅ The login page provides form inputs for username and password.  
✅ Users with valid credentials receive a JWT and are redirected to the main Kanban board.  
✅ Invalid login attempts display an error message.  
✅ On successful login, the JWT is stored in `localStorage`.  
✅ Logging out removes the JWT from `localStorage` and redirects to the login page.  
✅ API requests to protected routes require a valid JWT.  
✅ Inactive users will have their JWT expire and must log in again.  

---

## Technologies Used

- **Frontend:** React, TypeScript, Vite
- **Backend:** Express, Node.js, Sequelize ORM, PostgreSQL
- **Authentication:** JSON Web Tokens (JWT), bcrypt for password hashing
- **Deployment:** Render (for both server and client)

---

## Project Setup

### Prerequisites

- Node.js (v22+)
- PostgreSQL database
- Environment variables configured in a `.env` file.

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/jcalderaro-96/UCI-Module-14-KanbanBoard
   cd UCI-Module-14-KanbanBoard

2. **Install dependencies for the server and client:**
cd server && npm install
cd ../client && npm install

3. **Configure environment variables:**
Create a .env file in the server directory with:
- DB_NAME='kanban_db'
- DB_USER='your_db_username'
- DB_PASSWORD='your_db_password'
- JWT_SECRET_KEY='supersecretjwtkey123!'

4. **Run the application locally:**
- npm start

## Deployment Status
⚠️ Note: While the application was deployed to Render, there was a database connection issue (ECONNREFUSED) that prevented the app from running correctly in the deployed environment.
- The server and client apps were successfully built and uploaded to Render.
- The PostgreSQL database was not connecting properly in Render.
- Locally, the application runs as expected with JWT authentication and client-side token storage.

## Screenshots
- Login Page
- Kanban Board

## Grading Rubric Self-Assessment
Technical Acceptance Criteria:
- Fully implemented in local environment, including authentication and token validation.

Deployment:
- Application was deployed to Render, but deployment is not functional due to database connection issues.

Application Quality:
- Clean, user-friendly interface with intuitive layout and polished styles.

Repository Quality:
- Clear file structure and naming conventions.

Quality commit messages.
- This README includes screenshots, description, and project details.

## Future Work / Bonus Features
🔲 Add sorting and filtering functionality for Kanban tickets to earn the bonus points.

## License
This project is licensed under the MIT License.

## Contact
For any questions or feedback please reach me here locally.

## Live Application (Non-functional due to database error)
🔗 Render Deployment
(Deployment exists but does not function due to database connection error.)

## Acknowledgement
This project was created by Me (JCalderaro). Assistance was provided by OpenAI’s ChatGPT, a language model that helped with debugging advice, deployment explanations, and README documentation editing.
