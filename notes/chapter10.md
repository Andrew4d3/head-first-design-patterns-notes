Identify the following pattern:

"It allows an object to alter its behavior
when its internal state changes. The object will appear to
change its class."

[HFDP]

---

The State pattern:

<img width="1004" alt="image" src="https://user-images.githubusercontent.com/1868409/198012288-04935534-0bbf-407d-9ae9-03a05ee1ad97.png">
<img width="1050" alt="image" src="https://user-images.githubusercontent.com/1868409/198012659-cfc898d2-6ab3-42ca-ac0d-7ad2d6970f0e.png">

===

Explain actors involed in the state pattern (2)

[HFDP]

---

Context: holds the current state and is responsible to delegate transitions to the current state.
State: handles the requests sent by the context. Each concrete state should implement the same interface, but only the methods that make sense should do something.

===

Can we use an abstract class instead of an interface to define our state methods?

[HFDP]

---

In your own implementation, you might want to consider an abstract
class. Doing so has the benefit of allowing you to add
methods to the abstract class later, without breaking the
concrete state implementations