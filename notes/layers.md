# Layers

Contains a set of classes named Controllers that will canalize the business logic and application specific operations. On the other hand, there are also a set of classes that model the domain of our use case.

### Starting our domain layer design
The first step is to define our domain diagram, which contains the set of classes that we will use with the following information:
• Associations
• Associative Classes
• Multiple Inheritance Cases
• Dynamic Generalization
• Derived Information
• Integrity Restrictions

Those operations that are not specific to any class and that represent infrastructure communication operations, data persistance... shall be delegated to Technical Services, of Services for short.