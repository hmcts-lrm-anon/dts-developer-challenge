# HMCTS DTS Developer Challenge

I have developed a basic system for managing tasks that allows caseworkers to track and manage their work.

## Backend API

The backend API:

- Creates tasks with title, description (optional), status, and due date/time
- Retrieves a task by ID
- Retrieves all tasks
- Updates task status and details
- Deletes tasks
- Includes validation and error handling
- Stores data in a database

## Frontend Application

The frontend application:

- Creates, views, updates, and deletes tasks
- Displays tasks in a user-friendly interface
- Provides form validation and error feedback
- Uses GOV.UK Design System components

## How to Use

### Prerequisites

- Java 21+ (for backend)
- Node.js 18+ with yarn (for frontend)
- Docker (for PostgreSQL database)

### Running the System

1. Start the PostgreSQL database:

   ```
   cd hmcts-dev-test-backend/docker
   docker-compose up -d
   ```

2. Start the backend (runs on port 4000):

   ```
   cd hmcts-dev-test-backend
   ./gradlew bootRun
   ```

3. Start the frontend (runs on port 3100):

   ```
   cd hmcts-dev-test-frontend
   yarn install
   yarn start:dev
   ```

4. Access the application at http://localhost:3100

## Repositories

- [Backend Repository](https://github.com/hmcts-lrm-anon/hmcts-dev-test-backend) - Spring Boot REST API
- [Frontend Repository](https://github.com/hmcts-lrm-anon/hmcts-dev-test-frontend) - Express.js web application

## Security & Quality Improvements

- Comprehensive testing
- Comprehensive documentation
- Security enhancements
- Accessibility compliance

## Example Future features

- Search and filtering
- User authentication
- Role-based access
