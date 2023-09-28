		Project Overview:
		-----------------




1. **Class Declaration**: ES6 introduced a new way to declare classes in JavaScript using the `class` keyword.

   ```javascript
   class Person {
     constructor(name, age) {
       this.name = name;
       this.age = age;
     }

     sayHello() {
       console.log(`Hello, my name is ${this.name}.`);
     }
   }
   ```

2. **Constructor**: The `constructor` method is a special method used for initializing object instances when a new object is created from the class.

3. **Methods**: You can define methods inside the class, and they are added to the class's prototype.

4. **Properties**: Properties (variables) can be defined within the constructor or directly on the class instance.

5. **Inheritance**: Classes can extend other classes using the `extends` keyword. This allows for creating a subclass that inherits properties and methods from a parent class.

   ```javascript
   class Student extends Person {
     constructor(name, age, studentId) {
       super(name, age); // Call the parent class constructor
       this.studentId = studentId;
     }

     study() {
       console.log(`${this.name} is studying.`);
     }
   }
   ```

6. **`super` Keyword**: The `super` keyword is used to call methods and constructors from the parent class within the subclass.

7. **Static Methods**: You can define static methods using the `static` keyword. These methods are called on the class itself, not on instances.

   ```javascript
   class MathUtil {
     static square(x) {
       return x * x;
     }
   }

   const result = MathUtil.square(5);
   ```

8. **Getter and Setter**: ES6 classes support getter and setter methods for controlling access to object properties.

   ```javascript
   class Circle {
     constructor(radius) {
       this.radius = radius;
     }

     get area() {
       return Math.PI * this.radius * this.radius;
     }

     set diameter(diameter) {
       this.radius = diameter / 2;
     }
   }
   ```

ES6 classes provide a more structured and object-oriented way to work with JavaScript, making it easier to create and manage complex data structures and application logic. They are widely used for defining and organizing reusable code in modern JavaScript applications.
