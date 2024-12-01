# IREAD Online Learning Platform

## Introduction

This project is a multi-phase website development effort. Currently, we are working on the primary phase, which focuses on authentication management, event management, and blog management. The next phase will introduce course management. The application is designed with a focus on user experience and scalability, enabling efficient creation, viewing, and management of content.

## Technologies Used

- **Frontend**: Next.js, Tailwind CSS
- **Backend**: Node.js, Express
- **Architecture**: MVC (Model-View-Controller)
- **Database**: MySQL
- **Containerization**: Docker

## Features

### Current Phase Features
- User authentication and role management
- Event creation and management
- Blog posting and editing
- Responsive and user-friendly design
- Secure API endpoints

### Upcoming Features
- Course creation and management

## Backend Project Structure

The project follows the MVC pattern for better separation of concerns and maintainability:

```
project-root
|├── src
|   |├── controllers  // Contains logic for handling requests and responses
|   |├── models       // Defines the data structure and database interactions
|   |├── routes       // Contains route definitions for API endpoints
|   |├── views        // Stores frontend templates (if applicable)
|├── public          // Static files and assets
|├── node_modules    // Dependencies installed via npm
|├── package.json   // Project metadata and dependencies
|├── Dockerfile      // Docker configuration for containerizing the project
|├── docker-compose.yml  // Docker Compose configuration
|├── README.md       // Documentation
```

## Setup Instructions

### Prerequisites

- Node.js (>= 16.x)
- npm or yarn
- Git
- Docker and Docker Compose

### Steps

1. **Clone the Repository**:

   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. **Install Dependencies**:

   ```bash
   npm install
   ```

3. **Environment Configuration**:

   - Create a `.env` file in the project root.
   - Add the required environment variables (e.g., database credentials, API keys).

4. **Run the Application Locally (Without Docker)**:

   ```bash
   npm run dev
   ```

   The application will be available at `http://localhost:5000`.

5. **Run the Application Using Docker**:

   - Build and run the Docker container:

     ```bash
     docker-compose up --build
     ```

   - The application will be available at `http://localhost:5000`.

6. **Build for Production**:

   ```bash
   npm run build
   ```

   Deploy the production build to your preferred hosting platform.

## Deployment Instructions

- Ensure your hosting platform supports Docker.
- Push the Docker image to a container registry (e.g., Docker Hub, AWS ECR).
- Deploy the containerized application using a platform like AWS, Google Cloud, or Azure.
- Configure environment variables in the production environment.

## Usage Guide

- **Authentication**:
  - Manage user accounts, roles, and permissions through the Authentication section.
- **Events**:
  - Navigate to the Events section to add, edit, or view event details.
- **Blogs**:
  - Use the Blogs section to create and manage blog posts.

## Development Process

- **Frontend**:
  - Designed using Next.js for server-side rendering and fast performance.
  - Styled with Tailwind CSS for a modern and responsive UI.
- **Backend**:
  - Built with Express, following the MVC architecture.
  - Secure API endpoints for data interaction.
- **Containerization**:
  - Docker is used to containerize the application for consistent development and deployment environments.

## Future Improvements

- Develop course management features.
- AI based solutions.

---
