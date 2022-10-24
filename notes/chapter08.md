Identify the following pattern:

"It defines the skeleton
of an algorithm in a method, deferring some steps to
subclasses. This pattern lets subclasses redefine
certain steps of an algorithm without changing the
algorithm’s structure."

[HFDP]

---

Template Method Pattern

<img width="996" alt="image" src="https://user-images.githubusercontent.com/1868409/197513470-bf2174b5-a979-4f34-9d4b-a1a586e11ee6.png">

===

Explain actors involed in the template method pattern (2)

[HFDP]

---

- Abstract class: is responsible for defining the steps and methods that are common for all the algorithms and declaring as abstract methods those that differ.
- ConcreteClass: inherits from the abstract class and define the methods or steps that are unique for one algorithm.

===

In the template method pattern, what's a "hook"?

[HFDP]

---

A hook is a method that is declared in the
abstract class, but only given an empty or default
implementation. This gives subclasses the ability to
“hook into” the algorithm at various points, if they
wish; a subclass is also free to ignore the hook. 

<img width="931" alt="image" src="https://user-images.githubusercontent.com/1868409/197514463-ec9f7c8c-5c93-4a18-9274-eba8aae0d091.png">

===

Explain the following principle:

"The Hollywood Principle Don’t call us, we’ll call you."

[HFDP]

---

With the Hollywood Principle, we allow low-level components
to hook themselves into a system, but the high-level
components determine when they are needed, and how. In
other words, the high-level components give the low-level
components the “don’t call us, we’ll call you” treatment.

===

How does the Hollywood Principle relate to the
Dependency Inversion Principle that we learned a few chapters
back?

[HFDP]

---

The Hollywood Principle is a technique for building
frameworks or components so that lower-level components can be
hooked into the computation, but without creating dependencies
between the lower-level components and the higher-level layers.

===

What's the difference and similarity bettween the Template Method Pattern and the Strategy pattern?

[HFDP]

---

The Strategy and Template
Method Patterns both encapsulate
algorithms, the first by composition
and the other by inheritance.