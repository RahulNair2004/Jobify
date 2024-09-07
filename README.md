# Jobify

## Overview
**Jobify** is a job scheduling and recruitment platform built with the MERN stack (MongoDB, Express.js, React.js, Node.js). Jobify allows users to:
- **Find jobs** by browsing available listings.
- **Give jobs** by posting job listings as recruiters.
- **Schedule interviews** to streamline the job application process for both job seekers and recruiters.

## Features
- **Job Listings:** Browse, filter, and search for jobs based on title, location, salary, and company.
- **Job Application:** Apply for jobs by submitting resumes and tracking application status.
- **Recruiter Dashboard:** Recruiters can post jobs, manage job applications, and schedule interviews.
- **Interview Scheduling:** Set up and track interviews between recruiters and job seekers.
- **User Authentication:** Secure login and registration for job seekers and recruiters using JWT.
- **Profile Management:** Update profiles with resumes, skills, and experience.
- **Admin Panel:** Manage users, jobs, and applications with an admin dashboard.

## Tech Stack
- **Frontend:**
  - React.js
  - Axios for API calls
  - Redux (optional) for state management
  - CSS for styling (or any preferred framework like Bootstrap/Material-UI)
  
- **Backend:**
  - Node.js + Express.js
  - MongoDB with Mongoose for data handling
  - JWT for secure authentication
  - Bcrypt for password hashing

## Installation and Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/jobify.git
   cd jobify
2. **Install dependencies:**

   For the backend:
   ```bash
   cd server
   npm install
3. ** Set up environment variables: In the server folder, create a .env file with the following variables:**
   ```bash
   MONGO_URI=your_mongodb_uri
   JWT_SECRET=your_jwt_secret
   PORT=5000
4. ** Start the development server: **
   For the backend:
   ```bash
   npm run dev
   ```
   For the frontend:
   ```bash
   npm start

## API Endpoints

### Job Routes:
- `GET /api/jobs` - Get all jobs
- `POST /api/jobs` - Create a new job (for recruiters)
- `GET /api/jobs/:id` - Get a specific job by ID
- `PUT /api/jobs/:id` - Update a job (for recruiters)
- `DELETE /api/jobs/:id` - Delete a job

### User Routes:
- `POST /api/users/register` - Register a new user
- `POST /api/users/login` - User login
- `GET /api/users/me` - Get the logged-in user's profile

### Interview Routes:
- `POST /api/interviews` - Schedule a new interview
- `GET /api/interviews/:userId` - Get all interviews for a specific user

## License

This project is licensed under the MIT License - see the [LICENSE](MIT) file for details.
