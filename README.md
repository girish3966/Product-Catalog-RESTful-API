# Product-Catalog-RESTful-API
Product Catalog RESTful API
This project implements a simple RESTful API for managing a product catalog. It allows you to perform CRUD (Create, Read, Update, Delete) operations on product entities. The project uses Java, Spring Boot, and MongoDB for data storage.

==== Table of Contents ====
1. Prerequisites
2. Project Structure
3. Product Entity
4. Availability and Rating Classes
5. MongoDB Configuration
6. Product Repository
7. REST Controller
8. Endpoints
9. Advanced Features
10.Getting Started

--- Prerequisites ---
Java (JDK 8 or higher)
Spring Boot
MongoDB (local or MongoDB Atlas)

---Project Structure---
src/main/java/com/example/productcatalog: Java source files
src/main/resources: Application properties and MongoDB configuration
pom.xml: Maven project configuration

---Product Entity---
The Product entity has the following attributes:

id: Unique identifier for the product
name: Name of the product
description: Text description of the product
price: Price of the product
categories: List of categories the product belongs to
attributes: Map of additional attributes (e.g., size, color)
availability: Availability details (in stock, quantity)
ratings: List of user ratings

--- Availability and Rating Classes ---
Availability: Represents product availability (in stock, quantity)
Rating: Represents user ratings (user ID, rating value, comment)

--- MongoDB Configuration ---
Configure MongoDB connection properties in application.properties or application.yml.
Use Spring Data MongoDB to connect to the database.

--- Product Repository ---
ProductRepository: Extends MongoRepository<Product, String> for CRUD operations.

--- REST Controller ---
ProductController: Provides endpoints for managing products.

--- Endpoints ---
GET /api/products: Retrieve all products
GET /api/products/{id}: Retrieve a specific product by ID
POST /api/products: Create a new product
PUT /api/products/{id}: Update an existing product
DELETE /api/products/{id}: Delete a product by ID
GET /api/products/search?name={name}&category={category}&attribute={attribute}: Search products

--- Advanced Features ---
Implement pagination and sorting for product retrieval.
Add an endpoint for rating a product.

--- Getting Started ---
1. Set up MongoDB (local or MongoDB Atlas).
2. Configure MongoDB connection properties.
3. Run the Spring Boot application.
   
Contributions are welcome! Feel free to open issues or submit pull requests.
                        THANK YOU
