# Airbnb Clone Project

## Overview

The Airbnb Clone Project is a comprehensive application designed to simulate the development of a robust booking platform similar to Airbnb. This project aims to enhance understanding of full-stack development, focusing on backend systems, database design, API development, and application security.

## Project Goals

- Develop a scalable web application.
- Master collaborative workflows using GitHub.
- Deepen understanding of backend architecture and database design.
- Implement advanced security measures for API development.
- Gain proficiency in CI/CD pipelines for efficient deployment.

## Tech Stack

- **Backend Framework**: Django
- **Database**: MySQL
- **API Technology**: GraphQL
- **Containerization**: Docker
- **CI/CD**: GitHub Actions

## Conclusion

This project will help learners build technical skills while adopting a problem-solving mindset geared toward scalability and industry-grade project execution.

## Team Roles

### 1. Project Manager

The Project Manager oversees the project, ensuring that it stays on track and within budget. They coordinate the team, set deadlines, and manage communication between stakeholders.

### 2. Backend Developer

The Backend Developer is responsible for the server-side logic and integration of the application. They work with databases, APIs, and server frameworks to ensure smooth data flow and functionality.

### 3. Frontend Developer

The Frontend Developer focuses on the user interface and experience. They implement the visual elements that users interact with, ensuring that the application is responsive and user-friendly.

### 4. Database Administrator (DBA)

The DBA manages the database, ensuring data integrity, security, and availability. They design the database schema and optimize database performance for efficient data retrieval.

### 5. Quality Assurance (QA) Engineer

The QA Engineer is responsible for testing the application to identify bugs and ensure that it meets the specified requirements. They create test cases and perform manual or automated tests.

### 6. DevOps Engineer

The DevOps Engineer focuses on the deployment and operations of the application. They set up CI/CD pipelines, manage server environments, and monitor application performance.

### 7. Security Specialist

The Security Specialist ensures that the application is secure from vulnerabilities. They implement security measures, conduct audits, and respond to potential threats.

### 8. UI/UX Designer

The UI/UX Designer is responsible for the application's look and feel. They conduct user research, design wireframes, and create prototypes to enhance user experience.

## Technology Stack

### 1. Django

Django is a high-level web framework for building web applications quickly and efficiently. It follows the Model-View-Template (MVT) architectural pattern and helps in developing RESTful APIs.

### 2. MySQL

MySQL is a relational database management system that stores application data in a structured format. It provides powerful querying capabilities and ensures data integrity.

### 3. GraphQL

GraphQL is a query language for APIs that enables clients to request only the data they need. It allows for more efficient data retrieval compared to traditional REST APIs.

### 4. Docker

Docker is a containerization platform that allows developers to package applications and their dependencies into containers. This ensures consistency across different environments and simplifies deployment.

### 5. GitHub Actions

GitHub Actions is a CI/CD tool that automates workflows directly in GitHub. It helps in building, testing, and deploying applications automatically, enhancing development efficiency.

### 6. Bootstrap

Bootstrap is a front-end framework that provides pre-designed components and styles for building responsive web interfaces. It helps in creating a visually appealing user experience.

### 7. Nginx

Nginx is a web server that can also be used as a reverse proxy. It efficiently handles client requests and serves static content, improving application performance.

### 8. Redis

Redis is an in-memory data structure store used as a database, cache, and message broker. It enhances application performance by providing fast data access and temporary storage.

## Database Design

### Key Entities

**1. Users**

- **user_id**: Unique identifier for each user.
- **username**: The name chosen by the user.
- **email**: User's email address.
- **password**: Hashed password for authentication.
- **created_at**: Timestamp of account creation.

**2. Properties**

- **property_id**: Unique identifier for each property.
- **user_id**: Foreign key linking to the owner (User).
- **title**: Title of the property listing.
- **description**: Detailed description of the property.
- **price_per_night**: Cost of renting the property per night.

**3. Bookings**

- **booking_id**: Unique identifier for each booking.
- **property_id**: Foreign key linking to the booked property.
- **user_id**: Foreign key linking to the user who made the booking.
- **check_in_date**: Date of check-in.
- **check_out_date**: Date of check-out.

**4. Reviews**

- **review_id**: Unique identifier for each review.
- **property_id**: Foreign key linking to the reviewed property.
- **user_id**: Foreign key linking to the user who wrote the review.
- **rating**: Numeric rating given by the user.
- **comment**: Text feedback from the user.

**5. Payments**

- **payment_id**: Unique identifier for each payment.
- **booking_id**: Foreign key linking to the associated booking.
- **amount**: Total amount paid.
- **payment_date**: Date when the payment was made.
- **payment_method**: Method used for payment (e.g., credit card, PayPal).

### Relationships

- A **User** can have multiple **Properties** (one-to-many).
- A **Property** can have multiple **Bookings** (one-to-many).
- A **User** can make multiple **Bookings** (one-to-many).
- A **Booking** belongs to one **Property** and one **User** (many-to-one).
- A **Property** can have multiple **Reviews** (one-to-many).
- A **User** can write multiple **Reviews** (one-to-many).
- A **Review** belongs to one **Property** and one **User** (many-to-one).
- A **Payment** is linked to one **Booking** (one-to-one).
