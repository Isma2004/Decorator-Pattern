# Decorator Pattern Implementation

## **Problem:**
Need to dynamically add functionalities (like adding milk and sugar) to a base `Coffee` object without altering its structure, ensuring flexibility and scalability.

## **Solution:**
Implemented the **Decorator Pattern**, which allows attaching additional responsibilities to an object dynamically. The Decorator provides a flexible alternative to subclassing for extending functionality, adhering to the Open/Closed Principle.

### **Components:**
1. **Coffee Interface (`Coffee.java`):** Defines the core functionalities.
2. **Concrete Component (`SimpleCoffee.java`):** Implements the `Coffee` interface.
3. **Decorator Abstract Class (`CoffeeDecorator.java`):** Implements the `Coffee` interface and holds a reference to a `Coffee` object.
4. **Concrete Decorators (`MilkDecorator.java`, `SugarDecorator.java`):** Extend `CoffeeDecorator` to add specific functionalities.
5. **Main Class (`Main.java`):** Demonstrates adding decorators to a `Coffee` object dynamically.

## **Usage:**
1. **Create a Simple Coffee:** Instantiate `SimpleCoffee`.
2. **Add Milk:** Wrap the `SimpleCoffee` object with `MilkDecorator`.
3. **Add Sugar:** Further wrap the decorated coffee with `SugarDecorator`.
4. **View Descriptions and Costs:** Each decorator adds its description and cost to the coffee.
