# CareerCarve - Mentor Booking Platform
## Project Overview
CareerCarve is a web application that allows students to book 1x1 sessions with mentors based on the availability and preferences of both parties. The platform handles scheduling, mentor-student matching based on areas of interest, and payment processing.

## Features
Mentor Matching: Students can browse and book sessions with mentors based on their areas of interest.
Scheduling: Manage bookings and schedules for both students and mentors.
Payment Processing: Simple payment calculation based on session duration and mentor status (premium or regular).
## Tech Stack
Frontend: React.js
Backend: Node.js, Express.js
Database: SQLite
Deployment: (Specify the platform if deployed)
## Getting Started
### Prerequisites
Node.js (v14+)
npm (v6+)
### Installation
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/career-carve.git
cd career-carve
#### Backend Setup:

Navigate to the backend directory:
bash
Copy code
cd backend
Install dependencies:
bash
Copy code
npm install
Start the backend server:
bash
Copy code
npm start
#### Frontend Setup:

Navigate to the frontend directory:
bash
Copy code
cd ../frontend
Install dependencies:
bash
Copy code
npm install
Start the frontend server:
bash
Copy code
npm start
## Directory Structure
backend/: Contains the server-side code using Node.js and Express.js.
frontend/: Contains the client-side code using React.js.
## Database Schema
### Mentors Table:

id
name
availability
areas_of_expertise
is_premium
### Students Table:

id
name
availability
area_of_interest
### Bookings Table:

id
student_id
mentor_id
session_time
is_paid
## API Endpoints
Mentors:
GET /mentors: Fetch all mentors.
Bookings:
POST /bookings: Create a new booking.
GET /bookings: Retrieve bookings for a student or mentor.
## Frontend Components
BookingForm: Allows students to select a mentor, choose a duration, and specify their area of interest.
MentorList: Displays available mentors based on the student's area of interest.
PaymentPage: Handles payment processing after a session is booked.
## Testing
Manual Testing: Verify the booking process, mentor matching, and payment calculations.
Debugging: Use browser developer tools and console logs for troubleshooting.
## Deployment
Deploy the application to a web service that supports Node.js (Vercel). Ensure the environment variables and database connections are properly configured.

## Future Improvements
Automated Testing: Implement unit and integration tests.
Enhanced Payment Integration: Integrate with a payment gateway like Stripe or PayPal.
Notifications: Add email or SMS notifications for bookings.