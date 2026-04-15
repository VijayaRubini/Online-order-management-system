# Online-order-management-system
Online order management system

📌 Project Overview
This is a RESTful Web Service built using the Spring Boot framework to manage the lifecycle of customer orders. The system handles product data ingestion, order validation, and database persistence.
Drawing from my 4 years of QA experience at TCS, I developed this project with a "Quality-First" approach, ensuring robust error handling and defensive coding practices to manage common data-entry failures.
________________________________________
🛠 Tech Stack
•	Language: Java 17
•	Framework: Spring Boot 3.x
•	Data Access: Spring Data JPA / Hibernate
•	Database: H2 (In-Memory) / MySQL
•	Build Tool: Maven
•	API Testing: Postman
________________________________________
🚀 Key Features
•	Layered Architecture: Follows the standard Controller-Service-Repository pattern for clear separation of concerns.
•	Data Validation: Implements business logic to prevent invalid orders (e.g., negative quantities, empty product codes).
•	RESTful Endpoints: Provides a clean API for creating and retrieving orders.
•	Automated Persistence: Uses JPA to map Java objects to database tables automatically.
________________________________________
📁 Project Structure
Plaintext
src/main/java/com/example/order/
├── controller/   # API Endpoints (REST Controllers)
├── service/      # Business Logic & Validation
├── model/        # Database Entities
└── repository/   # Database Access (JPA Repositories)
________________________________________
🚦 How to Run the Project
1.	Clone the repository:
Bash
git clone https://github.com/VijayaRubini/Online-order-management-system.git
2.	Navigate to the project folder:
Bash
cd Online-order-management-system
3.	Run the application:
Bash
mvn spring-boot:run
4.	Access the API: The server will start at http://localhost:8080/api/orders.
________________________________________
🧪 API Documentation (Testing with Postman)
Create a New Order
•	Method: POST
•	URL: /api/orders
•	Body (JSON):
JSON
{
    "customerName": "John Doe",
    "productCode": "RET-102",
    "price": 299.99,
    "quantity": 2
}
________________________________________
💡 QA-to-Dev Insights
During the development of this project, I applied my testing background to:
•	Identify potential null-pointer exceptions in request payloads.
•	Ensure consistent HTTP status codes (201 Created vs. 400 Bad Request).
•	Structure the code for unit testability using JUnit and Mockito.
