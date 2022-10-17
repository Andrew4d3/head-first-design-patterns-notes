Design Principle: Classes should be open for extension, but closed for modification.

Explain how this design principle is related to "favor object composition instead of inheritance"

[HFDP]

---

By dynamically composing objects, I can add new functionality by writing new code and encapsulating this code into a new object referenced by our main class.  Because I’m not changing existing code, the chances of
introducing bugs or causing unintended side effects in pre-existing code are much reduced.

===

What do we get when we apply the open-closed principle? (2)

[HFDP]

---

We get designs that are (1) resilient to change and (2) flexible enough to take on new
functionality to meet changing requirements.

===

Identify the following design pattern:

"It attaches additional responsibilities to an object dynamically in order to extend functionality"

[HFDP]

---

The Decorator Pattern

<img width="1156" alt="image" src="https://user-images.githubusercontent.com/1868409/196160038-c66446ee-f44b-4f5e-a209-583b30ad3b4f.png">
<img width="1183" alt="image" src="https://user-images.githubusercontent.com/1868409/196160670-fa25bf3b-aea2-4001-b3e1-568d65be04e3.png">

