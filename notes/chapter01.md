"Identify the aspects of your application that vary and separate them from what stays the same"

What does this principle mean?

[HFDP]

---

Take the parts that vary and encapsulate them, so that later you can
alter or extend the parts that vary without affecting those that don’t.

===

Why shoul we "Program to an interface, not an implementation"?

[HFDP]

---

The point is to exploit polymorphism by programming
to a supertype so that the actual runtime object isn’t locked into
the code. By doing this, it's easy to replace a concrete behavior by other that conforms to the same interface

<img width="518" alt="image" src="https://user-images.githubusercontent.com/1868409/195325169-aa2479d5-0672-4e19-af11-1eb57ae7e5d9.png">

===

Why should we "Favor composition over inheritance"? (2)

[HFDP]

---

As you’ve seen, creating systems using composition gives you
a lot more flexibility. (1) Not only does it let you encapsulate
a family of algorithms into their own set of classes, but it
also (2) lets you change behavior at runtime as long as
the object you’re composing with implements the correct
behavior interface. 

===

Identify the following design principle:

"Defines a family of algorithms,
encapsulates each one, and makes them interchangeable.
(...) lets the algorithm vary independently from
clients that use it"

[HFDP]

---

The Strategy Pattern