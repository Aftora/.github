<img src="https://github.com/Cascade-Panel/.github/blob/main/profile%2FScreenshot_20260220-041529.png" alt="Aftora Systems Banner" style="width:100%;height:auto;">

# Aftora Systems

Aftora Systems builds and operates operational software platforms across infrastructure orchestration and workforce management.

The organization focuses on clear system boundaries, secure-by-default architecture, and scalable, production-grade reliability.

---

## Platform Structure

Aftora Systems develops and maintains independent product platforms that integrate through well-defined interfaces.

Current product lines:

- **Cascade** — Distributed infrastructure orchestration
- **Cadence** — Workforce and operational management

Each platform is designed with separation of concerns, minimal cross-dependency, and long-term operational scalability.

---

## Cascade

Cascade is the distributed infrastructure platform developed by Aftora Systems.

It combines centralized orchestration with licensed node-level execution to manage:

- VPS environments
- Game servers
- Application hosting
- Database services
- Proxy and domain infrastructure

Cascade consists of two primary components:

### Conduit

The control plane responsible for orchestration, licensing, API surfaces, and system-wide coordination.

Repository:  
https://github.com/Cascade-Panel/Conduit

### Cascadia

The Rust-based licensed node runtime responsible for local workload execution and infrastructure operations.

Repository:  
https://github.com/Cascade-Panel/Cascadia

---

## Cadence

Cadence is the workforce management platform within Aftora Systems.

It provides:

- Employee management and role-based permissions
- Shift scheduling and recurring rota systems
- Clock-in/out workflows with overtime logic
- PTO request and approval processes
- Payroll automation and audit logging
- Internal operational communication tools

Cadence is built as a full-stack platform combining a Sanic API with a React dashboard.

Repository:  
https://github.com/Cascade-Panel/Cadence

---

## Engineering Principles

Aftora Systems builds platforms according to the following principles:

- Clear separation between orchestration and execution
- Secure communication and authentication by default
- License-based runtime validation where appropriate
- Auditability for privileged and financial operations
- Horizontal scalability across distributed deployments
- Long-term maintainability over short-term complexity

---

## Contribution

Each repository contains its own documentation and contribution guidelines.

Changes are reviewed per project and must align with platform architecture and security standards.

---

## Licensing

Licensing varies by repository.  
Refer to the LICENSE file in each project for applicable terms.
