# ⚡ Electricity Billing System

A menu-driven electricity billing application developed using Python. It uses Object-Oriented Programming (OOP), inheritance, and file handling to manage customer records and calculate electricity bills.

## ✨ Features

- **Add Customer:** Register customers with a unique customer ID, name, and electricity consumption.
- **View All Customers:** Display stored customer records and their electricity bills.
- **Search Customer:** Find a customer using their ID.
- **Delete Customer:** Remove a customer's record from the system.
- **Automatic Bill Calculation:** Calculate energy charges, fixed charges, and electricity duty.
- **File Handling:** Store customer information persistently in a text file.
- **Duplicate ID Prevention:** Prevent registration when a customer ID already exists.
- **Formatted Bill Display:** Present customer details and billing information in a structured format.

## 🛠️ Technologies Used

- **Python 3**
- **Object-Oriented Programming**
- **Inheritance**
- **File Handling**
- **Conditional Statements**

## 🧮 Electricity Bill Calculation

The program calculates energy charges using the following slab-based tariff:

| Electricity Consumption | Rate |
|---|---:|
| First 100 units | ₹1 per unit |
| Next 100 units | ₹2 per unit |
| Above 200 units | ₹3 per unit |

A fixed charge of ₹50 and electricity duty of 5% of the energy charges are added to the bill.

**Formula:**

```text
Total Bill = Energy Charges + Fixed Charges + Electricity Duty

Electricity Duty = 5% × Energy Charges

Fixed Charges = ₹50
```

**Example:** For 250 units consumed:

```text
First 100 units  = 100 × ₹1 = ₹100
Next 100 units   = 100 × ₹2 = ₹200
Remaining 50     =  50 × ₹3 = ₹150

Energy Charges   = ₹450
Fixed Charges    = ₹50
Electricity Duty = ₹22.50

Total Bill       = ₹522.50
```

## 🚀 Getting Started

### Prerequisites

Install Python 3 on your computer.

### Installation

1. Clone this repository:

   ```bash
   git clone Electricity-billing-system
   ```

2. Navigate to the project directory:

   ```bash
   cd Electricity-Billing-System
   ```

3. Run the Python program:

   ```bash
   python electricity_billing.py
   ```

   Replace `electricity_billing.py` with your actual Python filename.

No external libraries are required.

## 💻 Usage

After running the program, choose an option from the menu:

```text
============================================================
*****************ELECTRICITY BILLING SYSTEM*****************
============================================================
What would you like to choose?
1.Add Customer
2.View All
3.Search
4.Delete
5.Exit
```

Enter the corresponding number to perform an operation.

- **Option 1:** Add a new customer.
- **Option 2:** View all customer records and their bills.
- **Option 3:** Search for a customer by ID.
- **Option 4:** Delete a customer record.
- **Option 5:** Exit the application.

## 📁 Project Structure

```text
Electricity-Billing-System/
│
├── electricity_billing.py   # Main Python application
├── customers.txt            # Customer records, created when data is saved
└── README.md                # Project documentation
```

The `customers.txt` file stores records in a pipe-separated format:

```text
CustomerID|CustomerName|UnitsConsumed|TotalBill
```

Each customer occupies one line in the file.

## 🧠 Concepts Demonstrated

- **Classes and Objects:** Represent customers and the billing system.
- **Inheritance:** The `Customer` class inherits from the `Person` class.
- **Constructors:** Initialize customer details and calculate bills.
- **Method Overriding:** The `Customer` class provides its own `display()` method.
- **File Handling:** Read, append, and rewrite customer records.
- **Conditional Logic:** Apply different electricity rates based on consumption.
- **CRUD Operations:** Create, read, search, and delete customer records.

## 🔮 Possible Future Improvements

- Add input validation for customer IDs and electricity consumption.
- Implement customer record updates.
- Generate downloadable bills as PDF files.
- Add a graphical user interface.
- Introduce database integration for improved record management.
- Add support for configurable electricity tariff rates.

## 👩‍💻 Author

**NATARAJA SUNDARI K S**

## 📄 License

This project is available for educational purposes.
