# 💡 Summary
- [DRY (Dont Repeat Yourself)](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DevelopmentPrinciples/DEVELOPMENT_PRINCIPLES.md#dry-dont-repeat-yourself)
- [KISS (Keep It Simple, Stupid!)](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DevelopmentPrinciples/DEVELOPMENT_PRINCIPLES.md#kiss-keep-it-simple-stupid)
- [YAGNI (You aren't gonna need it)](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DevelopmentPrinciples/DEVELOPMENT_PRINCIPLES.md#yagni-you-arent-gonna-need-it)
- [GRASP](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DevelopmentPrinciples/DEVELOPMENT_PRINCIPLES.md#grasp)
- [S.O.L.I.D](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DevelopmentPrinciples/DEVELOPMENT_PRINCIPLES.md#solid)
- [Clean Code](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DevelopmentPrinciples/DEVELOPMENT_PRINCIPLES.md#clean-code)
---
---
---
# DRY (Dont Repeat Yourself)
* In the layered architecture approach DRY code is very essential for robust software development.
* If you are developing and you are repeating a lot some part of the code, you probably could use a function for re use this code
* [Reference](http://www.c-sharpcorner.com/UploadFile/dhananjaycoder/keep-your-code-dry/)


# KISS (Keep It Simple, Stupid!)
* A simple solution is better than a complex one, even if the solution looks stupid.
* The KISS principle is about striving for simplicity.
* The KISS principle states that there is no value in a solution being "clever" but in one being easily understandable.
* Sometimes developers might feel tempted to write "clever" solutions that use all these complex features.
* The KISS principle states that a solution is better when it uses less inheritance, less polymorphism, fewer classes, etc.
* [Reference](http://principles-wiki.net/principles:keep_it_simple_stupid)


# YAGNI (You aren't gonna need it)
* Principle of extreme programming (XP) that states a programmer should not add functionality until deemed necessary.
* "Always implement things when you actually need them, never when you just foresee that you need them."
* On of the simplest thing that could possibly work.
* It is meant to be used in combination with several other practices, such as continuous refactoring, continuous automated unit testing, and continuous integration. 
* Used without continuous refactoring, it could lead to disorganized code and massive rework
* [Reference](https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it)


# GRASP
* General Responsibility Assignment Software Principle.
* Guidelines for assigning responsibility to classes and objects in object-oriented design.
* The different patterns and principles used in GRASP are:
  * **Controller:** Controller design principle helped in minimizing the dependency between GUI components and Domain Model classes.
  * **Creator:** Creator is a GRASP principle and helps in deciding which class should be responsible for creating a new instance of a class.
  * **Indirection:** How to let objects interact in a manner that the bond among them remain weak? Give the responsibility of interaction to an intermediate object so that the coupling among different components remain low.
  * **Information Expert:** Gives guidelines about giving responsibilities to classes. It says assign a responsibility to the class which has the information necessary to fulfill that responsibility.
  * **Low Coupling:** This principle states that one should assign a responsibility so that the dependency between the classes remains low
  * **Polymorphism:** This principle provides guidelines about how to use this oop language feature in your object oriented design.
  * **Protected Variations:** It protects elements from the variations on other elements by wrapping the focus of instability with an interface and using polymorphism to create various implementations of this interface.
  * **Pure Fabrication:** A pure fabrication is a class that does not represent a concept in the problem domain, specially made up to achieve low coupling, high cohesion, and the reuse potential thereof derived.
  * [Reference](https://en.wikipedia.org/wiki/GRASP_(object-oriented_design))


# S.O.L.I.D
### **"S" (Single Responsibility Principle)**
* "A class should have one, and only one, reason to change".
* Build a separate class for each type of thing (Validation, Post methods, Get methods).

### **"O" (Open Closed Principle)**
* "Objects or entities should be open for extension, but closed for modification".
* I've got a SAQUE method in CONTA class.
* I have CONTAPOUPANCA inheriting CONTA with an override method called SAQUE with your specific implementation.

### **"L" (Liskov Substitution Principle)**
* Every subclass/derived class should be substitutable for their base/parent class.
* This principles says that we cannot just say the: A SQUARE IS RECTANGLE.
* We gotta care about the behaviors.

### **"I" (Interface Seggregation Principle)**
* The class "X" must not be forced to depend on methods which it will not use it.
* Some specifics interfaces are better than one generic interface.

### **"D" (Dependecy Injection Principle)**
* High-level modules, should not depend on low-level modules. Both should depend on abstractions.
* Abstractions should not depend on details.
* Details should depend on abstraction.
* You should depend on abstraction not on Implementation.
* You want to hire Internet. You just want to have this working. You do not need to know how VIVO/GVT works to delivery that to you.


# Clean Code

### **Meaningful Names**
* Names must reflect what a variable, field, property stands for. Names have to be precise.
* Choose names that reflect the level of abstraction of the class or method you are working in.
* Use long names for long scopes.
* Names have to reflect the entire functionality.
* Use standard nomenclature where possible.
  * Camel Case: "AbcDefg", "MyClass"
  * Pascal Case: "abcDefg", "myVariable"
* [Reference](http://www.itiseezee.com/?p=83)

### **Summary**
* Summary might look unncessary, but is trully important to a good code writing.
* Its purpose is to describe what a method / prop / enum... does.
* It is very important to create a documentation pattern.
* In a macro view, how much time do you spend reviewing someone else code trying to understand if it fits you?
* Wouldn't it be better to have a description of what your method does to someone else understand, it would?
  * Summary: Quick briefing of what your method does.
  * Param: A quick explanation about the method's parameters.
  * Returns: A general explanation about the method's return.
  * Remarks: Observation that might be useful for others developers.
* [Reference](http://www.planetgeek.ch/wp-content/uploads/2011/02/Clean-Code-Cheat-Sheet-V1.3.pdf)

### **Syntatic Sugar**
* Is a simple way to write code.
* Nullable Assignament: int Anos? { get; set; }
  * With this expression, you are saying that te Anos prop is a Nullable Type.
* Nullable Verification: A ?? B ?? C?? "VALOR QUALQUER"
  * With this expression, you are checking if every var (A,B,C) is null, and else, using the next statement.
* Using approach: using (var x = new X()){ ... }
  * With this expression, you are using the try{} finally {} terms but in a hidden way.
* [Reference](http://eduardopires.net.br/2012/08/c-sharp-iniciantes-syntactic-sugar/)
