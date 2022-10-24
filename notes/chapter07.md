Explain the actors in the adapter pattern (3)

[HFDP]

---

Target Interface: as the name implies, is the target interface that we want to adapt to. 
Adapter: is the wrapper class/instance. It should implement the target interface.
Adaptee: is instance with a different interface from the target that we want to adapt to the new interface. Adapter delegates actions to this instance.


===

Does an adapter always wrap one and only one class?

[HFDP]

---

The Adapter Pattern’s role is to convert one interface into another. Nevertheless, you may well have situations where an adapter holds two or more adaptees that are needed to implement the target interface. This relates to another pattern called the Facade Pattern; people often confuse the two.

===

Identify the following design pattern:

"It converts the interface of a class
into another interface the clients expect. Adapter lets
classes work together that couldn’t otherwise because of
incompatible interfaces."

[HFDP]

---

The adapter Pattern
<img width="820" alt="image" src="https://user-images.githubusercontent.com/1868409/197180603-aea6c936-4783-46e2-8147-148124c38421.png">
<img width="983" alt="image" src="https://user-images.githubusercontent.com/1868409/197180938-31e4811a-dc54-44db-ba82-551ba54ea6e5.png">

===

What's the difference between Decorator Pattern and Adapter Pattern? (2)

[HFDP]

---

- Decorators add new behavior to an instance that implements the **same** interface
- Apdapters don't add any new behavior, they only convert the interface of an instance that is **different**

===

Identify the following pattern:

"It provides a unified interface to a
set of interfaces in a subsystem. Facade defines a higherlevel interface that makes the subsystem easier to use"

[HFDP]

---

The Facade Pattern 
<img width="889" alt="image" src="https://user-images.githubusercontent.com/1868409/197183047-4313777b-8d6d-491d-879e-637bff686964.png">

===

What's the difference between the Facade pattern and the Decorator pattern?

[HFDP]

--- 

The facade’s intent is to provide a simplified interface to a subsystem, while an adapter’s is to convert
the interface to something different.

===

What does the following principle mean?

"Principle of Least Knowledge: talk only to your immediate friends"

[HFDP]

---

It means when you are designing a system, for any object, be careful of the
number of classes it interacts with and also how it comes to interact with those classes. 

===

How does the facade pattern implement the Principle of Least knowledge?

[HFDP]

---

Because at the end, the client will have "one friend" (The Facade instance) so we reduce the number of instances that we interact directly.

<img width="1015" alt="image" src="https://user-images.githubusercontent.com/1868409/197184710-96118daf-20c4-48d3-b7be-bd97b97415e8.png">