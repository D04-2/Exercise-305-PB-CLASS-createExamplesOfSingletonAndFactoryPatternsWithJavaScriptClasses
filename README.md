# Create examples of Singleton and Factory patterns with JavaScript Classes

Use your knowledge of JavaScript classes and OOP to create an example of the Singleton and Factory patterns.

## Singleton Pattern

- Create a class called `Customers` which has a constructor with no parameters
- Make the constructor load an array of customer objects into a property called `customers`
- Make a `list()` method which displays all customers in the array
- Instantiate the class once as a variable `customers` and once as a variable `custs`
- Show that the data in the constructor is executed twice
- Implement a Singleton pattern
- Show that the data in the constructor is executed once, even though it the class instantiated two objects

### Challenge :muscle:
  
- Use fetch to load actual data from [this Northwind customer JSON file](https://raw.githubusercontent.com/graphql-compose/graphql-compose-examples/master/examples/northwind/data/json/customers.json)
- Implement `async/await` so that the method `list()` waits until the data in the constructor is loaded asynchronously
- see [Two examples of OOP design patterns using JavaScript classes: Singleton and Factory](https://edwardtanguay.netlify.app/howtos?id=517) for code examples to solve this


## Factory Pattern
