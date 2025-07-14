# Full-Stack Application Starter

A modern full-stack application template with Spring Boot backend and React frontend.

## Project Structure

```
task-master-test-/
├── backend/          # Spring Boot application (Java/Gradle)
├── frontend/         # React application (JavaScript/npm)
├── docs/            # Project documentation
├── .gitignore       # Git ignore patterns
└── README.md        # This file
```

## Architecture Overview

This project implements a clean separation between frontend and backend:

- **Backend**: RESTful API built with Spring Boot, providing data and business logic
- **Frontend**: React single-page application (SPA) consuming the backend API
- **Development**: Both components run independently with hot-reload support

## Prerequisites

Before running this application, ensure you have the following installed:

- **Java 17+** (for backend)
- **Gradle 7+** (for backend build)
- **Node.js 18+** (for frontend)
- **npm 9+** (for frontend package management)
- **Git** (for version control)

## Quick Start

### 1. Clone the Repository

```bash
git clone <repository-url>
cd task-master-test-
```

### 2. Backend Setup

```bash
cd backend
./gradlew bootRun
```

The backend will start on `http://localhost:8080`

### 3. Frontend Setup

```bash
cd frontend
npm install
npm start
```

The frontend will start on `http://localhost:3000`

## Development Workflow

1. Start the backend server first (`./gradlew bootRun` in `/backend`)
2. Start the frontend development server (`npm start` in `/frontend`)
3. The frontend is configured to proxy API requests to the backend
4. Both applications support hot-reload for efficient development

## API Documentation

Once the backend is running, you can access:

- Health Check: `GET http://localhost:8080/health`
- API Documentation: Available after implementation

## Testing

### Backend Tests
```bash
cd backend
./gradlew test
```

### Frontend Tests
```bash
cd frontend
npm test
```

## Building for Production

### Backend
```bash
cd backend
./gradlew build
```

### Frontend
```bash
cd frontend
npm run build
```

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.