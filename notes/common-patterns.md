# Common Patterns

## Architecture Patterns

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

## Responsability Assignation Patterns
They define the responsabilities of the elements that conform the system.

### Controller
Manages system events. The controller element detects events and triggers actions or informs of these events to other parts of the system. There are a few of them:
1. Facade Controller: Models all the possible events in the system and adds proxies to them.
1. Use Case Controller: Models a use case for the system. Contains as many operations as you can have for the specific use case.
1. Session Controller: Represents an actor's session. Models all possible interactions the actor and the system can have.
1. Transaction Controller: Contains a single action: `execute()`, which represents a unary operation in the system.

Creator method able to decide with specific subclass to implement depending on the environment that invokes it. Basically we delegate the responsability of deciding which Classes to create by delegating the decision to the subclasses in change of requesting the creation of the new object.
### Expert
Manages a highly specialized operation within the system. The expert tends to be the Class that models the real or virtual operation that the system is targeting.

### Pure Fabrication
A Class that does not translate to a real component of the model but whose sole purpose is to manage a specially complex part of the business logic. You can think of it as a highly specialized consumer facing service provider.

### Creator or Factory
We need to create instances of a class, this patterns allows us to do this easily.

## Design Patterns

### State
Contains a conditional block that knows how to update the state when certain events trigger.

### Facade
Offers abstraction over a subsystem, while centralizing access and offering and abstraction layer that can potentially simplify the intricacies of the mentioned subsystem.

### Iterator
Allows iterative access over the objects contained in a class property without revealing information over the internal implementation of these class or the way the objects are aggregated.
The Iterator Class has to implement, at least, the following methods:
• `reset()` -> Resets the iteration
• `next()` -> Advances one element and returns it
• `hasNext()` -> Returns a boolean that reflects if we still have elements to explore.

### Factory method
Creator method able to decide with specific subclass to implement depending on the environment that invokes it. Basically we delegate the responsability of deciding which Classes to create by delegating the decision to the subclasses in change of requesting the creation of the new object.