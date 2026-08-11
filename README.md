# 💊 Pharmacy Management System

A simple **Pharmacy Management System built using Java** to demonstrate core Object-Oriented Programming (OOP) concepts such as **interfaces, inheritance, encapsulation, polymorphism, and method overriding**.

## 📌 Project Overview

This project allows users to:

* View available medicines and their details
* Search for a medicine by name
* Purchase medicines
* Manage medicine stock
* Handle prescription and non-prescription purchases
* Generate bills based on the quantity purchased
* Apply discounts for bulk purchases

The project is designed as a console-based Java application and is suitable for learning and demonstrating basic OOP concepts.

## 🛠️ Technologies Used

* **Java**
* **Java Scanner** for user input
* Object-Oriented Programming (OOP)

## 🧩 OOP Concepts Demonstrated

### 1. Interface

The `Pharmacy` interface defines the `stockManagement()` method:

```java
interface Pharmacy {
    int stockManagement();
}
```

### 2. Encapsulation

The `Medicine` class uses private fields with getter methods to control access to medicine information.

```java
private String medicineId;
private String medicineName;
private double price;
private String type;
```

### 3. Inheritance

The project uses multiple levels of inheritance:

```text
Medicine
   |
   +-- Info
   |
   +-- Buy
        |
        +-- Prescription
        |
        +-- WithoutPrescription
        |
        +-- BillMake
```

### 4. Polymorphism

Methods such as `stockManagement()` and `showDetail()` are overridden in subclasses to provide different behavior.

### 5. Method Overriding

For example:

```java
@Override
public int stockManagement() {
    // Purchase and stock management logic
}
```

## 💊 Sample Medicines

The system contains sample medicines such as:

| Medicine ID | Medicine     | Stock |    Price | Type      |
| ----------- | ------------ | ----: | -------: | --------- |
| M0034       | Sertraline   |   150 |   Rs. 60 | Tablet    |
| M0035       | Metformin    |   100 | Rs. 1000 | Tablet    |
| M0036       | Zolpidem     |    10 |  Rs. 500 | Injection |
| M0134       | Insulin      |   200 |  Rs. 600 | Tablet    |
| M0074       | Phenytoin    |   157 |   Rs. 50 | Tablet    |
| M0044       | Morphine     |   180 |  Rs. 100 | Liquid    |
| M0050       | Isotretinoin |    30 |  Rs. 680 | Tablet    |
| M0654       | Prednisolone |   800 |  Rs. 840 | Liquid    |
| M0844       | Diazepam     |   600 |  Rs. 640 | Tablet    |
| M0010       | Fluoxetine   |   300 |  Rs. 560 | Liquid    |

## 🧾 Billing System

The system calculates the total bill according to the number of units purchased.

### Discount Rules

|      Quantity |    Discount |
| ------------: | ----------: |
|          1–10 | No discount |
|        11–100 |         10% |
| More than 100 |         25% |

For example:

```text
Quantity: 20
Price per unit: Rs. 100

Subtotal = Rs. 2000
Discount = 10%
Total = Rs. 1800
```

## ▶️ How to Run

### Prerequisites

Make sure you have Java installed on your computer.

Check your Java version:

```bash
java -version
```

### Clone the Repository

```bash
git clone https://github.com/your-username/pharmacy-management-system.git
```

Move into the project directory:

```bash
cd pharmacy-management-system
```

### Compile

```bash
javac Main.java
```

### Run

```bash
java Main
```

## 🖥️ Example

When the program starts:

```text
================ WELCOME TO PHARMACY SYSTEM ================
What do you want?
1. Show available medicine details
2. Buy medicine
Choose an option:
```

### View Medicine Details

Select:

```text
1
```

The program displays the available medicines, including:

```text
====== MEDICINE INFO ======
Medicine ID    : M0034
Medicine Name  : Sertraline
Price          : Rs. 60.0
Stock Count    : 150
Type           : Tablet
---------------------------
```

### Buy Medicine

Select:

```text
2
```

Then enter the medicine name and quantity:

```text
Enter medicine name: Sertraline
How many units? 5
Is prescription required? (true/false): false
```

The system processes the purchase and displays the bill.

## 📁 Project Structure

```text
Pharmacy-Management-System/
│
├── Main.java
└── README.md
```

The main Java file contains the following classes:

```text
Pharmacy
   │
   └── Medicine
        │
        ├── Info
        │
        └── Buy
             ├── Prescription
             ├── WithoutPrescription
             └── BillMake
```

## 🎯 Learning Objectives

This project was created to practice:

* Java classes and objects
* Interfaces
* Inheritance
* Encapsulation
* Polymorphism
* Method overriding
* Constructors
* Access modifiers
* Arrays of objects
* User input using `Scanner`
* Conditional statements
* Basic billing calculations

## 🚀 Future Improvements

Possible improvements include:

* Add a graphical user interface (GUI)
* Store medicines in a database
* Add medicine search by ID
* Add login/authentication
* Add an admin panel
* Add expiry-date management
* Add automatic prescription validation
* Add customer records
* Generate printable invoices
* Improve stock management
* Add exception handling and input validation

## 👨‍💻 Author

**Your Name**

This project was developed as a Java OOP learning project.

## 📄 License

This project is available for educational purposes. You are free to modify and improve it for learning and personal projects.

GitHub profile:https://github.com/Saranja6<br>
Linkedin Profile:https://www.linkedin.com/in/saranja-jeyaradnarajah-94a8353ba?utm_source=share_via&utm_content=profile&utm_medium=member_android
