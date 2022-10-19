Explain how to implement the singleton pattern in most languages (3)

[HFDP]

---

- We need to have a class or module and declare a var or attribute that will hold our unique instance
- We need to declare our constructor as private so, only our class will be able to call it
- We expose a public (and static) method. This method should call the private constructor if the unique instance doesn't exist, otherwise should return the one already created

===

Identify the following pattern:

"It ensures a class has only one instance, and provides a global point of access to it."

[HFDP]

---

The Singleton Pattern

===

When working with singletons, how can prevent problems that can occur when dealing with multi-threading scenarios, where multiple instances might be created?

[HFDP]

---

Usually, the singleton class creates the unique instance lazily, this means that it will create it the first time the singleton method is called. So one way to mitigate the given problem, is to create the singleton instance early, before any thread creation happens, so we ensure our threads will never create the singleton instance.