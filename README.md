# Airbnb Clone Project

This project simulates an Airbnb-like booking platform. It focuses on backend systems, database, APIs, security, and CI/CD pipelines.

Technologies used: Django, MySQL, GraphQL, Docker, GitHub Actions.

## Team Roles

- Backend Developer: Designs and builds the server-side logic and API.
- Database Administrator: Manages database design, optimization, and backups.
- Frontend Developer: Creates the user interface and user experience.
- DevOps Engineer: Builds and maintains the CI/CD pipeline and deployment.
- Security Specialist: Ensures API security, authentication, and data protection.

## Technology Stack

- Django: A web framework used to build the RESTful API backend.
- MySQL: Relational database to store user, property, booking, and payment data.
- GraphQL: API query language to request precise data from the backend.
- Docker: Containerization tool to package and deploy the application consistently.
- GitHub Actions: Automates build, test, and deployment processes (CI/CD).

## Database Design

Entities:
- Users: id, name, email, password, role
- Properties: id, owner_id (User), title, description, location, price
- Bookings: id, user_id, property_id, start_date, end_date, status
- Reviews: id, user_id, property_id, rating, comment
- Payments: id, booking_id, amount, payment_date, status

Relationships:
- A user can own multiple properties.
- A booking belongs to one user and one property.
- Users can leave many reviews for different properties.
- Each booking has a related payment.

## Feature Breakdown

- User Management: Allows users to register, log in, and manage profiles.
- Property Management: Users can list and edit properties for rent.
- Booking System: Users can search properties and make bookings.
- Review System: Users can leave feedback on properties.
- Payment Processing: Handles payment transactions securely.

## API Security

- Authentication: Verify user identity, e.g., using JWT tokens.
- Authorization: Control access to resources based on user roles.
- Rate Limiting: Prevent abuse by limiting API call frequency.
- Data Encryption: Protect sensitive information in transit.
- Input Validation: Guard against injection attacks and bad data.

## CI/CD Pipeline

CI/CD pipelines automate building, testing, and deployment to speed up development and reduce errors.

Tools like GitHub Actions help run tests automatically on every change and deploy code using Docker containers for consistency.
