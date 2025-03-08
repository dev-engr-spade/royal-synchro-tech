# royal-synchro-tech
## Technologies Used

- **Backend**: Java 21, Spring Boot
- **Frontend**: React.js
- **Database**: MongoDB
- **Authentication**: OAuth2 (Google Login)


## Directory Structure Breakdown

com.royalsynchrotech.lom360.command<br>
│	│<br>
│	platform.core<br>
│	│<br>
│	├── config<br>
│	│   ├── SecurityConfig.java          // Configuration for Spring Security and OAuth2<br>
│	│   ├── MongoConfig.java             // MongoDB configuration (if needed)<br>
│	│   └── AppConfig.java               // General application configuration<br>
│	│<br>
│	├── controller<br>
│	│   ├── SuperAdminController.java    // REST controller for Super Admin functionalities<br>
│	│   ├── ClientController.java        // REST controller for Client functionalities<br>
│	│   ├── UserController.java          // REST controller for User functionalities<br>
│	│   ├── ProductController.java       // REST controller for Product functionalities<br>
│	│   └── TransactionController.java   // REST controller for Transaction functionalities<br>
│	│<br>
│  	├── data<br>
│  	│   ├── SuperAdminDTO.java           // Data Transfer Object for Super Admin<br>
│  	│   ├── ClientDTO.java               // Data Transfer Object for Client<br>
│  	│   ├── UserDTO.java                 // Data Transfer Object for User<br>
│  	│   ├── ProductDTO.java              // Data Transfer Object for Product<br>
│  	│   └── TransactionDTO.java          // Data Transfer Object for Transaction<br>
│  	│<br>
│  	├── entity<br>
│  	│   ├── SuperAdmin.java              // Entity class for Super Admin<br>
│  	│   ├── Client.java                  // Entity class for Client<br>
│  	│   ├── User.java                    // Entity class for User<br>
│  	│   ├── Product.java                 // Entity class for Product<br>
│  	│   └── Transaction.java             // Entity class for Transaction<br>
│  	│<br>
│ 	 ├── exception<br>
│  	│   ├── CustomException.java         // Custom exception class<br>
│  	│   └── GlobalExceptionHandler.java  // Global exception handler for REST API<br>
│  	│<br>
│  	├── repository<br>
│  	│   ├── SuperAdminRepository.java    // Repository interface for Super Admin<br>
│  	│   ├── ClientRepository.java        // Repository interface for Client<br>
│  	│   ├── UserRepository.java          // Repository interface for User<br>
│  	│   ├── ProductRepository.java       // Repository interface for Product<br>
│  	│   └── TransactionRepository.java   // Repository interface for Transaction<br>
│  	│<br>
│  	├── security<br>
│  	│   ├── OAuth2UserService.java      // Service for handling OAuth2 user details<br>
│  	│   ├── JwtTokenProvider.java       // JWT token provider (if using JWT)<br>
│  	│   └── UserDetailsServiceImpl.java // Implementation of UserDetailsService<br>
│  	│<br>
│  	├── service<br>
│       ├── SuperAdminService.java      // Service class for Super Admin functionalities<br>
│       ├── ClientService.java          // Service class for Client functionalities<br>
│       ├── UserService.java            // Service class for User functionalities<br>
│       ├── ProductService.java         // Service class for Product functionalities<br>
│       └── TransactionService.java     // Service class for Transaction functionalities<br>
│  <br>
└── StoreManagementApplication.java    // Main application class<br>

### `platform.core`
This is the core of the platform containing key components like configuration files, controllers, services, entities, and repositories.

#### `config`
Contains configuration files for setting up the platform:

- **`SecurityConfig.java`**: Configures Spring Security and OAuth2 for authentication.
- **`MongoConfig.java`**: Handles MongoDB connection setup.
- **`AppConfig.java`**: General application configuration.

#### `controller`
REST API controllers responsible for exposing endpoints related to platform functionalities:

- **`SuperAdminController.java`**: Manages Super Admin-related operations.
- **`ClientController.java`**: Handles Client-related API operations.
- **`UserController.java`**: Manages user-related API operations.
- **`ProductController.java`**: Handles product-related API operations.
- **`TransactionController.java`**: Manages transactions through the API.

#### `data`
Contains **DTOs** (Data Transfer Objects) for each model, which are used to transfer data between layers.

- **`SuperAdminDTO.java`**: DTO for Super Admin data.
- **`ClientDTO.java`**: DTO for Client data.
- **`UserDTO.java`**: DTO for User data.
- **`ProductDTO.java`**: DTO for Product data.
- **`TransactionDTO.java`**: DTO for Transaction data.

#### `entity`
Holds **Entity** classes that represent the structure of the database models.

- **`SuperAdmin.java`**: Represents Super Admin entity.
- **`Client.java`**: Represents Client entity.
- **`User.java`**: Represents User entity.
- **`Product.java`**: Represents Product entity.
- **`Transaction.java`**: Represents Transaction entity.

#### `exception`
Handles custom exceptions and global exception handling:

- **`CustomException.java`**: Custom exception class.
- **`GlobalExceptionHandler.java`**: Global exception handler for REST API errors.

#### `repository`
Contains the repository interfaces for each model:

- **`SuperAdminRepository.java`**: Repository for managing Super Admin entities.
- **`ClientRepository.java`**: Repository for managing Client entities.
- **`UserRepository.java`**: Repository for managing User entities.
- **`ProductRepository.java`**: Repository for managing Product entities.
- **`TransactionRepository.java`**: Repository for managing Transaction entities.

#### `security`
Handles authentication and authorization:

- **`OAuth2UserService.java`**: Service to manage OAuth2 user details.
- **`JwtTokenProvider.java`**: Responsible for JWT token management.
- **`UserDetailsServiceImpl.java`**: Implements `UserDetailsService` for custom user authentication.

#### `service`
Contains service classes for each major functionality:

- **`SuperAdminService.java`**: Business logic related to Super Admin.
- **`ClientService.java`**: Business logic related to Client.
- **`UserService.java`**: Business logic related to User.
- **`ProductService.java`**: Business logic related to Product.
- **`TransactionService.java`**: Business logic related to Transaction.
