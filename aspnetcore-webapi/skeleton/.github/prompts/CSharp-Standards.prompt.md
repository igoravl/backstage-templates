# C# Coding Standards

When working with C# files in this project, please follow these conventions:

Follow Microsoft's recommended C# naming conventions:
- PascalCase for namespaces, classes, methods, properties, and public fields
- camelCase for parameters and local variables
- _camelCase for private fields
- I prefix for interfaces (e.g., IRepository)
- Avoid abbreviations in names
- Use meaningful and descriptive names

Code organization principles:
- One class per file (except for small related classes)
- Group usings by .NET namespaces first, then alphabetically
- Keep methods focused and small (aim for 50 lines or less)
- Limit nesting to 3-4 levels maximum
- Use expression-bodied members for simple methods and properties
- Prefer readonly fields where possible
- Use C# latest language features appropriately

Error handling guidelines:
- Use exception filtering when appropriate
- Avoid catch-all blocks without specific exception types
- Don't catch exceptions only to rethrow them
- Add contextual information when rethrowing
- Use Result pattern for predictable errors
- Ensure all exceptions are properly logged

Performance best practices:
- Use async/await for I/O operations
- Avoid blocking calls in async methods
- Use ConfigureAwait(false) in library code
- Use proper collection types for the use case
- Avoid excessive string concatenation
- Be mindful of memory allocations
- Use value types appropriately

Unit testing guidelines:
- Follow Arrange-Act-Assert pattern
- Keep tests focused on single behavior
- Use descriptive test names (Given_When_Then or Feature_Scenario)
- Mock external dependencies
- Test both happy path and edge cases
- Use test data builders when appropriate
