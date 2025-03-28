# Tracex

## 📌 Project Overview
This project is a **full-stack application** designed to monitor and trace API calls from another application. It logs request execution times, traces HTTP requests, and provides performance reports to help developers detect bottlenecks and optimize application efficiency.

## 🏗️ Architecture
- **Frontend:** Angular
- **Backend:** .NET (Microservices Architecture)
- **Database:** PostgreSQL / MongoDB (for storing logs)
- **Communication:** gRPC / REST
- **Containerization:** Docker
- **Tracing & Logging:** OpenTelemetry / Serilog
- **Testing:** xUnit (Unit Testing), Moq (Mocking), TestContainers (Integration Testing)
- **Documentation:** Swagger, OpenAPI, Markdown-based docs

## ⚡ Core Features

- API Request Tracing: Monitors and records API requests from initiation to response.
- Execution Time Analysis: Measures request execution time, including database interaction times.
- TCP Handshake Tracking: Analyzes the time taken for API calls to establish a connection with the database.
- Error Detection: Identifies failed requests and provides detailed error logs.
- Performance Reports: Generates detailed reports with response time metrics.

## Additional Features

- Filtering & Sorting: Search and filter requests by endpoint, response time, status code, and more.
- Real-time Monitoring: Live dashboard to track API performance.
- Alerts & Notifications: Notify developers when an endpoint exceeds a response time threshold.
- Multi-Tenant Support: Designed for scalability, allowing multiple projects to be monitored simultaneously.

## 📦 Project Structure
```
/monitoring-tool
  ├── frontend/             # Angular frontend
  ├── services/
  │   ├── api-gateway/      # API Gateway for routing requests
  │   ├── tracer-service/   # Service for request tracing
  │   ├── logger-service/   # Centralized logging service
  ├── database/             # Database schema and migrations
  ├── docker/               # Dockerfiles & Compose setup
  ├── tests/                # Unit & integration tests
  ├── docs/                 # Documentation files
```

## 🚀 Setup Guide
### Prerequisites
- Node.js & Angular CLI
- .NET SDK (latest version)
- PostgreSQL or MongoDB
- Docker & Docker Compose

### Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/api-monitoring-tool.git
   cd api-monitoring-tool
   ```
2. Install frontend dependencies:
   ```sh
   cd frontend
   npm install
   ```
3. Set up backend services:
   ```sh
   cd services
   dotnet restore
   dotnet build
   ```
4. Run Docker containers:
   ```sh
   docker-compose up -d
   ```
5. Start the frontend:
   ```sh
   cd frontend
   ng serve
   ```

## 🧪 Testing
- **Unit Tests:** Run `dotnet test` inside the services folder.
- **Integration Tests:** Use TestContainers for running services in isolated environments.
- **E2E Testing:** Use Postman / Playwright.

## 📜 API Documentation
- API documentation is available via Swagger at:
  ```
  http://localhost:5000/swagger
  ```
- OpenAPI specs are stored in the `/docs` directory.

## 🔄 CI/CD Pipeline
- Uses GitHub Actions for automated testing and deployment.
- Docker images are built and pushed to a container registry.
- Supports Kubernetes deployment (future enhancement).

## 🎯 Future Enhancements
- AI-powered anomaly detection for API performance.
- GraphQL support.
- More visualization dashboards.

## 📩 Contributing
Contributions are welcome! Please follow the coding guidelines and submit a pull request.

---

### 👨‍💻 Author
Ahmed Hamza

---

Let me know if you need any modifications or extra details! 🚀


