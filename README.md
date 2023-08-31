# Mobile Contacts Application - Data Access Object (DAO)

Welcome to the repository for the Mobile Contacts Application's Data Access Object (DAO) module!

## Summary

The Data Access Object (DAO) module of the Mobile Contacts Application handles interactions with the database, providing methods for storing, retrieving, and managing mobile contact and user details data. It includes interfaces and implementations for accessing and manipulating data.

## Modules

### IMobileContactDAO.java

This interface defines the contract for interacting with the Mobile Contact database. It includes methods for CRUD (Create, Read, Update, Delete) operations on mobile contact records.

### MobileContactDAOImpl.java

This class provides the implementation of the `IMobileContactDAO` interface. It connects to the database and executes SQL queries to perform CRUD operations on mobile contact records.

## Data Transfer Objects (DTO)

### MobileContactDTO.java

This DTO (Data Transfer Object) class represents a mobile contact's data in a format that can be easily transferred between layers of the application. It mirrors the structure of the `MobileContact` model.

### UserDetailsDTO.java

This DTO class represents user details' data in a format suitable for data transfer between layers of the application. It mirrors the structure of the `UserDetails` model.

## Model

### AbstractEntity.java

An abstract class, `AbstractEntity`, serves as the base class for all entities in the application. It provides common fields like `id` and methods that entities can inherit.

### IdentifiableEntity.java

An abstract class, `IdentifiableEntity`, extends `AbstractEntity` and provides a unique identifier (ID) for entities. Other entities in the application can inherit this class to have a common ID field.

### MobileContact.java

The `MobileContact` class represents a mobile contact entity, including attributes like name, phone number, and email.

### UserDetails.java

The `UserDetails` class represents user details, such as username and password. It can be associated with mobile contacts for authentication purposes.

## Service

### Main.java

The `Main` class contains the application's entry point, where the program execution begins. It sets up the application and starts it.

### MobileContactsApp.java

The `MobileContactsApp` class represents the main application logic. It uses the DAO to interact with the database and provides methods for managing mobile contacts and user details.

## Installation and Execution

To run the Mobile Contacts Application with the DAO module:

1. Install the required dependencies, including a suitable database.

2. Download the source code for the entire application, including the DAO module.

3. Configure the database connection settings in the appropriate configuration files.

4. Run the application by executing the main class `Main.java` or `MobileContactsApp.java`, depending on your preferred setup.

## License

This application is licensed under the [MIT License](LICENSE), allowing free use, distribution, and modification of the code.

## Contact

For any questions, comments, or issues related to this module, please feel free to contact us at [dimthoma@aueb.gr].
