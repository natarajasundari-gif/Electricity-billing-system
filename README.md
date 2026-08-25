Electricity Billing SystemA CLI-based Python application that manages customer records and calculates electricity bills using object-oriented programming concepts.
Data is stored locally in a text file.
FeaturesClass Inheritance:
      Utilizes a Person base class and a Customer derived class to encapsulate customer details and billing logic.Dynamic Bill Calculation:
      Calculates tiered energy charges, fixed charges, and electricity duty (tax).
      Data Persistence: Stores and reads customer records directly to and from a local text file (customers.txt).
CRUD Operations:
      Add Customer: Prevents duplicate Customer IDs.
      View All Records: Displays formatted billing receipts for every customer.
      Search Record: Retrieves billing information by Customer ID.
      Delete Record: Removes customer entries safely.
Bill Calculation StructureUnits ConsumedRate per UnitFirst 100 Units₹1.00 / unit101 to 200 Units₹2.00 / unitAbove 200 Units₹3.00 / unitFixed Charges:₹50.00
Electricity Duty (Tax): 5% on the calculated energy chargePrerequisitesPython 3.x installed on your system.
UsageClone or Download the repository to your local machine.Run the Script:Bashpython elctricity_billing.py
Follow the On-Screen Menu:
Plaintext
============================================================
*****************ELECTRICITY BILLING SYSTEM*****************
============================================================
What would you like to choose?
1.Add Customer
2.View All
3.Search
4.Delete
5.Exit
