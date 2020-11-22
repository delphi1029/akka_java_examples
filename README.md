# What is Actor Model?
Conceptual model of concurrent computation.It defines some general rules for how the system’s components should behave and interact with each other. 

# What is an Actor?
An actor is the primitive unit of computation. It’s the thing that receives a message and do some kind of computation based on it.

The idea is very similar to what we have in object-oriented languages: An object receives a message (a method call) and does something depending on which message it receives (which method we are calling).
The main difference is that actors are completely isolated from each other and they will never share memory. It’s also worth noting that an actor can maintain a private state that can never be changed directly by another actor.

* Each actor has its own thread.
* Actors won't share data.
* One actor can send messages to another actor.
* These messages must be immutable.
* Messages are processed by the actor one at a time.
