# API Security Review

Your goal is to perform a security review of an ASP.NET Core API.

When reviewing APIs for security issues, check for:

- Authentication implementation
  - Verify JWT token validation is properly implemented
  - Check for proper claims validation
  - Ensure tokens have appropriate expiration

- Authorization controls
  - Verify [Authorize] attributes are applied appropriately
  - Check for proper role/policy-based authorization
  - Look for missing authorization on sensitive endpoints

- Input validation
  - Ensure all user inputs are validated
  - Check for model validation with [Required] and other data annotations
  - Verify custom validation logic for complex business rules

- Data protection
  - Check for proper handling of sensitive data
  - Ensure PII is encrypted at rest and in transit
  - Verify secrets are not exposed in logs or responses

- API-specific vulnerabilities
  - Look for CSRF vulnerabilities on state-changing operations
  - Check for proper rate limiting implementation
  - Ensure protection against injection attacks (SQL, NoSQL, etc.)
  - Verify protection against mass assignment vulnerabilities

- Secure configuration
  - Check for HTTPS enforcement
  - Verify secure cookie settings
  - Ensure proper CORS policy implementation
  - Look for appropriate security headers
