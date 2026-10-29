# Designs — Software Architecture Portfolio

A collection of practical software architecture and system design examples, focused on .NET, Azure, distributed systems, API security, and reliability.

> **Status:** Reference design / learning project. This repository describes a proposed architecture and its trade-offs; it should not be presented as a production deployment unless it has actually been implemented and operated.

## Designs

### [Azure Distributed Audit Logging](./AuditLogging/README.md)

An asynchronous, multi-tenant audit pipeline that decouples the transactional application from audit persistence using Azure Service Bus Topics, Azure Functions, Azure Cosmos DB, and Azure Blob Storage.

**Topics covered:** event-driven architecture, durable messaging, idempotent consumers, large payloads, tenant isolation, retries, dead-letter queues, observability, and operational recovery.

## How to use this portfolio

Each design aims to explain:
- the problem and requirements;
- the architecture and event flow;
- the key design decisions and alternatives;
- failure modes and recovery;
- security, scalability, and operational considerations.

Diagrams are stored as Mermaid source (`.mmd`) so they can be reviewed and version-controlled. GitHub can render Mermaid diagrams in Markdown; standalone `.mmd` files can also be previewed in Mermaid-compatible tools.

## Disclaimer

Examples are illustrative. Validate service limits, pricing, security controls, retention requirements, and operational procedures against the target environment before production use. Do not commit credentials, connection strings containing secrets, customer data, or confidential employer information.
