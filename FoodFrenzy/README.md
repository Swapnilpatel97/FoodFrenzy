# FoodFrenzy (Swapnil Patel)
FoodFrenzy is a comprehensive system designed for managing customers, inventory, and orders. It offers secure authentication, role-based access control, and database integration using MySQL. Built with Spring Boot and Thymeleaf, the application provides a seamless experience for admin and staff members.

![f1](https://github.com/user-attachments/assets/7f191ae8-747a-4539-a55b-d51c207a44de)



## Features

- **Customer Management**: Easily add, update, and delete customer information.
- **Inventory Management**: Keep track of your inventory items, including stock levels and pricing.
- **Order Management**: Manage customer orders, including order creation, updates, and status tracking.
- **User Authentication**: Secure login and authentication for admin and staff members.
- **Role-Based Access Control**: Define roles and permissions for different user types.
- **Thymeleaf Templates**: Utilizes Thymeleaf for dynamic HTML templates.
- **Database Integration**: Integrated with MySQL for data storage and retrieval.

## Technology Stack

- **Backend**: Spring Boot, Java 8, Spring MVC, Spring Data JPA (Hibernate)
- **Frontend**: Thymeleaf, HTML, CSS, JavaScript
- **Database**: MySQL
- **IDE**: VsCode, Intellij Idea

## Prerequisites

Before running this project, ensure you have the following installed:

- Minimum Java 8
- MySQL
- Maven
- Vs Code

## Setup and Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Swapnilpatel97/FoodFrenzy.git
    ```

2. Navigate to the project directory:
    ```bash
    cd FoodFrenzy
    ```

3. Configure MySQL Database:
    - Create a new MySQL database.
    - Update `application.properties` with your MySQL credentials:
      ```properties
      spring.datasource.url=jdbc:mysql://localhost:3307/foodfrenzy
      spring.datasource.username=root
      spring.datasource.password=****
      spring.jpa.hibernate.ddl-auto=update
      ```

4. Run the project:
    ```bash
    mvn spring-boot:run
    ```

5. Access the application:
    - Navigate to `http://localhost:8080` in your browser. 
## Website Screenshot

Here is a preview of the FoodFrenzy interface:

![f1](https://github.com/user-attachments/assets/d47a757b-2ca5-4a15-b8ef-429635c9f8c5)

![f2](https://github.com/user-attachments/assets/f8646a07-1894-4229-b116-cea57b856243)

![f3](https://github.com/user-attachments/assets/224235d4-3b03-4c37-9c55-173e7f248298)

![f4](https://github.com/user-attachments/assets/bbefb1bf-5c6d-4c44-b9e4-6b9c740741c5)

![f5](https://github.com/user-attachments/assets/bc74215f-661e-4a5f-86c2-58608eca773a)

![f6](https://github.com/user-attachments/assets/d4bff42b-6a03-490b-b628-1707827adb34)

![f7](https://github.com/user-attachments/assets/a938cce8-70dc-45e2-9d32-dd57653c1a77)

![f8](https://github.com/user-attachments/assets/59746619-b9ec-46cb-830d-c6054b2d270e)

![f9](https://github.com/user-attachments/assets/8954623c-a200-4fc5-ab21-a9e4d9d57982)

![f10](https://github.com/user-attachments/assets/0aa33585-829c-4c06-ac60-89b4f698107c)


## Project Structure

```bash
src/
├── main/
│   ├── java/
│   │   └── com.example.foodfrenzy/
│   │       ├── controller/      # Contains all controllers
│   │       ├── model/           # Contains entity classes
│   │       ├── repository/      # Repository interfaces for database interaction
│   │       └── service/         # Service layer with business logic
│   ├── resources/
│   │   ├── templates/           # Thymeleaf templates for views
│   │   ├── static/              # Static assets (CSS, JavaScript)
│   │   └── application.properties  # Project configuration
│   └── webapp/
│       └── WEB-INF/
│           └── views/           # Additional view files
└── test/                        # Test cases for unit testing
