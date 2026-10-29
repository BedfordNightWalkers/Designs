# Diagram source

These diagrams are written in Mermaid.

- `architecture.mmd` — component relationships and main data stores.
- `sequence.mmd` — successful processing, idempotency, and failure paths.
- `failure-and-dlq.mmd` — retry, dead-letter, investigation, and replay flow.

The optional SQL outbox is shown as a recommended enhancement when audit events must reliably correspond to committed business transactions. If the actual implementation publishes directly from the API, update the diagram and explicitly document the delivery gap.
