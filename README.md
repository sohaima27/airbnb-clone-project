# airbnb-clone-project

##  Overview
This is a full-stack web development project aimed at replicating the core features of Airbnb. It includes user management, property listings, booking system, payments, and reviews.

##  Project Goals
- Understand backend architecture and database design
- Implement API development with Django REST Framework and GraphQL
- Ensure secure transactions and proper authentication
- Collaborate using GitHub workflows and CI/CD

##  Tech Stack
- Python (Django)
- Django REST Framework
- GraphQL
- MySQL
- Docker
- Redis & Celery
- Git & GitHub
- CI/CD with GitHub Actions
  


  ## Team Roles

In this project, several key roles contribute to its success. Below are the main roles and their responsibilities:

### Backend Developer
Responsible for designing, implementing, and maintaining the server-side logic, APIs, and database interactions. They ensure that the backend services perform efficiently and securely.

### Database Administrator (DBA)
Manages the database design, implementation, and maintenance. They optimize data storage, indexing, and ensure data integrity and security.

### DevOps Engineer
Handles the deployment, monitoring, and scaling of the application infrastructure. They automate workflows using CI/CD pipelines and manage server environments.

### QA Engineer
Ensures the quality of the software through rigorous testing, identifying bugs, and validating that all features meet the required standards before deployment.

---

These roles collaborate closely to deliver a robust, scalable, and secure application.


## Technology Stack

This project uses the following technologies:

- **Django**: A high-level Python web framework used for building the backend and creating RESTful APIs.
- **Django REST Framework**: A toolkit to build Web APIs easily and efficiently with Django.
- **PostgreSQL**: A powerful relational database system used to store and manage application data.
- **GraphQL**: A flexible query language and runtime for APIs, allowing clients to request exactly the data they need.
- **Celery**: An asynchronous task queue used for handling background tasks like sending notifications or processing payments.
- **Redis**: An in-memory data structure store used for caching and session management to improve performance.
- **Docker**: A containerization platform that helps in creating consistent development and deployment environments.
- **CI/CD Pipelines**: Automated workflows for continuous integration and continuous deployment, ensuring efficient testing and delivery of code changes.

---

These technologies work together to build a scalable, efficient, and maintainable Airbnb Clone backend.


## Database Design

The database for this project is designed to manage key entities and their relationships effectively. The main entities include:

### Users
- **id**: Unique identifier for each user.
- **username**: The user's login name.
- **email**: User's email address.
- **password**: Hashed password for authentication.
- **profile_info**: Additional user details like name, bio, etc.

### Properties
- **id**: Unique identifier for each property.
- **owner_id**: References the user who owns the property.
- **title**: Name or title of the property.
- **description**: Details about the property.
- **location**: Address or location details.

### Bookings
- **id**: Unique identifier for each booking.
- **user_id**: References the user who made the booking.
- **property_id**: References the booked property.
- **start_date**: Booking start date.
- **end_date**: Booking end date.

### Reviews
- **id**: Unique identifier for each review.
- **user_id**: References the user who wrote the review.
- **property_id**: References the reviewed property.
- **rating**: Numeric rating value.
- **comment**: Text feedback from the user.

### Payments
- **id**: Unique identifier for each payment.
- **booking_id**: References the related booking.
- **amount**: Payment amount.
- **payment_date**: Date of the transaction.
- **status**: Payment status (e.g., completed, pending).

### Relationships:
- A **User** can own multiple **Properties**.
- A **User** can make multiple **Bookings**.
- Each **Booking** is associated with one **Property**.
- A **User** can write multiple **Reviews** for different properties.
- Each **Payment** is linked to a specific **Booking**.

---

This design ensures data consistency and supports the core functionalities of the Airbnb Clone project.



