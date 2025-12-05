Bike my Type: Bike Rental Management System

Group Name: Pokpok Girls (Bacsal, Glaziela B. and Palma, Angelo Joachim L.)
Course: CMSC 22 - Object-Oriented Programming
Status: In Development

Table of Contents

🚀 Overview

✨ Key Features

💻 Project Structure

🛠️ Technologies Used

📂 Getting Started

👥 Group Members

🚀 Overview

Bike my Type is a bike rental management system developed to demonstrate core principles of Object-Oriented Programming (OOP). The application provides an interactive Java Swing-based GUI that allows users to browse a diverse inventory of bikes, manage their rental selection in a cart, and complete a validated checkout process.

The system is designed to handle all aspects of a rental transaction, from initial inventory display to final receipt generation, using concepts like inheritance and polymorphism to manage different bike types.

Key Features

This project implements the following core functionalities:

1. Interactive GUI (Java Swing)

Main Display: Displays all available bike types, including their name, photo (placeholder image/icon), hourly rate, and available quantity.

User Interface: Features dedicated panels for browsing the inventory, viewing the cart, and displaying the final receipt.

Filtering & Sorting: Options to organize the inventory list (e.g., by hourly rate, category, or availability).

Details View: A "View Details" function to display the full description of a selected bike.

2. Rental and Transaction System

Cart Management: Users can add multiple bike types to their cart, specify the number of units, and select the rental duration (number of hours).

Input Validation: The system prevents the user from renting more units of a specific bike type than are currently in stock.

Cost Calculation: Total rental cost is dynamically calculated using the formula:


$$\text{Total Cost} = \sum (\text{Rate per Hour} \times \text{Number of Hours} \times \text{Quantity})$$

Inventory Update: The system decrements the available stock count immediately upon successful checkout.

3. OOP Implementation

Inheritance: An abstract Bike class defines common properties, which are extended by concrete subclasses (EBike, MountainBike, etc.).

Encapsulation: Dedicated classes like BikeInventoryItem and RentalCartItem manage stock, rates, and transaction data separately from the core UI.

4. Receipt Generation

Upon confirmation, a detailed receipt is displayed, containing:

Renter's identifying information (Name and Contact Number).

A clear line-item breakdown of each bike rented (quantity, rate, hours, and subtotal).

The final grand total cost.

Project Structure

The logical architecture separates the core business logic (inventory and rentals) from the UI presentation.

Component

Description

Bike.java (Abstract)

The base class for all rental items, defining common methods and properties.

EBike.java, MountainBike.java, etc.

Concrete bike model definitions extending Bike.

BikeInventoryItem.java

Tracks a specific Bike type's stockQuantity and long description.

RentalCartItem.java

Stores transaction details: the Bike being rented, hoursRented, and quantity selected by the user.

RentalService.java

The central service class. Manages the master inventory list, handles stock updates, and performs checkout validation.

Customer.java

Simple class to hold user input (name, contact number) during checkout.

MainGUI.java

The primary Java Swing JFrame that orchestrates all panel views (Inventory, Cart, Receipt).

Technologies Used

Technology

Role

Java Development Kit (JDK) 8+

Primary programming language.

Java Swing

Used for building the Graphical User Interface (GUI).

File I/O / Serialization

(Placeholder: Data Persistence method used to save and load inventory data between sessions.)

Getting Started

Prerequisites

Java Development Kit (JDK) 8 or later: Required to compile and run the Java source code.

Java IDE (Recommended): An IDE like IntelliJ IDEA or Eclipse simplifies project management.

Running the Application

Clone the repository:

git clone [https://github.com/YOUR_GITHUB_USERNAME/Bike-my-Type.git](https://github.com/YOUR_GITHUB_USERNAME/Bike-my-Type.git)


(Remember to replace YOUR_GITHUB_USERNAME with your actual username.)

Open the Project: Import the cloned directory into your Java IDE.

Run: Execute the main method located in FinalProject.java.

👥 Group Members

This project was completed by the Pokpok Girls group.

Name

Primary Role

Bacsal, Glaziela B.

Palma, Angelo Joachim L.
