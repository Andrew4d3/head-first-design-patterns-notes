Identify the following design pattern:

"It defines a one-to-many
dependency between objects so that when one
object changes state, all of its dependents are
notified and updated automatically"

[HFDP]

---

The Observer Pattern:

<img width="566" alt="image" src="https://user-images.githubusercontent.com/1868409/195331317-9060f7ec-1e83-4e96-aaa0-cdaf1be97cda.png">

===

Explain actors involded in the observer pattern (2)

[HFDP]

---

- Subject: object that holds the state and notify observer when a change happens
- Observers: objects that are dependant to the subject. They subscribe to the subject and get notified when a change happens on it

<img width="675" alt="image" src="https://user-images.githubusercontent.com/1868409/195334661-07f41102-a791-4f79-b0b5-627b63ea2d42.png">

===

What does it mean that two objects are loosely couple?

[HFDP]

---

When two objects are loosely coupled, they can interact, but they typically have very little knowledge
of each other.

===

Explain how the following principle applies to the observer pattern:

"Strive for loosely coupled designs between objects that interact."

[HFDP]

---

- We can add new observers at any time
- We never need to modify the subject to add new types of observers
- Changes to either the subject or an observer will not affect the other