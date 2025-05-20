# ASP.NET Core Web API Project Guidelines

This ASP.NET Core Web API project follows clean architecture principles and standard RESTful API practices.
When generating code for this project, please ensure that:
- All controllers should follow RESTful conventions
- Use async/await for IO-bound operations
- Use dependency injection for services
- Include proper XML documentation for public APIs
- Follow Microsoft's C# coding conventions
- New features should include appropriate unit tests
- Ensure proper error handling and status codes in controllers
- Use ILogger for logging important operations

Primary technologies:
- ASP.NET Core (latest version)
- Entity Framework Core for data access
- Swagger/OpenAPI for API documentation
- xUnit for unit testing
- Serilog for structured logging

Project architecture:
- Controllers handle API requests and responses
- Services layer contains business logic
- Repository pattern for data access
- DTOs for data transfer
- Do not put business logic in controllers
- Use middleware for cross-cutting concerns
- Maintain separation of concerns
- Avoid tight coupling between components

Security practices:
- Never hardcode credentials, use configuration/user secrets instead
- Always validate user input
- Use proper authentication and authorization
- Apply HTTPS redirection and HSTS
- Implement rate limiting for public APIs
- Follow OWASP security guidelines
- Ensure proper exception handling that doesn't leak sensitive information
