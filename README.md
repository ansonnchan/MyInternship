# MyInternship

MyInternship is a full-stack web app that helps students track internship applications in one place, manage status changes, and stay organized during recruiting.

## Live Deployment
- Frontend (Vercel): [https://internship-tracker-frontend-nu.vercel.app](https://internship-tracker-frontend-nu.vercel.app) 👈 Click here to try the app
- Backend (Render): [https://internship-tracker-xo8m.onrender.com](https://internship-tracker-xo8m.onrender.com)
- API Health: [https://internship-tracker-xo8m.onrender.com/api/health](https://internship-tracker-xo8m.onrender.com/api/health)

## Product Preview 

### Signup Page
<img src="./screenshots/signup.png" alt="Signup Page" width="500" />

### Login Page
<img src="./screenshots/login.png" alt="Login Page" width="500" />

### Dashboard (no applications)
<img src="./screenshots/dashboard-empty.png" alt="Signup Page" width="500" />

### Create Application
<img src="./screenshots/new-application.png" alt="Signup Page" width="500" />

### Dashboard (with applications)
<img src="./screenshots/dashboard-full.png" alt="Signup Page" width="500" />

### Email Classification
<img src="./screenshots/email classifier.png" alt="Signup Page" width="500" />
<img src="./screenshots/classifier-result.png" alt="Signup Page" width="500" />


## Project Structure
- Link to backend source code: [https://github.com/ansonnchan/internship-tracker-backend](https://github.com/ansonnchan/internship-tracker-backend)
- Link to frontend source code: [https://github.com/ansonnchan/internship-tracker-frontend](https://github.com/ansonnchan/internship-tracker-frontend)
  
## Tech Stack
### Backend
- Java
- Spring Boot
- Spring Security + JWT
- RESTful API
- PostgreSQL

### Frontend
- TypeScript + JavaScript
- CSS
- React / Next.js 

### Deployment and DevOps 
- Render (backend deployment)
- Vercel (frontend deployment)
- Docker (containerized backend) 

## Features 
- ### Authentication and Security
   - User signup/login with JWT-based authentication
   - Protected, user-scoped API endpoints
- ### Application Management
   - Create, view, update, and delete internship applications
   - Track application status: Applied, Offer, Interview, Rejected, Other
   - Sort by name, status, and date applied
- ### Email Classification
   - Input recruiter emails
   - Automatically classify outcomes to speed up status updates
- ### Persistent Data Storage
   - PostgreSQL-backed data persistence for users and applications

## Architecture Overview
- Frontend UI sends requests to the Spring Boot REST API
- Backend handles auth, validation, business logic, and data access
- PostgreSQL stores user/application data persistently

## Future Improvements
- Integrate Gmail API so the app can directly read/crawl relevant recruiting emails
- Replace hardcoded email classification logic with NLP or an LLM API for smarter, more flexible classification
- Create a delete account button
- Architect a system to verify email addresses
