# Object-Oriented Programming Exercise

## Exercise Objective
Design and implement a simple system to demonstrate key object-oriented programming concepts such as interface, package/namespace, public, protected, private, method overloading, method overriding, dynamic binding, abstract classes, and UML class diagrams.

## Scenario
You are required to create a simple simulation of an e-commerce system. The system should manage different types of products and users, as well as their respective behaviors and interactions.

## Instructions

1. **Define an Abstract Class `Product`:**
   - Attributes:
     - `productId` (String, private)
     - `name` (String, private)
     - `price` (double, protected)
   - Methods:
     - `getProductId()`: returns the product ID
     - `getName()`: returns the name of the product
     - `getPrice()`: returns the price of the product
     - Abstract Method `getDescription()`: returns a String describing the product

2. **Define Subclasses of `Product`:**
   - `Electronics`:
     - Additional Attribute: `warrantyPeriod` (int, private)
     - Override `getDescription()`: Returns a description including the warranty period
   - `Clothing`:
     - Additional Attribute: `size` (String, private)
     - Override `getDescription()`: Returns a description including the size

3. **Define an Interface `User`:**
   - Methods:
     - `getUsername()`: returns the username of the user
     - `addProductToCart(Product product)`: adds a product to the user's cart
     - `getCartContents()`: returns a list of products in the user's cart

4. **Define Implementations of the `User` Interface:**
   - `RegularUser`:
     - Attributes: `username` (String, private)
     - Implement Methods:
       - `getUsername()`: returns the username of the user
       - `addProductToCart(Product product)`: adds the product to the user's cart
       - `getCartContents()`: returns the list of products in the cart
   - `PremiumUser`:
     - Additional Attribute: `membershipLevel` (String, private)
     - Override `addProductToCart(Product product)`: Premium users get a discount on all products added to the cart

5. **Define the Main Class `ECommerceSystem`:**
   - Methods:
     - `main(String[] args)`: Create instances of products and users, and demonstrate the process of adding products to the cart, displaying the cart contents and product descriptions. Use lists to manage the cart contents and display them.

## UML Class Diagram

Refer to the [PlantUML diagram](../images/oop-version5.png).

## Submission
1. Upload your code to a public repository on GitHub.
2. Ensure your code is well-documented with comments explaining key parts.
3. Create a test case in the `main` method of the `ECommerceSystem` class to demonstrate the functionality.
4. Submit the GitHub repository link.

---

This exercise is designed to evaluate your understanding and implementation of object-oriented programming concepts. Good luck!
