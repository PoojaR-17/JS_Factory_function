# JS_Factory_function
A factory function is a function that returns a new object or instance of something, without requiring the use of the new keyword. It’s commonly used to create multiple objects of the same type while providing the flexibility to customize each one.
Key Points of a Factory Function:
No new Keyword: Unlike constructors, factory functions don’t require the new keyword.
Return Object: A factory function returns an object.
Customizable: Each object can have different properties and methods.
Encapsulation: It helps encapsulate the creation logic, making code cleaner.
# Factory Function Example

## Overview
This project demonstrates how to use a factory function in JavaScript. A factory function is a simple way to encapsulate object creation without the need for constructors or the `new` keyword.

## Factory Function: `createUser`

The `createUser` function creates a user object with the following properties:
- `name`: The name of the user.
- `role`: The role of the user (e.g., Admin, Manager).
- `greet()`: A method that returns a greeting message using the user's name and role.

### Usage

```javascript
function createUser(name, role) {
  return {
    name: name,
    role: role,
    greet: function() {
      return `Hello, ${this.name}! You are logged in as a ${this.role}.`;
    }
  };
}

const user1 = createUser("Pooja", "Admin");
console.log(user1.greet());  // Output: Hello, Pooja! You are logged in as a Admin.
Benefits of Factory Functions:
No need to use new.
Easier to create customized objects.
Clear and modular code structure.
