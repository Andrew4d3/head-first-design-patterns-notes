Explain actors involded in the command pattern (3)

[HFDP]

---

- Command object: encapsulates the actions that are delegated to the receiver once the executed method is called
- Receiver: is bound to the command object and knows how to perform the work needed to carry out the request
- Invoker: holds one or several commands and it's responsible to call the execute method of one command when needed.


===

Identify the following pattern:

"It encapsulates a request as an object, thereby letting you parameterize other objects
with different requests, queue or log requests, and support undoable operations."

[HFDP]

---

The command pattern

<img width="1050" alt="image" src="https://user-images.githubusercontent.com/1868409/196680486-8cfaa835-31a4-4511-bf93-eb47691adddd.png">


===

In summary, how do we implement the command pattern? (3)

[HFDP]

---

- The client creates a command object.
- The client does a setCommand() to store the command object in the invoker.
- Later...the client asks the invoker to execute the command.

===

How can we implement an "empty" command?

[HFDP]

---

This is called **null object**. A null object is useful when
you don’t have a meaningful object to return, and yet you want to remove the
responsibility for handling null from the client. For instance, in our remote control we
didn’t have a meaningful object to assign to each slot out of the box, so we provided
a NoCommand object that acts as a surrogate (substitute) and does nothing when its execute()
method is called.

So instead of doing something like this:

<img width="493" alt="image" src="https://user-images.githubusercontent.com/1868409/196933984-e523b98d-f953-4c22-a86f-d0d538aac94f.png">

We can do something like this:

<img width="496" alt="image" src="https://user-images.githubusercontent.com/1868409/196934026-7360d3f3-fcdd-4616-815e-1f7e0506550a.png">

And now we don't have to verify that the given object is null.

===

In the command pattern, is the receiver always necessary?

[HFDP]

---

Not really, in practice, it’s not uncommon for “smart” Command objects to
implement the request themselves rather than delegating to a receiver.