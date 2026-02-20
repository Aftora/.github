<img src="https://github.com/Cascade-Panel/.github/blob/main/profile%2Fbanner.png" alt="Cascade Banner" style="width:100%;height:auto;">

# Cascade Organization

Cascade is a platform organization building operational software across infrastructure orchestration and workforce management. The projects in this organization are designed with clear separation of responsibilities, secure-by-default architecture, and production-grade reliability.

---

## Product Architecture

Cascade is composed of distinct products that integrate through well-defined boundaries:

- Infrastructure orchestration is split between a centralized control plane and a licensed node runtime.
- Workforce operations are managed through a dedicated full-stack platform for scheduling and payroll.

This structure keeps execution isolated to the edge (nodes) where appropriate, while maintaining centralized orchestration, billing, and governance.

---

## Core Projects

### Conduit

Conduit is the control plane for the Cascade infrastructure platform. It coordinates licensed nodes, exposes the API surface used by the dashboard and integrations, and manages orchestration logic and system-wide state.

Responsibilities include:

- Node registration and license validation
- Workload orchestration and lifecycle management
- Proxy and domain configuration delegation
- API surface for UI and automation integrations

Repository: https://github.com/Cascade-Panel/Conduit

---

### Cascadia

Cascadia is the licensed node runtime daemon written in Rust. It executes infrastructure workloads locally on nodes and performs system-level operations delegated by Conduit.

Responsibilities include:

- VPS lifecycle management
- Game server provisioning and supervision
- Web and application hosting workloads
- Database host operations
- Proxy and domain execution
- Secure communication with the control plane

Repository: https://github.com/Cascade-Panel/Cascadia

---

### Cadence

Cadence is the workforce management platform within the Cascade ecosystem. It provides scheduling, time tracking, PTO workflows, payroll automation, and internal communications through a Sanic API and React dashboard.

Responsibilities include:

- Employee management and role-based permissions
- Shift scheduling with recurring patterns and cover workflows
- Clock-in/out with overtime rules and automated safeguards
- PTO approvals and reassignment tools
- Payroll automation with audit logging

Repository: https://github.com/Cascade-Panel/Cadence

---

## Design Principles

- Separation between orchestration and execution
- Secure-by-default communication and authentication
- Minimal central runtime responsibility where possible
- Auditability for privileged actions and financial workflows
- Scalability across distributed deployments

---

## Contributing

Contributions are reviewed per repository. See each project’s README for setup instructions and contribution guidelines.

---

## License

Licensing varies by repository. Refer to each project’s LICENSE file for the applicable terms.
