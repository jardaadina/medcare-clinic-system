# MedCare - Medical Clinic Management System

## Description

MedCare is a desktop application designed for the efficient management of patient appointments in a medical clinic. The system allows for the registration and management of medical consultations, offering a smooth experience for both administrative staff and receptionists.

## Technologies Used

- **Backend:** Java 17, Spring Boot 3.4.4
- **Frontend:** Java Swing
- **Data Persistence:** Spring Data JPA, Hibernate, MySQL
- **Security:** Spring Security, BCrypt (for password encryption)

## Features

### Authentication and Authorization
- Secure login-based access.
- Two user roles: **Administrator** and **Receptionist**.
- Passwords are encrypted in the database.

### Administrators
- Manage receptionist accounts.
- Manage the list of doctors (add, edit, delete).
- Manage medical services offered by the clinic.
- Generate and view reports and statistics.
- Export reports to **CSV** or **XML** format.

### Receptionists
- Manage patient appointments.
- Check doctor availability.
- Update appointment status.
- Search and filter appointments.

### Doctor Management
- Register doctor information.
- Define work schedules for each doctor.
- Check availability for new appointments.

### Medical Services
- Register clinic services.
- Define the price and duration for each service.

### Appointments
- Register and manage appointments.
- Prevent scheduling overlaps.
- Update appointment status.

### Reports and Statistics
- Generate reports for appointments within a specific date range.
- Statistics on the most requested doctors.
- Statistics on the most requested medical services.

## Architecture

The application follows a **Layered Architecture**:
- **Presentation Layer:** User interface developed in Java Swing.
- **Business Logic Layer:** Services that implement the business rules.
- **Data Access Layer:** Repositories that facilitate database access.
- **Data Layer:** Base entities and the data model.

## Project Structure

```text
com.medcare
├── model        # Business entities
├── repository   # Data access interfaces
├── service      # Services implementing business logic
├── ui           # User interface components
└── config       # Spring configurations
