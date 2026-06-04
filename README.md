# STUDENT EVENT REGISTRATION SYSTEM

## 1. Project Overview

College events play an important role in enhancing student engagement, skill development, and extracurricular participation. However, managing event registrations manually can be time-consuming and error-prone. This project provides a digital platform that allows students to register for events online while enabling organizers to efficiently manage participants, attendance, notifications, and event-related activities.

---

## 2. Problem Analysis and Requirement Gathering

In many educational institutions, event registration and participant management are handled manually through forms and spreadsheets. This often leads to duplicate entries, data inconsistencies, and difficulties in tracking registrations.

The Student Event Registration System addresses these challenges by providing an automated platform for event creation, registration, attendance tracking, certificate generation, and event reporting.

---

## 3. Objectives and Goals

### Main Objective

To develop a web-based Student Event Registration System that simplifies event management and enables students to register and participate in events efficiently.

### Specific Objectives

* To provide secure student registration and login functionality.
* To allow administrators to create and manage events.
* To enable students to browse and register for available events.
* To track participant registrations and attendance.
* To generate participation certificates automatically.
* To send notifications and updates regarding events.
* To collect participant feedback after events.
* To generate reports and analytics for event organizers.
* To improve event management efficiency and user experience.

---

## 4. User Roles and System Modules

### 1. User Authentication Module

Allows students and administrators to register, log in, and securely access the system.

### 2. Event Creation Module

Enables administrators to create, update, and manage event details.

### 3. Event Registration Module

Allows students to view and register for available events.

### 4. Participant Management Module

Manages registered participants and their event information.

### 5. Attendance Tracking Module

Records participant attendance during events.

### 6. Notification Module

Sends event reminders, updates, and announcements.

### 7. Certificate Generation Module

Automatically generates participation certificates for attendees.

### 8. Feedback Management Module

Collects feedback and ratings from participants after event completion.

### 9. Dashboard and Reporting Module

Displays event statistics, participant counts, and reports.

### 10. Database Administration Module

Stores and manages all user, event, and registration data.

---

## 5. Database Requirement Analysis

The system must support the following operations:

### User Management

Users can register and log in.

Store user details:

* user_id (Primary Key)
* name
* email (Unique)
* password (Encrypted)
* role

### Event Management

Administrators can create and manage events.

Each event contains:

* event_id (Primary Key)
* event_name
* description
* event_date
* venue
* organizer

### Registration Management

Students can register for events.

Registration details:

* registration_id (Primary Key)
* user_id (Foreign Key)
* event_id (Foreign Key)
* registration_date
* status

### Attendance Management

Attendance records contain:

* attendance_id (Primary Key)
* registration_id (Foreign Key)
* attendance_status

### Relationship Handling

* One User → Multiple Event Registrations (1:M)
* One Event → Multiple Registrations (1:M)
* One Registration → One Attendance Record (1:1)

### Integrity Requirements

#### Primary Keys

* user_id
* event_id
* registration_id
* attendance_id

#### Unique Constraints

* email must be unique

#### Foreign Keys

* registration.user_id → user.user_id
* registration.event_id → event.event_id
* attendance.registration_id → registration.registration_id

#### Relationship Constraints

* User → Registration = One-to-Many (1:M)
* Event → Registration = One-to-Many (1:M)
* Registration → Attendance = One-to-One (1:1)

---

## 6. ER Diagram Design

Insert the ER Diagram image here.

docs/ERDiagram.png

---

# Technology Stack

## Frontend

* HTML
* CSS
* JavaScript
* Bootstrap

## Backend

* PHP

## Database

* MySQL

## Server

* Apache Server (XAMPP)

## Development Tools

* Visual Studio Code
* GitHub
* Postman

---

# System Features

* Student Registration and Login
* Event Creation and Management
* Online Event Registration
* Participant Management
* Attendance Tracking
* Event Notifications
* Certificate Generation
* Feedback Collection
* Dashboard Analytics
* Report Generation

---

# Project Workflow

Student Login/Register

↓

Browse Available Events

↓

Event Registration

↓

Registration Confirmation

↓

Event Participation

↓

Attendance Tracking

↓

Certificate Generation

↓

Feedback Submission

↓

Dashboard and Report Generation

---

# Current Progress

## Completed

* Project Title Finalization
* Requirement Gathering
* Technology Stack Selection
* Literature Survey

## In Progress

* Objective Definition
* Module Design
* Database Design
* User Interface Design
* ER Diagram Creation

## Upcoming Tasks

* Frontend Development
* Backend Development
* Database Implementation
* Integration Testing
* System Testing
* Documentation
* Final Deployment

