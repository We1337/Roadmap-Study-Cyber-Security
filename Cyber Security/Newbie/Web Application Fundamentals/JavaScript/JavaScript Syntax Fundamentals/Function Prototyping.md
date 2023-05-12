Function prototyping in JavaScript is a way of adding properties and methods to a function object. This allows you to define a function's properties and methods separately from the function definition itself.

In JavaScript, all functions are objects, and like any other object, they can have properties and methods. The prototype property is an object that is shared among all instances of a function. You can use the prototype property to add new properties and methods to a function's instances.

Here is an example of function prototyping in JavaScript:

```javascript
// Define the function constructor
function Person(name, age) {
  this.name = name;
  this.age = age;
}

// Add a method to the Person prototype
Person.prototype.sayHello = function() {
  console.log("Hello, my name is " + this.name);
};

// Create a new instance of the Person object
var person = new Person("John", 30);

// Call the sayHello method on the person instance
person.sayHello(); // Output: "Hello, my name is John"
```

In this example, we define a function constructor for a `Person` object, which takes two parameters: `name` and `age`. We then add a method to the `Person` prototype called `sayHello`, which logs a message to the console.

We then create a new instance of the `Person` object using the `new` keyword, passing in values for the `name` and `age` parameters. Finally, we call the `sayHello` method on the `person` instance, which logs the message to the console.

By adding methods to a function's prototype, you can avoid duplicating the same code for each instance of the function. This can help to reduce memory usage and improve performance in your JavaScript applications.