Identify the following pattern:

"It provides a way to
access the elements of an aggregate object
sequentially without exposing its underlying
representation."

[HFDP]

---

The Iterator Pattern

<img width="1011" alt="image" src="https://user-images.githubusercontent.com/1868409/197758524-3fe87b99-bb2b-445f-8687-8e49761f15f6.png">

===

Explain actors involved in the iterator pattern (2)

[HFDP]

---

- Aggregate: holds the collection of items and exposes a method that returns the corresponding iterator.
- Iterator: exposes a set of methods for traversing over elements of a collection. Each iterator should implement the same interface.

===

Explain when a module has high cohesion and when a module has low cohesion.

[HFDP]

---

We say that a module or
class has high cohesion when it
is designed around a set of related
functions, and we say it has low
cohesion when it is designed around a
set of unrelated functions.

===

What's the relation between having high cohesion and the SRP (A class should have only one
reason to change)?

[HFDP]

---

Classes that adhere to the principle
tend to have high cohesion and are
more maintainable than classes that
take on multiple responsibilities and
have low cohesion.

===

Identify the following pattern:

"It allows you to
compose objects into tree structures to
represent part-whole hierarchies. This pattern
lets clients treat individual objects and
compositions of objects uniformly"

[HFDP]

---

The Composite pattern:

<img width="999" alt="image" src="https://user-images.githubusercontent.com/1868409/197761581-3ebe9865-867c-409a-a022-4843d2309971.png">