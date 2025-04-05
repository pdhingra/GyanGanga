
see [[Hexagonal Architecture]] and [[Onion Architecture]]

# Key things to note
1. Separation of concerns by dividing s/w into layers
2. Use Dependency Inversion and polymorphism to make domain layer most independent and stable.
3. Source code dependency can only point inwards toward domain layer.
4. Domain layer is independent of framework/UI/databases/external agencies.
5. Test domain layer without requiring external elements.
6. Domain layer contains entities and use cases for the domain logic
7. Similar to Hexagonal and Onion Architecture - isolate the domain

# Ports and Adapters

Primary [Driving] Adaptors are input adapters and Secondary are output adapters. 

Domain Logic is invoked using Primary Adapters, and then domain logic uses secondary layer to get external information, processes it, and response is passed to client using primary adapters.

- Good for Long lasting application

# Entities
objects contains the critical business rules. - validating the state of order, price is correct

use cases - application specific rules - having a discount on entity, user not exceeded the daily purchase limit.




