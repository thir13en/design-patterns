# Common Patterns

### Layering
Divide the architecture into different layers where elements of the same layer take care of a certain part of the application.

#### 3 Tier
We divide the architecture into this categories:
1. UI or Presentation
1. Domain
1. Technical Services

### Dependency Injection
Allows for Injecting dependencies at by interface without having to worry about the specifics of the implementation of the interface.

### Model View Controller
The Model holds the state and the business logic
The View interacts with the user: displays data and sends the inputs of the user to the controller
Middleware between the Model and the View, decides which data to display to the user and how system actions map with user actions and the opposite direction.