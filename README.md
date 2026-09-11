**Platform reliability engineer building distributed ingestion and delivery systems.**
## @carmelaeisenbeisz
I build streaming ingestion and delivery systems around queues, workers, RPCs, and durable event schemas. I own the path from API boundary through persistence, retries, and operational recovery. I prioritize bounded queues, explicit backpressure, and recoverable state over short-lived performance gains. I accept operational complexity when it makes failures visible and contained.
### 🛠 Tech & Infrastructure
- **Core:** TypeScript, Node.js
- **Data:** PostgreSQL, Kafka
- **Infra:** Docker, Kubernetes
- **Tooling:** OpenTelemetry, Helm
### ⚙️ Engineering Areas
- Streaming ingestion and delivery with Kafka topics, partitions, offsets, and DLQs
- PostgreSQL schema evolution, indexes, migrations, and replay-safe consumers
- gRPC APIs and workers with idempotency keys, timeouts, and bounded retries
- OpenTelemetry traces, structured logs, and SLO-oriented alerting
### 🔭 Current Focus
- Splitting a monolithic consumer into ownership-based workers without duplicate delivery
- Backfilling Kafka records with a bounded concurrency model for a large topic
- Replaying PostgreSQL migrations into an ephemeral schema before promotion
- Tracing cross-service RPC failures without adding unacceptable sampling overhead
### 📌 Engineering Notes
- Tests should exercise boundaries with queues, RPCs, and persisted state, not only functions.
- Schema evolution should preserve old consumers until replay and rollback paths are proven.
- Migrations belong beside application code because rollback and recovery are part of the change.
- Retries need idempotency, deadlines, and circuit behavior; otherwise they amplify failures.
### 🧭 How I Work
- Prefer bounded queues and explicit backpressure over hidden buffering.
- Make failure modes visible before optimizing throughput.
- Treat operational recovery as part of the design review.
*I keep systems boring where they must be dependable and simple where they must change.*
[Email](mailto:carmelaeisenbeisz7153640@gmail.com)