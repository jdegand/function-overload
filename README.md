# Function Overload

[Angular Challenges](https://github.com/tomalaforge/angular-challenges) #15 Overload Function solution.

## Directions

### Information

Angular uses TypeScript, and mastering TypeScript can help you avoid runtime errors by catching them at compile time.

In this challenge, we have a function to create a vehicle. However, each vehicle type requires different mandatory properties.
Currently, we are getting an error at runtime if one property is missing and we don't get the return Type, which is not ideal.
One solution would be to create a separate function for each vehicle type, but for this challenge, I want to use the same function and have TypeScript automatically complete the properties depending on the type passed as the first parameter.

To achieve this, we will use overload functions.

### Statement

- Use function overload

## Built With

- [Angular](https://angular.io)
- [Angular CLI](https://github.com/angular/angular-cli) version 16.2.0.

## Thoughts

- `isPublicTransport property is missing for type bus` - Initial error when first running the app.
- Definitely, a weird challenge where you still end up with an error being thrown.  No way to make the bus variable actually return a Bus object.  
- The coder mixed up the bus and boat signatures.
- Now, at least you get the error before runtime.    
- First thought was to copy the function signature and change return type to all the different kinds of vehicles.
- Then I played with the parameters until I ran into errors with required and optional parameters. 
- You can't have required parameters come after an optional parameter.  
- I used undefined to get around this on the Bus & Boat signatures. 
- Thomas' solution combined fuel & capacity.  I took the approach where no other code besides signatures was to be changed. 
- I originally thought the challenge solution would have no errors and the code would compile. 
- Most general function signature has to be last.  

## Useful Resources

- [Medium](https://medium.com/ngconf/function-overloading-in-typescript-8236706b2c05) - Thomas' function overloading article
- [Typescript Lang](https://www.typescriptlang.org/docs/handbook/2/functions.html) - functions
- [Tutorials Teacher](https://www.tutorialsteacher.com/typescript/function-overloading) - function overloading
- [Stack Overflow](https://stackoverflow.com/questions/39407311/typescript-class-overload-signature-is-not-compatible-with-function-implementa) - typescript class overload signature is not compatible with function implementation

