# Common JavaScript Interview Questions

### What is event delegation?


Event delegation in JavaScript is a technique where you attach a single event handler to a parent element instead of individual handlers to its child elements. The event "bubbles" up from the child to the parent, triggering the handler. It helps handle events efficiently, especially for dynamic or numerous elements, reducing memory usage and improving performance.

### Explain how prototypal inheritance works.

Prototypal inheritance in JavaScript allows objects to inherit properties and behavior from other objects. Each object has an internal `Prototype` link that points to its prototype object. When accessing a property or method on an object, JavaScript looks for it in the object itself, and if not found, it continues searching up the prototype chain until the property is found or until it reaches the end of the chain (null prototype). This mechanism promotes code reuse and enables objects to share common functionality.

### What's the difference between a variable that is: `null`, `undefined` or `undeclared`?

`null`: It is a value assigned to a variable explicitly to indicate the absence of an object or empty value. It is a valid value in JavaScript and needs to be assigned explicitly.

`undefined`: It indicates that a variable has been declared but has not been assigned a value. It is the default value of variables that are declared but not initialized. It is a built-in value in JavaScript.

`undeclared`: It refers to a variable that has been referenced without being declared using the var, let, or const keyword. It results in a ReferenceError when trying to access an undeclared variable.

In summary, `null` is an assigned value indicating the absence of an object, `undefined` is the default value for uninitialized variables, and `undeclared` variables are those that have not been declared at all.

