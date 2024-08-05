# Object-Oriented Programming Exercise

## Exercise Objective
Design and implement a simple system to demonstrate key object-oriented programming concepts such as interface, package/namespace, public, protected, private, method overloading, method overriding, dynamic binding, abstract classes, and UML class diagrams.

## Scenario
You are required to create a simple simulation of a pet management system. The system should manage different types of pets and their behaviors, as well as their interactions with a veterinarian.

## Instructions

1. **Define an Abstract Class `Pet`:**
   - Attributes:
     - `name` (String, private)
     - `age` (int, private)
     - `species` (String, protected)
   - Methods:
     - `getName()`: returns the name of the pet
     - `getAge()`: returns the age of the pet
     - `getSpecies()`: returns the species of the pet
     - Abstract Method `makeSound()`: returns a String representing the sound the pet makes
     - Abstract Method `eat()`: returns a String describing what the pet eats

2. **Define Subclasses of `Pet`:**
   - `Dog`:
     - Additional Attribute: `breed` (String, private)
     - Override `makeSound()`: Dogs bark
     - Override `eat()`: Dogs eat dog food
   - `Cat`:
     - Additional Attribute: `color` (String, private)
     - Override `makeSound()`: Cats meow
     - Override `eat()`: Cats eat cat food

3. **Define an Interface `Veterinarian`:**
   - Methods:
     - `getName()`: returns the name of the veterinarian
     - `examinePet(Pet pet)`: examines the pet and returns a String describing the examination

4. **Define Implementations of the `Veterinarian` Interface:**
   - `GeneralVeterinarian`:
     - Attributes: `name` (String, private)
     - Implement Methods:
       - `getName()`: returns the name of the veterinarian
       - `examinePet(Pet pet)`: returns a String describing the general examination of the pet
   - `SpecialistVeterinarian`:
     - Additional Attribute: `specialty` (String, private)
     - Override `examinePet(Pet pet)`: returns a String describing the specialized examination of the pet

5. **Define the Main Class `PetClinic`:**
   - Methods:
     - `main(String[] args)`: Create instances of pets and veterinarians, and demonstrate the examination process, displaying the pets and their examinations. Use lists to manage the pets and display them.

## UML Class Diagram

Refer to the [PlantUML diagram](../images/oop-version1.png).

## Submission
1. Upload your code to a public repository on GitHub.
2. Ensure your code is well-documented with comments explaining key parts.
3. Create a test case in the `main` method of the `PetClinic` class to demonstrate the functionality.
4. Submit the GitHub repository link.

---

This exercise is designed to evaluate your understanding and implementation of object-oriented programming concepts. Good luck!
