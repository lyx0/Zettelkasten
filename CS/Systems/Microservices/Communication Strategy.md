# Communication Strategy
Created: 2021-08-07 09:12

Microservices communicate asynchronously.
- Services communicate with each other using events.
- The goal of the 'Event Bus' is to handle little notifications emitted from our different services.
- Each service can either emit or receive events from the event bus.
- Those notifications are like little notes that descirbe something that needs to happen inside our overall application. Is a point of failure so needs to be extremely robust.

 Pros and Cons of Async:
 - Pro:
	- No dependencies on other services.
	- Service X will be really fast.
- Con:
	- Data duplication, ~~more cost for storage~~. (is tiny)
	- Harder to understand.

## References
1. [[What are microservices?]]
2. [[Big Challenges]]
3.  [[CS/Systems/Monolithic Server/Communication Strategy]]