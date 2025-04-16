**Service-Oriented Architecture**

---

If you bring service-oriented architecture (SOA) up in a conversation, there’s a good chance someone will tell you that sounds a great idea. SOA is a way to design software systems by breaking them into **independent services** that communicate over a network. By using a solid approach within [[Software Architecture]], chopping the giant monolith program, transforming a masive system into a huge amount of services

Service-Oriented Architecture (SOA) is a software organize approach where services are provided to other components via network(typically via web protocols like HTTP, SOAP, or REST). These services are self-contained, modular business functions that can be reused across different systems.

---
# Key Characteristics of SOA

1. **Service Reusability**: Services are designed to be reused in different contexts
    
2. **Interoperability**: Services can communicate across different platforms and languages
    
3. **Loose Coupling**: Services maintain relationships that minimize dependencies
    
4. **Abstraction**: Service implementations are hidden from consumers
    
5. **Composability**: Services can be assembled into higher-level business processes
    
6. **Autonomy**: Services have control over the logic they encapsulate
    
7. **Discoverability**: Services can be discovered via a registry (like UDDI)

---

## SOA vs. Microservices

While **Microservices** is an evolution of SOA, key differences include:

- **SOA** often uses an **Enterprise Service Bus (ESB)** for communication.
    
- **Microservices** prefer **lightweight protocols (REST/gRPC)** and **API Gateways**.
    
- **SOA** services are larger (coarse-grained); **Microservices** are smaller (fine-grained).