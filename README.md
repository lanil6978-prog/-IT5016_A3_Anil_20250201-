# -IT5016_A3_Anil_20250201-
It includes my own codes as well as my practiced example.
It is Python Requisition System program. It enables the staff members to make requisitions of what they require, key in the price of each item, add the sum of cost and count the approval according to the sum. Granting of requisitions that have cost below 500 is automatically granted whereas larger requisitions are awaited and given a specific reference number. 
The system is an example of Object-Oriented Programming (OOP) in which a class named RequisitionSystem is used. Every requisition is stored as an object with its own data which includes the name of the staff, the date, requisition number, the sum of cost, and the approval status. Shared class variables such as requisition counter and all requisitions are used to ensure that the unique IDs are handled and all the requisitions are shared in a single list, across all the objects. Instance variables are specific to a particular requisition and carry information that is specific to a request.
Features and Workflow
The user is asked to provide the number of requisitions staff wishes to make.
For each requisition 
The information about the staff (name, staff ID and date) is gathered. The user takes different items and their respective costs. The system is used to calculate the total cost. All the requisitions that are below 500 are automatically approved, those that exceed this are pending and given a reference number. The system also lists all requisitions and contains such information as requisition ID, staff name, total cost, approval status, and reference number. General statistics are presented and they will indicate the number of approved, pending and not approved requisitions.
Software development principle
Object and Oriented Programming (OOP):
 The program has classes and objects to systemize the program in an orderly manner and it is easy to handle numerous requisitions. The requisitions are distinct objects. 
 Single Responsibility Principle (SRP):
 There is one, evident duty of each of the methods: 
staff_info(): gets staff information. 
requisitions_total(): calculate the cost of items. 
requisition_approval(): checks requisition and udapted approval to pending, approved and not approved.
display_requisition():  prints all requisition.
requisition_statistics(): calculates all requisition and display the requistion 
DRY (Don’t Repeat Yourself):
Repeating the code is avoided through the use of loops and reusable methods. As an illustration, all requisitions have one reusable method of item input and cost calculation.
Separation of Concerns:
The program has separated the responsibilities: the collection of inputs, the business logic, display, and statistics are all addressed with specific methods, which makes the code more convenient to debug and expand.
KISS (Keep It Simple Stupid):
Code is simple and avoids unnecessary complexity.
Open / Closed Principle:
Extra features can be added to the class (e.g. new approval rules) without changing the current methods.
Suggestions for Improvement:
The program can be improved in numerous ways in the future. An example is that the program may it may be enhanced by a graphical user interface or a simple web application so that users could interact with the system easily rather than using command-line input only. They could also install an authentication system so that only registered staff members would be able to create requisitions. Approval may take several levels based on the cost, which may be approval of line managers or approval of finance department. It is also possible to change the system to accept cost  in a decimal number form to make the system more realistic. Lastly, unit tests might be included to evaluate the program to be in place under various circumstances.
