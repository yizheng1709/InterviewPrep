# Common JavaScript Interview Questions

## Table of Contents

- [What is event delegation](#what-is-event-delegation)
- [Describe event bubbling](#describe-event-bubbling)
- [Explain how prototypal inheritance works](#explain-how-prototypal-inheritance-works)
- [What is the difference between a variable that is: `null`, `undefined` or `undeclared`?](#what-is-the-difference-between-a-variable-that-is-null-undefined-or-undeclared)
- [What is a closure, and how/why would you use one?](#what-is-a-closure-and-howwhy-would-you-use-one)
- [Can you describe the main difference between the `Array.forEach()` loop and `Array.map()` methods and why you would pick one versus the other?](#can-you-describe-the-main-difference-between-the-arrayforeach-loop-and-arraymap-methods-and-why-you-would-pick-one-versus-the-other)
- [What's a typical use case for anonymous functions?](#what-is-a-typical-use-case-for-anonymous-functions)
- [What's the difference between host objects and native objects?](#what-is-the-difference-between-host-objects-and-native-objects)
- []()
- []()
- []()

## What is event delegation?

Event delegation in JavaScript is a technique where you attach a single event handler to a parent element instead of individual handlers to its child elements. The event "bubbles" up from the child to the parent, triggering the handler. It helps handle events efficiently, especially for dynamic or numerous elements, reducing memory usage and improving performance.

## Describe event bubbling

Event bubbling is a mechanism in JavaScript where an event triggered on a specific element will also trigger the same event on its parent elements, propagating upwards through the DOM tree. During event bubbling, the event starts from the innermost element and propagates through its ancestors up to the root of the document. This allows parent elements to "listen" and potentially handle the event even if the event was initially triggered on a nested child element.

## Explain how prototypal inheritance works

Prototypal inheritance in JavaScript allows objects to inherit properties and behavior from other objects. Each object has an internal `Prototype` link that points to its prototype object. When accessing a property or method on an object, JavaScript looks for it in the object itself, and if not found, it continues searching up the prototype chain until the property is found or until it reaches the end of the chain (null prototype). This mechanism promotes code reuse and enables objects to share common functionality.

## What is the difference between a variable that is: null, undefined or undeclared?

`null`: It is a value assigned to a variable explicitly to indicate the absence of an object or empty value. It is a valid value in JavaScript and needs to be assigned explicitly.

`undefined`: It indicates that a variable has been declared but has not been assigned a value. It is the default value of variables that are declared but not initialized. It is a built-in value in JavaScript.

`undeclared`: It refers to a variable that has been referenced without being declared using the var, let, or const keyword. It results in a ReferenceError when trying to access an undeclared variable.

In summary, `null` is an assigned value indicating the absence of an object, `undefined` is the default value for uninitialized variables, and `undeclared` variables are those that have not been declared at all.

## What is a closure, and how/why would you use one?

A closure is a combination of a function and the lexical environment in which it was declared. It allows a function to access variables from its outer scope even after the function has finished executing. Closures are useful for creating private variables, encapsulation, maintaining state, and handling callbacks and asynchronous operations effectively.

## Can you describe the main difference between the `Array.forEach()` loop and `Array.map()` methods and why you would pick one versus the other?

The main difference between `Array.forEach()` and `Array.map()` methods is in their return values and the purpose they serve.

`Array.forEach()` is used when you want to iterate over each item in an array and perform some action or operation on it. It does not return a new array; instead, it executes a callback function for each item in the array.

`Array.map()`, on the other hand, is used when you want to transform each item in an array and create a new array based on the transformation. It returns a new array by applying a callback function to each item in the original array.

## What is a typical use case for anonymous functions?

A typical use case for anonymous functions is when you need a function for a specific task that doesn't require reusability or naming. Anonymous functions are commonly used in scenarios such as: callback functions, immediately invoked function expressions, event handlers, and function arguments.

## What is the difference between host objects and native objects?

Host objects are provided by the environment (e.g., web browser) and are not defined by the JavaScript language. Examples include window and DOM elements. Native objects, on the other hand, are built-in objects defined by the JavaScript language specification, such as Array and String. Host objects have environment-specific behavior, while native objects provide consistent functionality across JavaScript environments.

## Can you explain what `Function.call` and `Function.apply` do?

`Function.call`: It invokes a function by specifying the this value and passing arguments individually. The first argument of call is the value to be assigned to this, followed by the individual arguments to be passed to the function.

`Function.apply`: It invokes a function by specifying the this value and passing arguments as an array or an array-like object. The first argument of apply is the value to be assigned to this, and the second argument is an array or array-like object containing the arguments to be passed to the function.

The notable difference between `call` and `apply` lies in how the arguments are passed to the function. With call, the arguments are passed individually, while with apply, they are passed as an array or array-like object.

## Explain `Function.prototype.bind`.

`Function.prototype.bind` creates a new function with a specified this value and partially applied arguments, allowing for deferred execution and convenient customization of function invocation.

## What is the difference between feature detection, feature inference, and using the UA string?

Feature detection is a reliable technique that directly tests for the presence of specific features, while feature inference makes assumptions based on related features. Using the UA string involves extracting information from the client's browser and operating system, but it can be less accurate and prone to manipulation.

## Explain "hoisting"

Hoisting is a JavaScript behavior where variable and function declarations are moved to the top of their containing scope during the compilation phase, before the code is executed. This means that you can use variables and invoke functions before they are actually declared in the code. However, only the declarations are hoisted, not the initializations or assignments. It's important to note that hoisting applies to both variables declared with `var` and functions declared with the `function` keyword.

## What's the difference between an "attribute" and a "property"?

Attribute: An attribute is a value specified in HTML markup and defines initial or additional information about an HTML element. It is defined in the HTML source code and accessed using methods like `getAttribute()`.

Property: A property is a value associated with a JavaScript object representing an HTML element. It represents the current state or value of the element and can be accessed and manipulated through JavaScript code.

## What are the pros and cons of extending built-in JavaScript objects?

While extending built-in JavaScript objects can provide convenience and code reusability, it comes with the risks of naming collisions, decreased code maintainability, and potential compatibility issues. Careful consideration and cautious use of extensions are necessary to mitigate these drawbacks.

## What is the difference between `==` and `===`?

`==` is an equality operator that performs type coercion, allowing comparison between values of different types by converting them to a common type. On the other hand, `===` is a strict equality operator that compares values without type coercion, requiring both the value and the type to be the same for the comparison to be true.

## Explain the same-origin policy with regards to JavaScript

The same-origin policy is a security feature in web browsers that restricts JavaScript code from accessing resources (such as data or methods) on a different domain, port, or protocol. It ensures that scripts on one origin (combination of domain, port, and protocol) cannot access or interact with content from another origin. This policy helps prevent cross-site scripting (XSS) attacks and protects user data and privacy by enforcing a boundary between different origins.

## What is strict mode? What are some of the advantages/disadvantages of using it?

Strict mode offers benefits such as improved error handling, cleaner code, enhanced security, and future compatibility. However, it can introduce compatibility issues with older environments and may require adjustments to existing code.

## What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?

Using a language that compiles to JavaScript can provide enhanced language features, improved productivity, cross-platform compatibility, and performance optimizations. However, it may come with a learning curve, debugging limitations, compatibility challenges, and increased build complexity.

## Explain the difference between mutable and immutable objects

Mutable objects: Mutable objects are objects whose state can be changed after they are created. This means that properties and values of mutable objects can be modified, added, or removed throughout the program execution.

Immutable objects: Immutable objects, on the other hand, are objects whose state cannot be changed once they are created. This means that once an immutable object is created, its properties and values remain fixed and cannot be modified.

## What are the pros and cons of immutability?

Immutability offers benefits such as predictability, simplified code, thread safety, and potential performance optimizations. However, it can introduce memory overhead, performance impact, and object creation overhead.

## Explain the difference between synchronous and asynchronous functions

The key difference between synchronous and asynchronous functions is how they handle the flow of execution. Synchronous functions execute sequentially, while asynchronous functions initiate tasks and continue with other operations without waiting for the task to finish.

## What is event loop? What is the difference between call stack and task queue?

The event loop continuously checks the call stack and task queue. It executes tasks from the task queue when the call stack is empty, ensuring the proper handling of asynchronous operations and maintaining the responsiveness of the program. The call stack manages the execution context of synchronous code, while the task queue holds tasks/callbacks associated with asynchronous operations.

## What are the differences between variables created using `let`, `var` or `const`?

`var` has function or global scope, can be redeclared, and is hoisted. `let` and `const` have block scope, cannot be redeclared within the same scope, and are not hoisted. The difference between `let` and `const` is that `let` allows reassignment of values, while `const` variables are constant and cannot be reassigned.

## What is the definition of a higher-order function?

A higher-order function is a function that takes one or more functions as arguments or returns a function as its result. It operates on functions, treating them as first-class citizens. Higher-order functions enable powerful functional programming techniques such as function composition, currying, and abstraction of control flow. They provide flexibility and modularity in code by allowing functions to be dynamically created and manipulated.

## What is a Promise?

A Promise is an object in JavaScript that represents the eventual completion (or failure) of an asynchronous operation and its resulting value. It is a way to handle asynchronous operations in a more organized and manageable manner.

## Discuss how you might use Object Oriented Programming principles when coding with JavaScript

Object-Oriented Programming (OOP) principles can be applied in JavaScript to achieve code organization, reusability, and maintainability. Here's how you might use OOP principles in JavaScript:

Encapsulation: Use objects to encapsulate related data and behavior together. Group related properties and functions into objects, allowing you to create reusable and modular code.

Inheritance: Utilize prototypal inheritance to create hierarchical relationships between objects. Inherit properties and methods from a parent object to a child object, promoting code reuse and providing a structured way to extend functionality.

Polymorphism: Leverage the flexibility of JavaScript's dynamic typing to achieve polymorphism. Objects can have different forms (e.g., different objects implementing the same interface) and can respond to the same method calls in different ways.

Abstraction: Abstract away complex implementation details by exposing a simplified interface. Hide internal implementation details and provide public methods that allow users to interact with objects without needing to understand their internal workings.

Composition: Compose objects by combining smaller, more focused objects to create larger, more complex objects. This promotes code reuse and modularity, allowing you to build systems with interchangeable and interchangeable parts.

By applying OOP principles, you can create more structured, modular, and reusable code in JavaScript. It promotes code organization, encapsulation, and abstraction, allowing you to build complex systems in a more maintainable and scalable way.
