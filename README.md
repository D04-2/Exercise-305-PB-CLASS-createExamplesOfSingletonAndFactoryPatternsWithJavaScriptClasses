# Create examples of Singleton and Factory patterns with JavaScript Classes

Use your knowledge of JavaScript classes and OOP to create an example of the Singleton and Factory patterns.

## 1. Singleton Pattern

### 1.2. Create a simple singleton pattern

- Create a class called `Customers` which has a constructor with no parameters
- Make the constructor load an array of customer objects into a property called `customers`
- Make a `list()` method which displays all customers in the array
- Instantiate the class once as a variable `customers` and once as a variable `custs`
- Show that the data in the constructor is executed twice
- Implement a Singleton pattern
- Show that the data in the constructor is executed once, even though it the class instantiated two objects

### 1.3. Challenge :muscle:
  
- Copy the above solution and extend it to fetch actual data from [this Northwind customer JSON file](https://raw.githubusercontent.com/graphql-compose/graphql-compose-examples/master/examples/northwind/data/json/customers.json)
- Implement `async/await` so that the method `list()` waits until the data in the constructor is loaded asynchronously
- see [Two examples of OOP design patterns using JavaScript classes: Singleton and Factory](https://edwardtanguay.netlify.app/howtos?id=517) for code examples to solve this


## 2. Factory Pattern

### 2.1. Create a factory pattern to create objects

- create a parent class `ShoppingCart` with properties:
  - `products` - **array of strings**
- create a child class `MemberShoppingCart` which extends `ShoppingCart` and has addition property:
  - `memberId` - **number**
- create a child class `VipShoppingCart` which extends `ShoppingCart` and has addition property:
  - `vipId` - **string**
  - `vipDiscount` - **decimal** e.g. `.1` or `.2`
- make a factory class called `ShoppingCartFactory` which can 
  - instantiate both kinds of shopping carts
  - records which objects it has instantiated
  - has a `getReport()` method which displays which objects its instantiated
- see [Two examples of OOP design patterns using JavaScript classes: Singleton and Factory](https://edwardtanguay.netlify.app/howtos?id=517) for code examples to solve this

### 2.2. Challenge :muscle:

- Extend the above solution so that it not only stores the objects created internally, but also writes them in JSON format to a text file called `createdObjects.json`
- Hint: see [this code](https://edwardtanguay.netlify.app/howtos?id=516) for an example of how to use `fs` to write a file in Node
