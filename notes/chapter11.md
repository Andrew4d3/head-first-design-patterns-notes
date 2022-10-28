Identify the following pattern:

"It provides a surrogate or
placeholder for another object to **control access** to it"

[HFDP]

---

The proxy pattern

<img width="822" alt="image" src="https://user-images.githubusercontent.com/1868409/198268733-ec3360c8-544b-4e53-882b-6691144a059d.png">

===

Explain actors involed in the proxy pattern (2)

[HFDP]

---

- Real Subject: is the object that does the real work.
- Proxy: implements the same interface as the real subject, and control access to it

===

What's the difference between Decorator pattern and the proxy pattern?

[HFDP]

---

Their purposes are
different: a decorator adds behavior to
a class, while a proxy controls access
to it. 

===

How can we force the client code to use the proxy rather than the real subject?

[HFDP]

---

One common technique is to provide a factory that instantiates and returns the subject.
Because this happens in a factory method, we can then wrap the subject with a proxy before returning it. The client never knows or cares that it’s using a proxy instead of the real thing.

===

Is there a way to add caching to a proxy instance?

[HFDP]

---

Yes, here we are talking about a
specialized form of a Virtual Proxy
called a Caching Proxy. A caching proxy
maintains a cache of previously created
objects and when a request is made it
returns a cached object, if possible.

===

How can we add authorization to methods in our classes using design patterns?

[HFDP]

---

This is a perfect example of where we might be able to use a
**Protection Proxy**. What’s a Protection Proxy? It’s a proxy that controls
access to an object based on access rights.