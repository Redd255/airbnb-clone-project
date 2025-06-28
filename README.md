# 🏠 Airbnb Clone Project

This project is a backend simulation of a scalable property booking platform like Airbnb. It focuses on user management, property listings, bookings, reviews, payments, and secure backend development using modern tools and frameworks.

---

## 📌 Team Roles

- **Backend Developer**: Implements API endpoints, database schema, and core backend logic.
- **Database Administrator**: Designs and optimizes the database schema and ensures data integrity.
- **DevOps Engineer**: Manages deployment, CI/CD pipeline setup, and Docker configuration.
- **Security Specialist**: Applies security best practices like authentication, authorization, and rate limiting.
- **Project Manager**: Coordinates team efforts and manages timelines and deliverables.

---

## 🛠 Technology Stack

- **Django**: A web framework for building backend logic and RESTful APIs.
- **PostgreSQL**: A relational database used for structured data storage.
- **GraphQL**: Provides flexible and efficient querying of backend data.
- **Docker**: Containerizes the application for consistent development and deployment.
- **GitHub Actions**: Automates testing and deployment through CI/CD pipelines.

---

## 🗃 Database Design

**Entities:**

- **User**
  - `id`, `name`, `email`, `password`, `role`
- **Property**
  - `id`, `owner_id`, `title`, `location`, `price_per_night`
- **Booking**
  - `id`, `user_id`, `property_id`, `start_date`, `end_date`
- **Review**
  - `id`, `user_id`, `property_id`, `rating`, `comment`
- **Payment**
  - `id`, `booking_id`, `amount`, `status`

**Relationships:**

- A user can list multiple properties.
- A booking links a user to a property.
- A user can leave reviews for properties.
- Payments are tied to bookings.

---

## ✨ Feature Breakdown

- **User Management**: Users can register, log in, and manage profiles.
- **Property Management**: Hosts can create, edit, and remove property listings.
- **Booking System**: Guests can make and manage property bookings.
- **Payment Processing**: Users can securely pay for bookings.
- **Review System**: Guests can leave ratings and feedback on properties.

---

## API Security
API Security
- **Authentication**: Secure login to verify users.
- **Authorization**: Only authorized users can perform specific actions (e.g., only hosts can edit listings).
- **Rate Limiting**: Prevents abuse like brute-force login attempts.
- **Input Validation**: Protects against malformed or malicious input.
- **Encryption**: Ensures secure data transmission using HTTPS.

**Why Security Is Important:**

- Protects sensitive user and payment data.
- Ensures platform reliability and user trust.
- Prevents unauthorized access and data breaches.

---

## 🔄 CI/CD Pipeline

**CI/CD** (Continuous Integration and Deployment):

- Automates testing and deployment to reduce errors and speed up delivery.
- Improves collaboration and ensures code quality.

**Tools Used:**

- **GitHub Actions**: For running automated tests and deployments.
- **Docker**: For creating a consistent environment across development, staging, and production.
