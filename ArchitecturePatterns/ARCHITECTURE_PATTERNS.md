# 💡 Summary
- [Design Pattern](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#what-is-a-design-pattern)
- [Dependency](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#dependency)
- [Dependency Injection](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#dependency-injection)
- [Dependency Inversion Principle](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#dependency-inversion-principle)
- [Dependency Injection Container](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#dependency-injection-container)
- [J2EE Patterns](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#j2ee-patterns)
- [GoF Patterns](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#gof-patterns)

# What is a Design Pattern?
* It represents the best practices used by experienced object-oriented software developers.
* They are solutions to general problems that software developers faced during software development.

# Dependency
* Dependency is a class that is required in another class so this other class can work 100%.

# Dependency Injection
* It is to inject dependencies through constructor instead new operator inside of the class.
* It decouples your classes construction from the construction of its dependencies.

# Dependency Inversion Principle
* It is basically that code should depend upon abstractions (interfaces).
* By decoupling from abstractions, whe are decoupling implementations from each other

# Dependency Injection Container
* It figure it out from all the class and all its dependencies, which dependency that specific class needs.
* Also Known As: Service Locator
* It is basically a map between the Class and its Depedencies.

# J2EE Patterns
* These design patterns are specifically concerned with the presentation tier. 

# GoF Patterns
There are 23 patterns between 3 types which fluctuate between abstraction and granularity.
  * Creational
  * Structural
  * Behavior 

# GoF Patterns - Creational
These design patterns provide a way to create objects while hiding the creation logic, rather than instantiating objects directly using new operator.
* [Abstract Factory](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#abstract-factory-pattern-creational)
* [Builder](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#builder-pattern-creational)
* [Factory](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#factory-pattern-creational)
* [Prototype](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#prototype-pattern-creational)
* [Singleton](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#singleton-pattern-creational)

# GoF Patterns - Structural
These design patterns concern class and object composition.
  * [Adapter](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#adapter-pattern-structural)
  * [Bridge](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#bridge-pattern-structural)
  * [Composite](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#composite-pattern-structural)
  * [Decorator](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#decorator-pattern-structural)
  * [Facade](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#facade-pattern-structural)
  * [Flyweight](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#flyweight-pattern-structural)
  * [Proxy](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#proxy-pattern-structural)

# GoF Patterns - Behavioral
These design patterns are specifically concerned with communication between objects.
  * [Chain of Responsibility](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#chain-of-responsibility-behavior)
  * [Command](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#command-behavior)
  * [Interpreter](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#interpreter-pattern-behavior)
  * [Iterator](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#iterator-pattern-behavior)
  * [Mediator](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#mediator-pattern-behavior)
  * [Memento](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#memento-pattern-behavior)
  * [Observer](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#observer-pattern-behavior)
  * [State](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#state-pattern-behavior)
  * [Strategy](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#strategy-pattern-behavior)
  * [Template Method](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#template-method-pattern-behavior)
  * [Visitor](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/ArchitecturePatterns/ARCHITECTURE_PATTERNS.md#template-method-pattern-behavior)
---
---
---
## Factory Pattern (Creational)
* It creates object without exposing the creation logic to the client and refer to newly created object using a common interface.
* [Example](https://www.tutorialspoint.com/design_pattern/images/factory_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/factory_pattern.htm)

## Abstract Factory Pattern (Creational)
* It works around a super-factory which creates other factories. 
* This factory is also called as factory of factories. 
* [Example](https://www.tutorialspoint.com/design_pattern/images/abstractfactory_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/abstract_factory_pattern.htm)

## Singleton Pattern (Creational)
* It involves a single class which is responsible to create an object while making sure that only single object gets created (Single Instance).
* It provides a static method to get its static instance to outside world.
* Usage: (Shared Resource / Single Instance) DB Connection, Logging, Service Locators, Printer Spooler, etc.
* [Example](https://www.tutorialspoint.com/design_pattern/images/singleton_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/singleton_pattern.htm)

## Builder Pattern (Creational)
* It builds a complex object using simple objects and using a step by step approach.
* You use this when you need to do a lot of things to build an object.
* [Example](https://www.tutorialspoint.com/design_pattern/images/builder_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/builder_pattern.htm)

## Prototype Pattern (Creational)
* It refers to creating duplicate object while keeping performance in mind.
* "Clone this object and make minor changes".
* This pattern is used when directly object creation is costly.
* [Example](https://www.tutorialspoint.com/design_pattern/images/prototype_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/prototype_pattern.htm)
---
---
---
## Adapter Pattern (Structural)
* Adapter pattern works as a bridge between two incompatible interfaces.
* An easy example is a Memory Reader (Memory Card -> Card Reader -> Computer).
* [Example](https://www.tutorialspoint.com/design_pattern/images/adapter_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/adapter_pattern.htm)

## Bridge Pattern (Structural)
* It decouples implementation class and abstract class by providing a bridge structure between them.
* It is used when we need to decouple an abstraction from its implementation so that two can vary independently.
* An interface does the mid-field.
* [Example](https://www.tutorialspoint.com/design_pattern/images/bridge_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/bridge_pattern.htm)

## Composite Pattern (Structural)
* It creates a class that contains group of its own objects.
* [Example](https://www.tutorialspoint.com/design_pattern/images/composite_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/composite_pattern.htm)

## Decorator Pattern (Structural)
* It allows a user to add new functionality to an existing object without altering its structure. 
* It creates a decorator class which wraps the original class and provides additional functionality keeping class methods signature intact.
* [Example](https://www.tutorialspoint.com/design_pattern/images/decorator_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/decorator_pattern.htm)

## Facade Pattern (Structural)
* It hides the complexities of the system and provides an interface to the client using which the client can access the system.
* It defines a higher-level interface that facilitates the use of the subsystem.
* [Example](https://www.tutorialspoint.com/design_pattern/images/facade_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/facade_pattern.htm)

## Flyweight Pattern (Structural)
* It tries to reuse already existing similar objects by storing them and creates new object when no matching object is found.
* It is used to reduce the number of objects created, to decrease memory and to improve performance.
* It might be done with HashMap help.
* [Example](https://www.tutorialspoint.com/design_pattern/images/Flyweight_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/flyweight_pattern.htm)

## Proxy Pattern (Structural)
* Its primary goal is to encapsulate a object using another that has the same interface.
* That way, the second object (aka: Proxy), will control the first object (the truly object).
* [Example](https://www.tutorialspoint.com/design_pattern/images/proxy_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/proxy_pattern.htm)
---
---
---
## Chain of Responsibility (Behavior)
* It creates a chain of receiver objects for a request.
* It decouples sender and receiver of a request based on type of request. 
* In this pattern, normally each receiver contains reference to another receiver. 
* If one object cannot handle the request then it passes the same to the next receiver and so on.
* A good example of a use of this pattern is the inheritance search mecanism of object oriented programming languages (Java, C# and etc).
* [Example](https://www.tutorialspoint.com/design_pattern/images/chain_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/chain_of_responsibility_pattern.htm)

## Command (Behavior)
* It allows to encapsulate an object and provide to another a way to execute the encapsulated object method in a dynamic way.
* A request is wrapped under an object as command and passed to invoker object.
* Invoker object looks for the appropriate object which can handle this command and passes the command to the corresponding object which executes the command
* [Example](https://www.tutorialspoint.com/design_pattern/images/command_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/command_pattern.htm)

## Interpreter Pattern (Behavior)
* It defines a grammatical representation for a language and provides an interpreter to deal with this grammar.
* It is used in SQL parsing, symbol processing engine etc.
* But the best example is the java source code into byte code that is understandable by JVM.
* [Example](https://www.tutorialspoint.com/design_pattern/images/interpreter_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/interpreter_pattern.htm)

## Iterator Pattern (Behavior)
* It provides a way to access the elements of an aggregate object sequentially without exposing its underlying representation.
* For example, to iterate through a collection of custom objects, you do not need to know the size.
* [Example](https://www.tutorialspoint.com/design_pattern/images/iterator_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/iterator_pattern.htm)

## Mediator Pattern (Behavior)
* It defines an object that encapsulates how a set of objects interact.
* It provides a mediator class which normally handles all the communications between different classes and supports easy maintenance of the code by loose coupling. 
* It is used to reduce communication complexity between multiple objects or classes.
* [Example](https://www.tutorialspoint.com/design_pattern/images/mediator_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/mediator_pattern.htm)

## Memento Pattern (Behavior)
* Without violating encapsulation, capture and externalize an object's internal state so that the object can be returned to this state later.
* It is used to restore state of an object to a previous state. 
* It promotes undo or rollback to full object status.
* [Example](https://www.tutorialspoint.com/design_pattern/images/memento_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/memento_pattern.htm)

## Observer Pattern (Behavior)
* It is used when there is one-to-many relationship between objects.
* And, if it is modified, its depenedent objects should be notified/updated automatically.
* The "View" part of Model-View-Controller.
* [Example](https://www.tutorialspoint.com/design_pattern/images/observer_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/observer_pattern.htm)

## State Pattern (Behavior)
* Allow an object to alter its behavior when its internal state changes. 
* We create objects which represent various states and a context object whose behavior varies as its state object changes.
* [Example](https://www.tutorialspoint.com/design_pattern/images/state_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/state_pattern.htm)

## Strategy Pattern (Behavior)
* Define a family of algorithms, encapsulate each one, and make them interchangeable. 
* Strategy lets the algorithm vary independently from the clients that use it.
* [Example](https://www.tutorialspoint.com/design_pattern/images/strategy_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/strategy_pattern.htm)

## Template Method Pattern (Behavior)
* It lets subclasses redefine certain steps of an algorithm without changing the algorithm's structure.
* Base class declares algorithm 'placeholders', and derived classes implement the placeholders.
* It works like a template for the derived classes.
* [Example](https://www.tutorialspoint.com/design_pattern/images/template_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/template_pattern.htm)

## Visitor Pattern (Behavior)
* It lets you define a new operation without changing the classes of the elements on which it operates.
* A good example is the possibility to add new functionalities to objects structures of an existing object withouth changing it.
* [Example](https://www.tutorialspoint.com/design_pattern/images/visitor_pattern_uml_diagram.jpg)
* [Reference](https://www.tutorialspoint.com/design_pattern/visitor_pattern.htm)