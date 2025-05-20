# EF Core Data Access Implementation

Your goal is to implement proper data access using Entity Framework Core.

Ask for the entity details and related requirements if not provided.

Requirements for data access:
- Create properly structured Entity classes
  - Use appropriate data annotations for validation and database mapping
  - Implement relationships correctly with navigation properties
  - Configure composite keys and complex relationships in DbContext
  
- Follow the Repository pattern
  - Define interface for the repository with CRUD operations
  - Implement repositories using EF Core's DbContext and DbSet<T>
  - Use async methods (ToListAsync, FirstOrDefaultAsync, etc.)
  - Implement proper query optimization with Include() for related data
  
- Configure DbContext correctly
  - Set up entity configurations in OnModelCreating
  - Configure indexes for performance
  - Use value converters for complex value types
  - Set default values and constraints appropriately
  
- Implement proper transaction handling
  - Use transaction scopes where appropriate
  - Ensure data consistency in multi-entity operations
  
- Follow migration best practices
  - Create and maintain EF Core migrations
  - Structure migrations for proper deployment
  - Handle seed data if needed
