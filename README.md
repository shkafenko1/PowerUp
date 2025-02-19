# PowerUp - an app for your fitness centre

Welcome to the **PowerUp App** – a full-stack application designed to help clients manage their workouts and meal plans while empowering instructors to schedule and manage group sessions. The backend is built with Spring Boot using Gradle (Groovy DSL) and the frontend is built with React.

---

**Contents:**

1. Features
2. Tech Stack
3. Installation & Setup
4. Usage
5. API Endpoints
6. Contributing
7. Contact

## Features

- **Dual User Types:**
    - Client: Manage memberships, track solo workouts, enroll in group sessions, top-up balance via Robokassa, and receive personalized workout & meal plans powered by AI.
    - Instructor: Create and manage group workouts, view enrolled clients, and monitor earnings.
- **Workout Management:**
    - Track solo workouts tied to memberships.
    - Enroll and manage group workout sessions.
- **AI-Powered Plans:**
    - Generate personalized workout and meal plans based on client inputs through an external AI API.
- **Secure Payment Integration:**
    - Process payments via the Robokassa API with full transaction history and balance management.
- **Responsive Frontend:**
    - User-friendly interface built with React ensuring a responsive experience across devices.

## Tech Stack

- **Backend: Spring Boot with Gradle (Groovy DSL)**
- **Frontend: React**
- **Database: PostgreSQL**
- **External APIs: Robokassa API for payment processing; AI API for personalized workout and meal plan generation**

## Installation & Setup

**Backend**

1. Clone the repository from https://github.com/shkafenko1/PowerUp.
2. Navigate to the backend directory.
3. Check the build.gradle file (Groovy DSL) to ensure dependencies and plugins are configured.
4. Edit the application.properties or application.yml file to set up your database connection, Robokassa API keys, AI API endpoint, etc.
5. Use Gradle commands to build and run the project:
    - Clean and build the project.
    - Run the application using the bootRun command.
      The backend will start on the configured port (default is usually 8080).

**Frontend**

1. Navigate to the frontend directory.
2. Install the required dependencies.
3. Start the development server.
   The React application will be available at http://localhost:3000.

## Usage

**For Clients:**
- Register or log in.
- Manage memberships, track solo workouts, and enroll in group sessions.
- Submit data for AI-powered personalized workout and meal plans.
- Top-up your balance and view transaction history.

**For Instructors:**
- Register or log in.
- Create and manage group workout sessions.
- View details of enrolled clients.
- Track earnings from group sessions.

## API Endpoints

**Key endpoints include:**
- User Management:
    - POST /api/auth/register to register a new client or instructor.
    - POST /api/auth/login to authenticate and obtain a JWT token.
- Workout Management:
    - GET /api/workouts to retrieve available workouts.
    - POST /api/workouts/enroll for a client to enroll in a group workout.
- Payment Processing:
    - POST /api/payments/process to initiate a payment via Robokassa.
    - GET /api/payments/history to retrieve payment transaction history.
- AI Plan Generation:
    - POST /api/ai/generate to submit data for generating personalized plans.
    - GET /api/ai/plan/{clientId} to retrieve the generated plan for a client.

Note: Endpoints may evolve as the project develops.

## Contributing

Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes with clear messages.
4. Push your changes to the branch.
5. Submit a Pull Request.
   For major changes, open an issue first to discuss what you would like to change.

Contact

- Project Repository: https://github.com/shkafenko1/PowerUp
- Author: t.me/shkafenko1