# Object-Oriented Programming Exercise

## Exercise Objective
Design and implement a simple system to demonstrate key object-oriented programming concepts such as interface, package/namespace, public, protected, private, method overloading, method overriding, dynamic binding, abstract classes, and UML class diagrams.

## Scenario
You are required to create a simple simulation of a bookstore system. The system should manage books and customers, with different types of books and customers having unique behaviors and attributes.

## Instructions

1. **Define an Abstract Class `Book`:**
   - Attributes:
     - `title` (String, private)
     - `author` (String, private)
     - `price` (double, protected)
   - Methods:
     - `getTitle()`: returns the title of the book
     - `getAuthor()`: returns the author of the book
     - `getPrice()`: returns the price of the book
     - Abstract Method `calculateDiscount()`: returns a double representing the discount on the book

2. **Define Subclasses of `Book`:**
   - `FictionBook`:
     - Additional Attribute: `genre` (String, private)
     - Override `calculateDiscount()`: Fiction books have a 10% discount
   - `NonFictionBook`:
     - Additional Attribute: `subject` (String, private)
     - Override `calculateDiscount()`: Non-fiction books have a 5% discount

3. **Define an Interface `Customer`:**
   - Methods:
     - `getName()`: returns the name of the customer
     - `buyBook(Book book)`: processes the purchase of a book
     - `getPurchasedBooks()`: returns a list of books purchased by the customer

4. **Define Implementations of the `Customer` Interface:**
   - `RegularCustomer`:
     - Attributes: `name` (String, private)
     - Implement Methods:
       - `getName()`: returns the name of the customer
       - `buyBook(Book book)`: adds the book to the customer's purchased books
       - `getPurchasedBooks()`: returns the list of purchased books
   - `PremiumCustomer`:
     - Additional Attribute: `membershipId` (String, private)
     - Override `buyBook(Book book)`: Premium customers get an additional 5% discount on all books

5. **Define the Main Class `Bookstore`:**
   - Methods:
     - `main(String[] args)`: Create instances of books and customers, and demonstrate the purchasing process, displaying the books and their discounts.

## UML Class Diagram

Refer to the [PlantUML diagram](../images/oop-version3.png).

## Submission
1. Upload your code to a public repository on GitHub.
2. Ensure your code is well-documented with comments explaining key parts.
3. Create a test case in the `main` method of the `Bookstore` class to demonstrate the functionality.
4. Submit the GitHub repository link.

---

This exercise is designed to evaluate your understanding and implementation of object-oriented programming concepts. Good luck!

