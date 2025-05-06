# Pet Salon Appointment Scheduler
Allows the user to create, edit, and delete scheduled pet appointments and pet records for their pet grooming shop.

Author: Timothy Johnson <br>
Date: December 2022 to January 2023

## Overview

A full-featured desktop application to manage appointments, clients, and pets for a pet grooming salon.
Built with Java and JavaFX, it offers user authentication, database integration with MySQL/PostgreSQL, and generates detailed business reports.

The Pet Salon Appointment Scheduler is a desktop JavaFX application designed for small pet grooming businesses.
Users can securely log in, schedule or edit appointments, manage pet records, and generate detailed reports based on service type, groomer, or city.

🧩 Features

    🐶 Add, edit, and delete pet records from a central database

    📅 Schedule appointments with service type, date, time, and assigned groomer

    👤 User login and authentication to access the app

    📊 Built-in reporting: view services by type, sales by groomer, and appointments by city

    🗃️ View and filter appointment data through intuitive tabs and tables

    🧾 Status toggle for completed/canceled appointments

🔄 User Workflow

    Login using your username and password

    Manage Appointments: Create, update, or remove appointments

    Manage Pet Records: Add new pets, or modify existing entries

    View Reports: Navigate to the Reports tab and generate yearly summaries

    Data Persistence: All changes are saved to a connected MySQL or PostgreSQL database


📁 Code Structure

. <br>
├── PetAppointments/ <br>
│   ├── Main.java &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; Launches the app and connects to the database <br>
│   ├── JDBC.java &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; DB connection logic <br>
│   ├── README.md &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; <br>
│   ├── dataLayout/ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Data models <br>
│   ├── databaseAccess/ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; DB queries and DAO logic <br>
│   │   └── PetTypeAccess.java &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; Example: Loads pet types from the DB <br>
│   ├── forms/ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; FXML UI files <br>
│   │   └── loginPage.fxml &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; Login screen UI layout <br>
│   ├── lang/ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Language Data <br>

⚙️ How It Works
Main Application

    Loads FXML UI via JavaFX

    Connects to a MySQL or PostgreSQL database on startup

    Initializes the login screen and transitions to the dashboard after authentication

Reporting System

    🧾 Appointments by Service Type (for the year)

    💇 Sales by Groomer (for the year)

    🏙️ Appointments by City (for the year)

Reports are tab-separated and pull data directly from the connected SQL database.

🖼️ Screenshots / Visuals

🧰 Technologies Used

    ☕ Java 17.0.4.1

        JavaFX SDK 17.0.1

        OpenJFX 11.0.2

    🧩 UI Development:

        FXML for interface layout

        JavaFX Scene Builder

    🗃️ Database Systems:

        MySQL – Primary database (via mysql-connector-java-8.0.26)

        pgAdmin (PostgreSQL) – Used for testing SQL queries and managing schemas during development

    📄 Data Handling:

        SQL: CRUD operations for appointments, pets, and groomers

        File I/O: Reads pet types, handles session/login configurations

    🧪 Development Environment:

        IntelliJ IDEA 2021.1.3 (Community Edition)

        Java Runtime Environment 11.0.11+9-b1341.60 (amd64)

🚀 Getting Started

    1. Clone the repository:

      git clone https://github.com/yourusername/pet-salon-scheduler.git
      cd pet-salon-scheduler
      
    2. Open the project in IntelliJ IDEA or another Java IDE

    3. Configure your MySQL/PostgreSQL connection inside JDBC.java

    4. Run the application:
    
      java PetAppointments.Main

🌱 Planned Features

    📆 Calendar view for appointments

    🐾 Advanced pet filtering (by breed, age, service history)

    📥 Export reports as CSV or PDF

    🛑 Appointment conflict checking

    🌐 Language localization and dark mode

🪪 License

This project is open source and available under the [MIT License](https://opensource.org/license/mit).
