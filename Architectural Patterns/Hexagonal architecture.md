# Hexagonal Architecture

https://en.wikipedia.org/wiki/Hexagonal_architecture_(software)




---
## dotGo 2019 - Kat Zień - Achieving maintainability with hexagonal architecture

<iframe width="560" height="315" src="https://www.youtube.com/embed/vKbVrsMnhDc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Visual Representation
- Primary actors(Ports & Adapters) on the left
- Secondary actors(Ports & Adapters) on the right

![[hexagonal_ports&adapters.png]]

### Dependency only points inwards 

The outer layer can call anything they like from the inner layers and they can reach out to the domain layer as much as they like, but they cannot reference anything outside of themselves. 

For dependencies going out like calling the database, we use [[Dependency Injection (DI)]] or [[Inversion of Control (IoC)]].

![[hexagonal_dependencies.png]]


### Testing each layer
![[hexagonal_testing.png]]

### Maintainability

- Consistent.
- Easy to understand, navigate and reason about. 
- Easy to change, loosely-coupled. 

---

