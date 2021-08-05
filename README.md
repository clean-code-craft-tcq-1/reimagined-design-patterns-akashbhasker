# reimagined-design-patterns

Give a summary description of Four design patterns that you choose from the following design patterns: **Adapter,  Builder, Composite, Decorator, Observer, Interpreter, State, Mediator, Memento, Prototype, Proxy**. In your summaries say:

- what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example
- how the pattern works, what the basic idea of the pattern is
- what the main advantage and what the the main disadvantage is of using this pattern
- Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more). 

> Do not add diagrams, and do not try to give a complete description of the patterns as found in the books. Rather think of how you would explain the essential ideas of these patterns in a few sentences to a colleague while drinking coffee.

Pattern 1 : ADAPTER

Summary : Adapter helps to convert the interface of a class into another interface clients expect to make interactions between them compatible.
Similar to the Universal Adapter that we use in real life to Plug in Electical Pins of different country 

Where to Use : Mostly Used where we would like to reuse legacy Code for a new functionality , but the new functionality expects different interfaces
Example: A legacy Server is replaced with a new server with new interfaces, but the clients expect older interfaces. An adapter is added to solve the incompatability
How it Works : An adater class combines or redeines certain interfaces from one of the class to make it compatible with the other class through the adapter
Advantages : Helps avoiding any code change in the main classes , while still making them compatabile 

PATTERN 2 : PROXY
Summary : To Provide Controlled Access to an object , a proxy is used instead of direct access to the object. This helps to ensure object creation is done only when necessary and also limit the access when required
Where to Use : When There is a possibility of having multiple clients trying to access one server , a proxy can be used to ensure the clients requests the proxy and the proxy intern requests the server
Example: ATM access the Bank Server through a proxy
How it Works : A proxy class would be created for the Real class . A client object will request for functionaility of the real class through the Proxy Object
Advantages : Helps to ensure concurrency ,  access control and better memory management

PATTERN 3 : OBSERVER
Summary : Observer Pattern helps to achieve the requirement where clients need to be notified whenever there is a state change in the Observing Object
Where to Use : Used where clients required to be notified when there is a state change
Example: Users of an app , may want to know when a certain item becomes available. In such a case, the user ( client ) can register to become an observer for such an item. When the item becomes available, all the clients who have regsitered will get notified
How it Works : An observable class , allows clients to register to listen for updates. The observable class mainatins a list of all such registered clients and notifies them when there is state change
Advantages : Helps to manage the notification to N clients from 1 object

PATTERN 4 : STATE
Summary : State patters helps to solve the problem to perform different functionaility based on the current state of the system
Where to Use : When Different Actions need to be performed based on the current context , a state machine can be designed using the state pattern
Example: In Infotainment system , when a Key is pressed , based on the current state , necessary action can be performed
How it Works : All the possible states of an object will be defined . Based on certain triggers, the current state of the system will be changed by the State Manager. When a request comes in, based on the current state , required action can be performed
Advantages : Helps to limit the number of condition checks
