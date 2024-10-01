# Doctor Appointment Web App

This project is a full-stack Doctor Appointment Web Application. It allows users to search for doctors, book appointments, and manage their bookings. Doctors can manage their availability and view patient details, while admins can manage the entire system. The app includes secure authentication using JWT and OAuth, and integrates APIs for email notifications and payments.

## Table of Contents
- [Technologies](#technologies)
- [Features](#features)
  - [User Features](#user-features)
  - [Doctor Features](#doctor-features)
  - [Admin Features](#admin-features)
- [API Integrations](#api-integrations)
- [Future Enhancements](#future-enhancements)
- [Setup and Installation](#setup-and-installation)
- [Contributing](#contributing)
- [License](#license)

## Technologies

### Frontend
- **React.js**
- **Tailwind CSS**
- **Material UI / Ant Design / Chakra UI**
- **Redux**
- **Axios**
- **React Router v6**

### Backend
- **Spring Boot**
- **JWT Authentication**
- **OAuth (Google / Microsoft)**
- **Spring Security 6**
- **PostgreSQL**
- **Redis** (for caching)
- **EmailJS** (for email notifications)
- **Twilio** (for SMS notifications)
- **Stripe** (for payment integration)
- **ELK Stack** or **Prometheus + Grafana** (for logging and monitoring)

## Features

### User Features
- **Registration/Login**: Users can register via email/password or OAuth (Google, Microsoft).
- **Search for Doctors**: Search doctors by specialty, location, and ratings.
- **Book Appointment**: Users can book appointments and receive confirmation via email and SMS.
- **Manage Bookings**: View, cancel, or reschedule upcoming appointments.
- **Profile Management**: Update user profile information.
- **Notifications**: Receive reminders and updates via SMS and email.

### Doctor Features
- **Manage Availability**: Set available time slots.
- **View Appointments**: View details of upcoming appointments and mark them as completed.
- **Manage Profile**: Update profile information and specialties.

### Admin Features
- **Manage Users**: Add, remove, or update user accounts.
- **Manage Doctors**: Add, remove, or update doctor profiles.
- **Manage Appointments**: View and manage all appointments.

## API Integrations

### Third-Party APIs
- **BetterDoctor API**: Provides doctor data, including specialties and locations.
- **Twilio API**: For SMS notifications.
- **EmailJS**: For email notifications.
- **Stripe**: For payment integration.

### Custom APIs
- **Authentication API**: Handles user registration, login, and session management.
- **Doctor Management API**: Manages doctor profiles and availability.
- **Appointment API**: Manages appointments, bookings, and rescheduling.
- **User Management API**: Handles user profiles and management.

## Future Enhancements
1. **Telemedicine Integration**: Add video consultation feature using WebRTC or a third-party API like Vonage or Twilio Video.
2. **Analytics Dashboard**: Include dashboards for doctors and admins to view metrics (e.g., number of appointments, user engagement).
3. **Prescription Management**: Allow doctors to create and send prescriptions to users post-consultation.

## Setup and Installation

### Prerequisites
- Node.js (v14 or higher)
- Java 11 (for Spring Boot)
- PostgreSQL
- Redis

### Frontend Setup
1. Clone the repository:
    ```bash
    git clone https://github.com/hassan-jamshaid10/doctor-appointment-app.git
    cd doctor-appointment-app
    ```
2. Install dependencies:
    ```bash
    npm install
    ```
3. Start the development server:
    ```bash
    npm start
    ```

### Backend Setup
1. Navigate to the backend folder:
    ```bash
    cd backend
    ```
2. Install dependencies and build the project:
    ```bash
    ./mvnw clean install
    ```
3. Run the application:
    ```bash
    ./mvnw spring-boot:run
    ```

### Database Setup
1. Set up PostgreSQL and Redis on your local machine or use cloud services.
2. Update the `application.properties` file with your PostgreSQL and Redis connection details.

### Environment Variables
- Create a `.env` file in the root of the project and add your API keys:
    ```bash
    REACT_APP_STRIPE_KEY=your_stripe_key
    EMAILJS_USER_ID=your_emailjs_user_id
    EMAILJS_SERVICE_ID=your_emailjs_service_id
    EMAILJS_TEMPLATE_ID=your_emailjs_template_id
    TWILIO_ACCOUNT_SID=your_twilio_account_sid
    TWILIO_AUTH_TOKEN=your_twilio_auth_token
    ```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Author 
Hassan Jamshaid <br>
Email: hjamshaid81@gmail.com
