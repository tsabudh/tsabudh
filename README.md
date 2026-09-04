# Sabudh Thapa

backend / distributed systems engineer · Kathmandu, Nepal

**I build the plumbing behind reliable products.**

I own the backend and data infrastructure of a production financial-data platform: event-driven workers, PostgreSQL and DuckDB data paths, and the recovery paths that keep data correct under load, retries, and partial failure. Software engineer in Kathmandu, Nepal, backend work since 2022.

## What I build

**Service-oriented backend systems**
APIs, workers, database-backed workflows, and service boundaries. Billing and entitlements built as data rather than code, so a second payment provider needs no schema change.

**Idempotent job processing**
One Kafka backbone with Avro schemas for data operations, workflows, and notifications. Idempotent producers, DLQ replay, ordered shutdown, and correlation-ID tracing across workers.

**Data that stays correct under failure**
Identity resolution as its own layer: canonical records rebuilt nightly across ~6,000 companies with weighted source precedence and append-only provenance, so a bad source can be retracted.

**Queries shaped for the data they read**
Screener serving moved from PostgreSQL row-store plans to DuckDB over S3-backed Parquet. Nearly 100 freely combinable metrics, custom ranges under 600ms, down from 8-22s.

**Recovery engineering and auditability**
84 GB of production PostgreSQL cut over from Neon to RDS with ingestion never stopped. Structured logs draining to S3 as Parquet after undrained container logs took Redis down.

## Notes

- [When Indexes Stop Helping: Columnar Engines](https://tsabudh.com.np/blog/when-indexes-stop-helping-columnar-engines/)
- [Indexing Is Query Design, Not Column Decoration](https://tsabudh.com.np/blog/indexing-is-query-design-not-column-decoration/)
- [Why Your App Slows Down When Users Increase](https://tsabudh.com.np/blog/why-your-app-slows-down-when-users-increase/)
- [Backpressure playground](https://tsabudh.com.np/systems/backpressure/), a Rust/WASM model of event flow under failure

## Stack

TypeScript, Node.js, Fastify · Python · Rust · PostgreSQL · Kafka, Avro · Redis · DuckDB, Parquet, S3 · Docker, AWS · OpenTelemetry

[tsabudh.com.np](https://tsabudh.com.np) · [Resume](https://tsabudh.com.np/resume/) · [LinkedIn](https://linkedin.com/in/tsabudh) · tsabudh@gmail.com
