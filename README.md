Download Link: https://assignmentchef.com/product/solved-orderprocessor
<br>



5/5 - (3 votes)

This is your first ever program using object oriented methodology. In this assignment you will need to instantiate (creat*) object(s) and invoke their instance methods to perform different tasks. The program is to keep track of customer orders and to creat* reports as needed.

At minimum you will need several objects to be instantiated throughout the program such as:

An OrderProcessor objectOrder objectsLet’s get to class design now.

Class Design:

class &lt;your choice of name: this class simply contains the public static main method just as what we’ve been programming so far in the first four assignments. You must select a descriptive name for the class based on what the program is set out to do. There will be no constructor or any instance field should be defined for this class. Sometimes people call it the “Driver” class which is the starting point of your program. Read thru the specs you will know what the main method is supposed to do. You will be amazed as to how simplified it is now for the code inside the main method.

class OrderProcessor: maintain a list of Order objects (array of Order objects)

Public static constant integer representing the &lt;size of the array of Order objects and set it to 32Private instance fields:Company nameCompany web site (<a href="http://www.xyz.com/" target="_blank" rel="nofollow noopener">www.xyz.com</a> (Links to an external site.)

Links to an external site.for example)A reference to an array of Order objects (namely orderList)Order count (the actual number of Order objects to be processed)Public constructors:Default constructor: set order count to 0. Creat* an array of &lt;size references to Objects. HINT: orderList = new ……….. // step 2 in array creationNon-default constructor: take a String for company name and a String for company web site (must set order count to 0 similar to default constructor). Creat* an array of &lt;size references to ObjectsPublic instance methods:Accessor/mutator for company name, company web site, and order countinit: Use a for loop similar to the LoadVehicle function in assignment #4 to randomly generate data for 8 Orders. An Order has the following required information: customer name, product name, product quantity, Order date, and price. See the class Order specs in the next section for more information. For example Order #1 is from customer James Anderson (customer name) which orders iPhone 7 (product name), 5 of those (product quantity), Order date is March 6, and unit price of $859.95Declare an array of Strings (size=8) for customer names and manually initialize the array with products of your choiceDeclare an array of Strings (size=8) for product names and manually initialize the array with names of your choiceRandomly generate a Product quantity for the order (values from 1-10)Randomly generate an order day (1-30 for the month of March)Randomly generate product unit price between (LO:100.00-HIGH: 1000.00)Now instantiate an Order object using the Order’s default constructor. Next call the mutators in Order object to properly initialize the current Order element: customer name , product name, quantity, order date (of March, 2017), unit price. An example of this setting is: orderList[i].setCustomerName (nameList[i]);NOTE: don’t forget to update the order count instance field to 8addOrder: ask user input for a new Order with all needed Order info and add it to the end of the array. Must use non-default constructor when instantiating the Order object. Update order count as needed. Note if the array is full you should output and error message and do not add the new Order.reportOrderDetails: list all orders with a nice format as follows. Must use the new for loop syntax to display one Order at a time. Must check for null references before output the Order’s info.Company:                                                           Web-site:

Customer     Product   Quantity      Unit Price     Order date   Total cost

class Order: represent customer order information

Private instance fields:customer nameproduct nameunit pricequantityorder date (03/xx/2017)Public constructors:Default constructor: set name to “John Doe”, product to “Unknown”, price to 0.0, quantity to 0, date to 03/01/2017Non-default constructor taking customer name, product name, price, quantity, and date as parametersPublic instance methods:Accessor/mutator for all instance fieldsBehavioral methods:orderCost: return unit price * product quantityImplementation/Coding Requirements

Must follow Google style for naming convention for class names, variable namesconstructors, instance fields, static fields, instance methods must be declared with the correct access specifiers (private or public). No specifier for those will get heavy points deductionMain Program

Instantiate a non-default OrderProcessor object (manually provide parameters for the constructor)Invoke init method for the objectInvoke reportOrderDetails methodUse a loop to add three more Orders to the OrderProcessor (data from user input using BufferedReader or Scanner). Implement a public static method for the below (then called by main) passing in the OrderProcessor object and using GUI for user input will get 5 points extra credit.for (int count =0; count &lt;3; count++) {

// invoke addOrder method from OrderProcessor object

}