# verbal-remedies
There’s a lot of jargon in coding that doesn’t make sense to a non-coder or a newcomer. That’s no fun because such jargon intimidates people from making the jump into the wonderful world of code!

That’s why I’m translating a bunch of terms that come up a lot in tech literature and conversations…I want you to learn how to code!

# The terms

algorithm invariant  
amortized analysis 

**ASYNCHRONOUS:** Refers to events (often function calls) that happen "out of sync". For example, normally when you call a function `foo`, the computer runs the code in `foo` before proceeding to the next line (or the next _expression_) after the call to `foo`. If `foo` is an _asynchronous function_, then the computer does not finish waiting for the function to "fully execute" before proceeding on to whatever's after the call to `foo`. This is a common pattern in [Node.js](https://nodejs.org), for example, where most function calls are asynchronous, and each is given a _callback_ function that gets run when the function finishes executing. Where does the actual computation of the function occur? Normally it occurs on a background _thread_ (a "lightweight process") that's processing _events_ on an _event queue_, but it can also be done in a single thread using a _run loop_ that checks the status of a system queue (see [libevent](http://libevent.org)).

bulletproof code  
casting  
composition  
concurrency  
covariant  

**DEPLOYMENT**: all of the activities that make a software system available for use. (Credit: [Wikipedia](https://en.wikipedia.org/wiki/Software_deployment).) Separate from tasks such as editing content, designing an interface, or coding the functionality of a software project, deployment is often a final stage and the specific process of pushing or publishing a software project to an access point for others to use.

**DRY**: Acronym for "Don't repeat yourself" which is the concept that there should not be multiple instances of code accomplishing the same task. The primary ways to achieve this is to emphasize modularity where functions/methods typically accomplish one thing very well. [More info](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)
  
expressive  
eviction  
Extract/Transform/Load (ETL)  
fault tolerance  
fuzzing  
Hindley-Milner  
homoiconicity  
idempotence  

**IDIOMATIC**: Code written in the accepted style of its language community. For example, Ruby code written with a `for` loop would likely be unidiomatic because usage of methods from [Enumerable](http://ruby-doc.org/core-2.3.1/Enumerable.html) is preferred by most Ruby developers. Idiomatic code is often considered easier to read.

immutability  
interface  
invalidation  
iterable  
iterator  
load balancing  
loose coupling high cohesion  

**MARSHALLING**: Any mechanism for transforming an object into bytes for transmission or storage such that an equivalent instance of that object can be reconstituted elsewhere or at a later time. Marshalling is similar to serialization and the terms may be used interchangeably by some languages. Examples of marshalling include Python's [pickle](https://docs.python.org/3/library/pickle.html), Ruby's [Marshal](http://ruby-doc.org/core-2.3.0/Marshal.html), and Java's [Serializable interface](https://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html). 

memoization  
module  
mutable API  
MVC (Model/View/Controller)  
MVCC (Multiversion concurrency control)  
MVP (Model/View/Presenter)  
MVVM (Model/View/ViewModel)  
observable  
observer  
orthogonal  
paradigm  
performant  

**PIPE/PIPING/PIPELINE**: A metaphor from plumbing, a _pipe_ or _pipeline_ is a way of connecting the output of one program (a _stream_) as the input to another program. The act of constructing a pipeline is _piping_ and the `|` character is called _pipe_ after its usage to construct pipelines in the Unix shell. The pipe concept is used in many data processing systems.

principle of least surprise  
reification  

**SERIALIZATION**: The process of converting data into a known format that can be transfered or stored. In contrast to marshalling, serialization typically implies converting objects into a simpler, data-only representation (though the terms may be used interchangeably by some languages). There are [dozens of serialization formats](https://en.wikipedia.org/wiki/Comparison_of_data_serialization_formats) with different tradeoffs. For example, [JSON](https://en.wikipedia.org/wiki/JSON) is human-readable and flexible but verbose, while [Protocol Buffers](https://en.wikipedia.org/wiki/Protocol_Buffers) are compact and require a schema be defined.

single responsibility  
single source of truth

**STAGING**: The testing process - and often an entire environment - that allows review of a software project. A virtual "kicking of the tires," staging a project typically happens in a private, test environment where it can be put through some simulated, real-world-like use as a way to avoid unpredicted failures. Staging often happens as the step before deploying or publishing software to a non-test, production environment.

state machine
sticky load balancing
synchronous    
(syntactical) sugar  
TDD/BDD  
thread safe  
void (js)  

**YAGNI**: An acronym that stands for "You aren't gonna need it." Following
this principle, a developer shouldn't add something to their code until it's
actually necessary. This is to prevent developers from focusing too much
energy on areas they *think* might be important in the future, but which
ultimately turn out to be superfluous to the end product.

# Other resources

[A lightning quick reference for jargon](https://twitter.com/searls/status/609521655405113344)  
[A less quick reference (specific to Javascript)](https://github.com/HugoGiraudel/SJSJ)  
[The Jargon File - Glossary of Hacker Terms](http://www.catb.org/jargon/html/go01.html)  
[Useful Glossaries for Web Designers and Developers](https://www.smashingmagazine.com/2009/05/useful-glossaries-for-web-designers-and-developers/)  
[Skillcrush's Lexicon of 99 Tech Terms](http://skillcrush.com/2015/03/26/99-tech-terms/)  
[Functional Programming Jargon](https://github.com/hemanth/functional-programming-jargon)  
