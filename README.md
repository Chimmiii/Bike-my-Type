🚴 Bike my Type: Bike Rental Management System

Table of Contents

🚀 Overview

✨ Key Features

💻 Project Structure

🛠️ Technologies Used

📂 Getting Started

👥 Group Members

🚀 Overview

Bike my Type is a robust bike rental management system developed for CMSC 22 (Object-Oriented Programming). The application provides an interactive Java Swing-based GUI for users to browse, select, and rent various types of bicycles. The core goal is to demonstrate key OOP principles, including Inheritance, Polymorphism, and Encapsulation, through a practical, real-world scenario.

The system handles the entire rental lifecycle, from viewing inventory stock to generating a detailed receipt.

[ADD SCREENSHOT HERE: Image of Main Application Screenshot (e.g., screenshots/main_inventory.png)]

✨ Key Features

This project implements the following core functionalities:

1. Interactive GUI using Java Swing

Main Display: Automatically shows available bikes with their name, photo, hourly rate, and availability status.

Filtering & Sorting: Options to organize inventory (e.g., by price or bike type).

Details View: A "View Details" option to read a full description of any bike.

2. Robust Rental System

Cart Management: Allows users to add multiple bikes to a session's cart, adjust quantities/hours, and remove items.

Input Validation: Prevents users from renting more bikes than the available stock.

Cost Calculation: Calculates the total cost using the formula:


$$\text{Total Rate} = \text{Number of Hours} \times \text{Rate per Hour}$$

Rental Tracking: Decrements the available stock count upon successful checkout.

3. Inventory Management (Backend)

Bike Hierarchy: Uses an abstract Bike class and subclasses (e.g., EBike, MountainBike) to handle different bike models and rates (Polymorphism).

Stock Tracking: Maintains the current quantity for each bike model.

4. Receipt Generation

Upon checkout confirmation, the system generates a virtual receipt containing:

Renter's Name and Contact Number.

A line-item list of rented bikes, including hours, unit cost, and subtotal.

The final total cost of the rental session.

💻 Project Structure

The project is organized into several key classes to ensure clean separation of concerns.

Class/Package

Purpose

Bike (Abstract)

Base class for all bike types, defining common attributes and the getTotalPrice() method.

EBike, MountainBike, etc.

Concrete subclasses extending Bike and providing specific details (model, description).

BikeInventoryItem

Links a Bike type to its current stock quantity and image file path.

RentalCartItem

Represents a single line item in the user's cart (Bike type, hours, quantity).

RentalService

The central logic handler. Manages the main inventory, processes rental transactions, and handles validation.

Customer

Stores the renter's details (Name, Contact Number) for receipt generation.

GUI Package (e.g., MainFrame, InventoryPanel, CartPanel)

Contains all Java Swing classes responsible for the interactive user interface.

🛠️ Technologies Used

Technology

Role

Java Development Kit (JDK) 8+

Primary language and environment.

Java Swing

Used for building the interactive and user-friendly Graphical User Interface (GUI).

Object-Oriented Programming (OOP)

The foundational methodology used to structure the code.

Data Persistence

[EDIT THIS: Specify how data is saved, e.g., Object Serialization, or File I/O (CSV/Text files)]

📂 Getting Started

Prerequisites

Ensure you have Java Development Kit (JDK) 8 or later installed on your system.

An Integrated Development Environment (IDE) such as IntelliJ IDEA or Eclipse is recommended.

Running the Application

Clone the repository:

git clone [https://github.com/YOUR_GITHUB_USERNAME/Bike-my-Type.git](https://github.com/YOUR_GITHUB_USERNAME/Bike-my-Type.git)


Navigate to the project directory.

Open the project in your IDE (e.g., import as a Maven/Gradle or simple Java project).

Compile and run the FinalProject.java file, which contains the main method.

The application should launch the main Java Swing window displaying the bike inventory.

👥 Group Members

This project was developed by the Pokpok Girls group for CMSC 22.

Name

Role/Contribution

Bacsal, Glaziela B.

[EDIT THIS: e.g., GUI Development & Interface Design]

Palma, Angelo Joachim L.

[EDIT THIS: e.g., Core Logic Implementation & Object Modeling]
