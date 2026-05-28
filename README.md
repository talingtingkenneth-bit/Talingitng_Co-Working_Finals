# Talingitng_Co-Working_Finals
FlexSpace: Integrated Coworking & Workspace Management System
1. Project Overview
FlexSpace is a Java-based desktop application designed to streamline the operations of a coworking space. It replaces manual booking logs with a robust digital system that manages members, workspace inventory, and amenity reservations. The system ensures data integrity through a relational database model, preventing double bookings and maintaining clear links between members and their reserved resources.

2. Key Features
Member Management: Full CRUD (Create, Read, Update, Delete) operations for member profiles.

Workspace Booking: An integrated interface to book Hot Desks, Private Offices, and Meeting Rooms.

Search Functionality: Efficient filtering of records to find members or bookings by name/ID.

Amenity Integration: Allows users to add optional amenities (High-speed internet, Coffee, etc.) to specific bookings using a many-to-many relationship.

Data Validation: Prevents invalid inputs (e.g., non-numeric prices) and handles SQL foreign key constraints to prevent orphan records.

3. Tech Stack
Language: Java (JDK 17+)

GUI Framework: Java Swing (NetBeans GUI Builder)

Database: MySQL (Relational Model)

Driver: JDBC (MySQL Connector/J)

Version Control: GitHub

4. Database Schema
The system utilizes a relational schema with 5 related tables:

members: Stores member contact information.

workspaces: Inventory of available rooms and daily rates.

bookings: The core transaction table linking members to workspaces.

amenities: A catalog of additional services.

booking_amenities: A junction table managing the selection of multiple amenities per booking.

5. Installation & Setup
To run this project locally, follow these steps:

Prerequisites
Install XAMPP or MySQL Workbench.

Install NetBeans IDE or IntelliJ.

Download the MySQL Connector/J (.jar file).

Database Setup
Open your MySQL admin tool (phpMyAdmin or Workbench).

Create a new database named coworking_db.

Import the provided flexspace_db_setup.sql file located in the project root.

Application Setup
Clone this repository or extract the ZIP file.

Open the project in your IDE.

Add the mysql-connector-java.jar to your project's Libraries.

Navigate to src/com/flexspace/db/DatabaseConnection.java and update your database credentials (user and password).

Run MainDashboardFrame.java to launch the application.

6. Project Structure
Plaintext
FlexSpace/
├── src/
│   ├── com.flexspace.gui/      # JFrame and JPanel classes
│   ├── com.flexspace.models/   # Entity classes (Member, Booking, etc.)
│   └── com.flexspace.db/       # Database connection logic
├── flexspace_db_setup.sql      # Database export script
├── README.md                   # Project documentation
└── Documentation/              # ERD, UML, and GUI Screenshots
7. Author
Your Name:Kenneth lance Talingting

Course: Object-Oriented Programming (Final Project)

How to submit this on GitHub:
Create your repository.

Upload your src folder, your nbproject folder, your .sql file, and this README.md file.

GitHub will automatically detect the README.md and display it beautifully on your main repository page!
