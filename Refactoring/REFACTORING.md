# 💡 Summary
- [What?](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/Refactoring/REFACTORING.md#what-should-i-refactor-it)
    - [Bloaters](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/Refactoring/REFACTORING.md#bloaters)
    - [OO Abusers](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/Refactoring/REFACTORING.md#object-orientation-abusers)
    - [Dispensables](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/Refactoring/REFACTORING.md#dispensables)
- [How?](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/Refactoring/REFACTORING.md#how-should-i-refactor-it)
    - [Composing methods](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/Refactoring/REFACTORING.md#composing-methods-link)
    - [Moving Feat x Obj](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/Refactoring/REFACTORING.md#moving-features-between-objects-link)
    - [Organizing Data](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/Refactoring/REFACTORING.md#organizing-data-link)
    - [Simplifying Cond. Exp](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/Refactoring/REFACTORING.md#simplifying-conditional-expressions-link)
    - [Simplifying Method Calls](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/Refactoring/REFACTORING.md#simplifying-method-calls-link)
---
---
---
# What should I Refactor it?

## Bloaters
Bloaters are code, methods and classes that have increased to such gargantuan proportions that they are hard to work with. 

* **Long Method:** When a method contains too many lines of code.
* **Large Class:** When a class contains many fields/methods/lines of code.
* **Primitive Obsession:** When the use of primitives instead of small objects for simple tasks.
* **Long Parameter List:** When more than three or four parameters per method.
* **Data Clumps:** When different parts of the code contains identical groups of variables.


## Object-Orientation Abusers
All these items (smells) are incomplete or incorrect in an application of OOP principles

* **Switch Statements:** You have a complex switch operator or sequence of if statements.
* **Temporary Field:** When fields are filled in only some circustances.
* **Refused Bequest:** Unnecessary methods from a superclass (when the derived classes does not use them).
* **Alternative Classes with Different Interfaces:** Two classes perform identical functions but have different method names.

## Dispensables
A dispensable is something pointless and unneeded whose absence would make the code cleaner, more efficient and easier to understand.

* **Comments:** A method is filled with explanatory comments.
* **Duplicate Code:** Two code fragments look almost identical.
* **Lazy Class:** If a class doesn't do enough to earn your attention, it should be deleted.
* **Data Class:** When class contains only CRUD methods (OOP benefits is that they can contain behavior types or operations on their data).
* **Dead Code:** A variable, parameter, field, method or class is no longer used (obsolete).
* **Speculative Generality:** When code is created for the future/speculation.

# How should I Refactor it?

## Composing methods ([Link](https://sourcemaking.com/refactoring/composing-methods))
These refactoring techniques, removes code duplication, and pave the way for future improvements.

* **Extract Method:**
    * **Problem:** You have a code fragment that can be grouped together.
    * **Solution:** Move this code to a separate new method (or function) and replace the old code with a call to the method.

* **Inline Method:**
    * **Problem:** When a method body is more obvious than the method itself, use this technique.
    * **Solution:** Replace calls to the method with the method's content and delete the method itself.

* **Extract Variable:**
    * **Problem:** You have an expression that is hard to understand.
    * **Solution:** Place the result of the expression or its parts in separate variables that are self-explanatory.

* **Inline Temp:**
    * **Problem:** You have a temporary variable that is assigned the result of a simple expression and nothing more.
    * **Solution:** Replace the references to the variable with the expression itself.

* **Replace Temp with Query:**
    * **Problem:** You place the result of an expression in a local variable for later use in your code.
    * **Solution:** Move the entire expression to a separate method and return the result from it. Query the method instead of using a variable. Incorporate the new method in other methods, if necessary.

* **Split Temporary Variable:**
    * **Problem:** You have a local variable that is used to store various intermediate values inside a method.
    * **Solution:** Use different variables for different values. Each variable should be responsible for only one particular thing.

* **Remove Assignments to Parameters:**
    * **Problem:** Some value is assigned to a parameter inside method's body.
    * **Solution:** Use a local variable instead of a parameter.

* **Replace Method with Method Object:**
    * **Problem:** You have a long method in which the local variables are so intertwined that you cannot apply Extract Method.
    * **Solution:** Transform the method into a separate class so that the local variables become fields of the class. Then you can split the method into several methods within the same class.
    * [Example](https://sourcemaking.com/refactoring/replace-method-with-method-object)

## Moving Features between Objects ([Link](https://sourcemaking.com/refactoring/moving-features-between-objects))
These refactoring techniques show how to safely move functionality between classes, create new classes, and hide implementation details from public access.

* **Move Method:**
    * **Problem:** A method is used more in another class than in its own class.
    * **Solution:** Create a new method in the class that uses the method the most, then move code from the old method to there. 

* **Move Field:**
    * **Problem:** A field is used more in another class than in its own class.
    * **Solution:** Create a field in a new class and redirect all users of the old field to it.

* **Extract Class:**
    * **Problem:** When one class does the work of two, awkwardness results.
    * **Solution:** Create a new class and place the fields and methods responsible for the relevant functionality in it.

* **Inline Class:**
    * **Problem:** A class does almost nothing and is not responsible for anything, and no additional responsibilities are planned for it.
    * **Solution:** Move all features from the class to another one.

* **Hide Delegate:**
    * **Problem:** The client gets object B from a field or method of object А. Then the client calls a method of object B.
    * **Solution:** Create a new method in class A that delegates the call to object B. Now the client does not know about, or depend on, class B.
    * [Example](https://sourcemaking.com/refactoring/hide-delegate)

* **Introduce Foreign Method:**
    * **Problem:** A utility class does not contain the method that you need and you cannot add the method to the class.
    * **Solution:** Add the method to a client class and pass an object of the utility class to it as an argument.
    * [Example](https://sourcemaking.com/refactoring/introduce-foreign-method)

## Organizing Data ([Link](https://sourcemaking.com/refactoring/organizing-data))
These refactoring techniques help with data handling, replacing primitives with rich class functionality.

* **Self Encapsulate Field:**
    * **Problem:** You use direct access to private fields inside a class.
    * **Solution:** Create a getter and setter for the field, and use only them for accessing the field.

* **Replace Data Value with Object:**
    * **Problem:** A class (or group of classes) contains a data field. The field has its own behavior and associated data.
    * **Solution:** Create a new class, place the old field and its behavior in the class, and store the object of the class in the original class.

* **Replace Array with Object:**
    * **Problem:** When you have an array that contains various types of data.
    * **Solution:** Replace the array with an object that will have separate fields for each element.

* **Duplicate Observed Data:**
    * **Problem:** Is domain data stored in classes responsible for the GUI?
    * **Solution:** Then it is a good idea to separate the data into separate classes, ensuring connection and synchronization between the domain class and the GUI.

* **Replace Magic Number with Symbolic Constant:**
    * **Problem:** Your code uses a number that has a certain meaning to it.
    * **Solution:** Replace this number with a constant that has a human-readable name explaining the meaning of the number.

* **Encapsulate Field:**
    * **Problem:** You have a public field.
    * **Solution:** Make the field private and create access methods for it.

* **Encapsulate Collection:**
    * **Problem:** A class contains a collection field and a simple getter and setter for working with the collection.
    * **Solution:** Make the getter-returned value read-only and create methods for adding/deleting elements of the collection.

* **Replace Type Code with Class:**
    * **Problem:** A class has a field that contains type code. The values of this type are not used in operator conditions and do not affect the behavior of the program.
    * **Solution:** Create a new class and use its objects instead of the type code values.

* **Replace Type Code with Class:**
    * **Problem:** A class has a field that contains type code. The values of this type are not used in operator conditions and do not affect the behavior of the program.
    * **Solution:** Create a new class and use its objects instead of the type code values.

## Simplifying Conditional Expressions ([Link](https://sourcemaking.com/refactoring/simplifying-conditional-expressions))
Conditionals tend to get more and more complicated in their logic over time, and there are yet more techniques to combat this as well.

* **Decompose Conditional:**
    * **Problem:** You have a complex conditional (if-then/else or switch).
    * **Solution:** Decompose the complicated parts of the conditional into separate methods: the condition, then and else.

* **Consolidate Conditional Expression:**
    * **Problem:** You have multiple conditionals that lead to the same result or action.
    * **Solution:** Consolidate all these conditionals in a single expression.

* **Consolidate Conditional Expression:**
    * **Problem:** You have multiple conditionals that lead to the same result or action.
    * **Solution:** Consolidate all these conditionals in a single expression.

* **Remove Control Flag:**
    * **Problem:** You have a boolean variable that acts as a control flag for multiple boolean expressions.
    * **Solution:** Instead of the variable, use break, continue and return.

* **Replace Nested Conditional with Guard Clauses:*
    * **Problem:** You have a group of nested conditionals and it is hard to determine the normal flow of code execution.
    * **Solution:** Isolate all special checks and edge cases into separate clauses and place them before the main checks. 


* **Replace Conditional with Polymorphism:*
    * **Problem:** You have a conditional that performs various actions depending on object type or properties.
    * **Solution:** Create subclasses matching the branches of the conditional. In them, create a shared method and move code from the corresponding branch of the conditional to it. Then replace the conditional with the relevant method call.  

## Simplifying Method Calls ([Link](https://sourcemaking.com/refactoring/simplifying-method-calls))
These techniques make method calls simpler and easier to understand. This, in turn, simplifies the interfaces for interaction between classes.

* **Rename Method:**
    * **Problem:** The name of a method does not explain what the method does.
    * **Solution:** Rename the method.

* **Add Parameter:**
    * **Problem:** A method does not have enough data to perform certain actions.
    * **Solution:** Create a new parameter to pass the necessary data.

* **Separate Query from Modifier:**
    * **Problem:** Do you have a method that returns a value but also changes something inside an object?
    * **Solution:** Split the method into two separate methods. As you would expect, one of them should return the value and the other one modifies the object.

* **Parameterize Method:**
    * **Problem:** Multiple methods perform similar actions that are different only in their internal values, numbers or operations.
    * **Solution:** Combine these methods by using a parameter that will pass the necessary special value.

* **Replace Parameter with Explicit Methods:**
    * **Problem:** A method is split into parts, each of which is run depending on the value of a parameter.
    * **Solution:** Extract the individual parts of the method into their own methods and call them instead of the original method.

* **Remove Setting Method:**
    * **Problem:** The value of a field should be set only when it is created, and not change at any time after that.
    * **Solution:** So remove methods that set the field's value.

* **Hide Method:**
    * **Problem:** A method is not used by other classes or is used only inside its own class hierarchy.
    * **Solution:** Make the method private or protected.

* **Replace Error Code with Exception:**
    * **Problem:** A method returns a special value that indicates an error?
    * **Solution:** Throw an exception instead.x