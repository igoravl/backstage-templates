# Generate ASP.NET Core API Controller

Your goal is to generate a new ASP.NET Core API controller.

Ask for the controller name and resource/entity type if not provided.

Requirements for the controller:
- Follow REST conventions for endpoint naming
- Implement standard CRUD operations (GET, POST, PUT, DELETE)
- Include proper route attributes and HTTP verb attributes
- Add XML comments for all public API methods
- Implement async patterns with Task<ActionResult<T>> return types
- Use dependency injection for services
- Include proper model validation and error handling
- Return appropriate HTTP status codes (200, 201, 204, 400, 404, etc.)
- Use ActionResult<T> for typed responses
- Include logging with ILogger<T>
- Handle exceptions appropriately
- Use DTOs for request/response instead of exposing domain models directly

Remember to generate both the controller and any required DTOs or model classes.
