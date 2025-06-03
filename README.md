# Onion Architecture Application

This is a .NET Core application built using the Onion Architecture pattern, which provides a clean and maintainable way to structure enterprise applications.

## Project Structure

The solution is organized into the following layers:

- **OAA.Web**: The presentation layer containing the web interface and API controllers
- **OAA.Service**: The application service layer containing business logic and use cases
- **OAA.Repo**: The repository layer handling data access and persistence
- **OAA.Data**: The domain layer containing entities, interfaces, and domain logic

## Architecture Overview

The project follows the Onion Architecture pattern with the following key principles:

1. **Domain Layer (OAA.Data)**
   - Contains enterprise business rules
   - Independent of other layers
   - Contains entities and interfaces

2. **Repository Layer (OAA.Repo)**
   - Implements data access logic
   - Implements interfaces defined in the domain layer
   - Handles database operations

3. **Service Layer (OAA.Service)**
   - Contains application business rules
   - Orchestrates the flow of data
   - Implements use cases

4. **Web Layer (OAA.Web)**
   - Handles HTTP requests
   - Contains controllers and views
   - Manages user interface

## Getting Started

### Prerequisites

- .NET Core SDK (latest version)
- Visual Studio 2019 or later
- Git

### Setup

1. Clone the repository:
   ```bash
   git clone [repository-url]
   ```

2. Open the solution in Visual Studio:
   ```
   OnionArchitectureApp.sln
   ```

3. Restore NuGet packages

4. Build the solution

5. Run the application

## Development

- Follow the Onion Architecture principles when adding new features
- Keep the domain layer independent of other layers
- Use dependency injection for loose coupling
- Write unit tests for business logic

## License

This project is licensed under the terms included in the LICENSE.txt file.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request 