Explain how "Change" can impact the repeated use of the "new" keyword when instantiating classes and how we can mitigate it.

[HFDP]

---

When we use the keyword "new" too much, we expose too many **concrete objects**. This will cause trouble because the code may have to be changed as new concrete classes are added. So, in other words, your code will
not be “**closed for modification**.”

The way to mitigate this is **to code to an interface** instead. By doing this you can **insulate yourself**
from many of the changes that might happen to a system down the road. Why? If your code is written to an interface, then it will work with any new classes implementing that interface through polymorphism

===

Identify the following design pattern:

"It defines an interface for creating an object, but lets subclasses decide which class to instantiate. This pattern lets a class defer instantiation to subclasses"

[HFDP]

---

The Factory Method pattern

<img width="1220" alt="image" src="https://user-images.githubusercontent.com/1868409/196166977-0a67f121-5361-4f5a-b826-6648404e51b1.png">
<img width="1193" alt="image" src="https://user-images.githubusercontent.com/1868409/196167157-fbcb1317-bf34-48db-a015-fc1d0404172c.png">

===

Explain actors involed in the factory method pattern

[HFDP]

---

Creator: responsible for exposing the method that instantiates the objects. The abstract creator should define an abstract method (like createProduct) that each subclass should implement.

Product: the final object that the factory produces, each product should implement the same interface.

===

Explain the principle: "Depend upon abstractions. Do not depend upon concrete classes"

[HFDP]

---

This principle suggests that our high-level components should not depend on our low-level
components; rather, they should both depend on abstractions.

===

Identify the following pattern:

"It provides an interface for creating families of related or dependent objects
without specifying their concrete classes"

[HFDP]

---

The Abstract Factory Pattern