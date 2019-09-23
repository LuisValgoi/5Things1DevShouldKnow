# 💡 Summary
- [OOP](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DevelopmentConcepts/DEVELOPMENT_CONCEPTS.md#object-oriented-programming)
- [General](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DevelopmentConcepts/DEVELOPMENT_CONCEPTS.md#general)
- [Graphic](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DevelopmentConcepts/DEVELOPMENT_CONCEPTS.md#graphic)
- [Security](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DevelopmentConcepts/DEVELOPMENT_CONCEPTS.md#security)
- [I18n & L10n](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DevelopmentConcepts/DEVELOPMENT_CONCEPTS.md#internationalization-i18n--localization-l10n)
---
---
---
# Object Oriented Programming

### **What is Behavior & State ?**
* States are declared in "fields" and are related to what your **objects** _are_.
* Behaviors are declared in "methods" and are related to what your **objects** _do_.

### **What is Abstract ?**
* Abstract Class are classes that provides some default states and implementations which it can be used when inherited.
* You may have a base implementation.
* Interfaces can have a state or implementation.
* Cannot instantiate objects.
* A abstract class can be inherited only once.
* **Pros:**
  * You may have a base implementation.
  * Interfaces can have a state or implementation.
* **Cons:**
  * Cannot instantiate objects.
  * A abstract class can be inherited only once.

### **What is an Interface ?**
* It is kind of a contract that you sign in when implements it.
* It does not have implementation, but signatures.
* You cannot instanciate it or ctor it.
* It works like an agreement.
* Multiple interfaces inheritance.
* **Pros:**
  * You can have multiple-inherited.
* **Cons:**
  * You must implement the methods.
  * Interfaces can have no state. 
  * Interfaces can have no implementation.

### **What is Couplin ?**
* It is how much a class is connected to another in a strong or a week way.
* The more connected a class is connect to another, more problems I have.
* It happens because if I update one, others that is connected to it, will be affected.
* The savior for a Strong Coupling is the Inversion of Control / Dependency Injection.

### **What is Cohesion ?**
* It is totally connected do SRP - Single Responsibility Principle.
* A class should not assign other classes responsibilities.
* The more cohesion I have, the better.

### **What is Encapsulation ?**
* It refers to an object's ability to hide data or behavior that are not necessary to be public to someone.
* Is defined "as the process of enclosing one or more items within a physical or logical package".
* Encapsulation is implemented by using access specifiers:
  * Public / Private / Protected / Internal

### **What is Inheritance ?** 
* It is when you have a Base Class and throught inheritance, you passes to your child class its properties.
* Normally, when you want to know if you should use Inheritance, ask yourself:
  * "Is this class X a class Y ?"
  * "Is a Motocycle a Vehicle ?" 
* **Pros:** Capture the common uses. Code recyclying
* **Cons:** Week encapsulation. Strong Coupling. Tied to Build Time.

### **What is Composition ?**
* Is when you extends a class by another objects delegation. In real time. When you need it.
* Normally, when you want to know if you should use Composition, ask yourself:
  * "Is this class X has a Y"?
  * "Is this System has a Person"?
* **Pros:** Real time behavior. Tied to Execution Time. Responsabilities separation. Good Coupling.
* **Cons:** Fucking hard to know in a big application.

### **What is Polymorphism ?**
* It is a pattern in OOP which classes have different behaviors.
* It happens due theirs specific implementation while sharing a common interface.
* Is the ability (in programming) to present the same interface for differing underlying forms (data types).
* The classic example is the Shape class and all the classes that can inherit from it (square, circle, etc).

# General

### **WebService ?**
* By definition, they are services exposed in a network that allow communication between one or more electronic devices, capable of sending and processing data.
* To do this, Web Services uses the SOAP protocol and the REST design template.

### **SOAP (Simple Object Access Protocol) ?**
* Web Service. Well defined, mature.
* It aims to establish a protocol for communication of objects and services.
* For transport, use generic methods (SMTP, JMS).
* As Object Transfer, uses XMLs.
* Envelop that defines the content of the message.
* Set of coding rules for data types.
 
### **REST (Representational State Transfer) ?**
* Web Service. Design Pattern that gives idea of how to correctly use HTTP verbs.
* Easy implementation and understanding.
* Return and its type is requested by the developer, that is, returns any language.
* Uses the URI pattern.
* You can also use XMLHttpRequest (old base AJAX).
* When an application uses all its good practices, it is called: RESTful.

### **URI (Uniform Resource Identifier) ?**
* They are the utilization's interface of your services (e.g.:`service.com/User`).
* They work as a contract that will be used by customer / clients to access them.  

### **WebSocket ?**
* Advanced technology.
* Opens an interactive communication session between the user's browser and a server.
* You are able to send messages to a server and receive their message without having to query the server for a response.

### **Stateless Session ?**
* It is the ability that a server has to process client requests without any data kept on it.
* So, the data must be sent to the server with all the need information to be fully processed and returned.

### **Content Negotiation ?**
* It occurs mainly in REST services that expects multiples formats.
* It expects that the client block inform that desired format.
* It is the resources format negotiation. (AKA: accept header).

### **JDBC (Java Database Connectivity) ?**
* It is a standard for Database Access.
* It is a standard for direct connection to a Database and execution of queries (SELECT * FROM).
* One of the issues is that the application may have bad codes due to the large amount of datasets and mapping between objects, making logic and SQL queries mixed.

### **JPA (Java Persistence API) ?**
* It is a standard for ORM - Object Relational Mapping.
* Allows you to map between objects in code and database tables.
* This, "hides" the developer's SQL queries causing it to just wrap with JAVA classes.
* Generally, "annotations" in getters and setters makes the linke betweens a ORM and ENTITY.
* The most famous is HIBERNATE, but there is OpenJPA, TopLink and so on.
* Obs: Hibernate, use JDBC for persistence.

### **JSF (Java Server Faces) ?**
* Technology that allows developers to create JAVA Web applications using pre-made visual components.
* This causes dev not to worry about JavaScript and HTML.
* Save the state of the components - creating the Stateful feature (navigation with values selected in a wizard, for example).
* Separate the layers - MVC.

### **JSP (Java Server Pages) ?**
* Its primary goal is the generation of dynamic content for Internet pages.
* Instead of using HTML to develop statistical and non-functional Web pages, you can use JSP for dynamism.
* It is possible to write HTML codes with embedded JSP codes. Razor (c #) like.

### **ORM (Object Relational Mapping) ?**
* It is a technique used to reduce the impedance of OOP.
* The Database tables are represented by class which each row in the table is represented by a single instance of this specifc class.

### **P.O.C.O (Plain OLD CLR Object) ?**
* A POCO class is used as a domain class of your application.
* It does not have any connection with any .net framework.
* Build a POCO class is to build some class that express the business with props, ctor and methods using only the .NET Framework.

### **Spring Framework ?**
* Non-intrusive framework, based on the IoC (Control Inversion) and Dependency Injection design standards.
* In Spring, Container is responsible for instantiating classes and defining dependencies through an XML configuration file (it can have several).
* Architecture based on Interfaces and POJOS (Plain Old Java Objects).
* Spring Data = Persistence handling.
* Spring Security = Handles application security.


# Graphic
### **What is SVG ?**
* Is an XML-based markup language for describing two dimensional based.
* SVG is essentially to graphics what HTML is to text.
* SVG images and their related behaviors are defined in XML text files which means they can be searched, indexed, scripted and compressed.
* Additionally this means they can be created and edited with any text editor and with drawing software. 
* SVG drawings and images are created using a wide array of elements.
* They are dedicated to the construction, drawing, and layout of vector images and diagrams.

### **SVG Attributes:**
* [SVG attributes by category](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute#SVG_attributes_by_category)
* [SVG attributes A to Z](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute#SVG_attributes_A_to_Z)

### **SVG Elements:**
* [SVG attributes by category](https://developer.mozilla.org/en-US/docs/Web/SVG/Element#SVG_elements_by_category)
* [SVG Elements from A to Z](https://developer.mozilla.org/en-US/docs/Web/SVG/Element#SVG_elements_A_to_Z)

# Security
* [Secure Development Guidelines](https://developer.mozilla.org/en-US/docs/Mozilla/Security/Secure_Development_Guidelines)

* _**Confidentiality**_: Imagine that only the people who are authorized to do so can gain access to sensitive data.
* _**Integrity**_: It refers to ensuring the authenticity of information.
* _**Availability**_: It means that information is accessible by authorized users.
* _**Vulnerability**_: It is a weakness in a system that can be exploited to negatively impact confidentiality, integrity, and/or availability.
* _**Threat**_ : It is any circumstance or event with the potential to adversely impact data or systems via unauthorized access.
* _**Privilege**_: The system should offer only the required functionality to each authorized user, so that no one can use functions that are not necessary.
* _**TCP/IP**_: When a user wants to transfer data across networks, the data is passed from the highest layer through intermediate layers to the lowest layer (Application / Transport / Network / Data Link).
* _**Same Origin Policy**_: It restricts how a document or script loaded from one origin can interact with a resource from another origin (mechanism for isolating potentially malicious documents). 
* _**Mixed content**_ : Pages that includes content fetched using cleartext HTTP. They are only partially encrypted, leaving the unencrypted content accessible to sniffers and man-in-the-middle attackers.
* _**Content Delivery Network**_: Is a group of servers spread out over many locations.
* _**SubResource Integrity**_: Is a security feature that enables browsers to verify that files they fetch (for example, from a CDN) are delivered without unexpected manipulation.

# Internationalization (I18n) & Localization (L10n)

* [W3C Internationalization](https://www.w3.org/International/technique-index)
* Browsers process text as Unicode internally.
* UTF-8 is a way of representing characters in terms of bytes is used for transferring text over the network to the browser.

>"Think Globally, Act Locally"

### **What is I18n?**_
* Is the process through which products can be prepared to be taken to other countries.
* "Building the structure of a piece of software so that it can be adjusted for different markets"

### **What I18n includes?**_
>"Designing and developing in a way that removes barriers to localization or international deployment. This includes such things as enabling the use of Unicode, or ensuring the proper handling of legacy character encodings where appropriate, taking care over the concatenation of strings, avoiding dependance in code of user-interface string values, etc."

>"Providing support for features that may not be used until localization occurs. For example, adding markup in your DTD to support bidirectional text, or for identifying language. Or adding to CSS support for vertical text or other non-Latin typographic features.”

>"Enabling code to support local, regional, language, or culturally related preferences. Typically this involves incorporating predefined localization data and features derived from existing libraries or user preferences. Examples include date and time formats, local calendars, number formats and numeral systems, sorting and presentation of lists, handling of personal names and forms of address, etc."

>"Separating localizable elements from source code or content, such that localized alternatives can be loaded or selected based on the user’s international preferences as needed."

### **What is L10n?**_
* Localization is simply the act of changing a piece of software to suit a different locale. 
* "Process of actually doing so for a specific market"
* Often thought of only as a synonym for translation of the user interface and documentation, localization is often a substantially more complex issue.

### **What L10n includes?**_
* Numeric, date and time formats
* Use of currency
* Keyboard usage
* Collation and sorting
* Symbols, icons and colors
* Text and graphics containing references to objects, actions or ideas which, in a given culture, may be subject to misinterpretation or viewed as insensitive.
* Varying legal requirements
* and many more things.
