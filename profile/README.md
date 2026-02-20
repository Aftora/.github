<img src="https://github.com/Cascade-Panel/.github/blob/main/profile%2Fbanner.png" alt="Cascade Banner" style="width:100%;height:auto;">

# Cascade Organization

Cascade is a distributed infrastructure platform focused on orchestrating licensed node runtimes at scale. The organization maintains the core components powering the Cascade ecosystem, including the control plane and node runtime responsible for managing VPS environments, game servers, application workloads, databases, and networking infrastructure.

Cascade is designed around a strict separation between orchestration and execution, enabling scalable, secure, and modular infrastructure deployments.

---

## Platform Architecture

Cascade is composed of two primary components:

Control Plane  
→ Secure API / WebSocket  
→ Licensed Node Runtime  
→ Local Infrastructure Execution  

The control plane coordinates workloads and system state.  
The node runtime executes infrastructure operations locally.

This separation ensures fault isolation, horizontal scalability, and minimal centralized execution risk.

---

## Core Projects

### Conduit

Conduit is the Cascade control plane.

It provides:

- Node registration and license validation  
- Infrastructure orchestration  
- Workload lifecycle management  
- API surface for frontend and automation integrations  
- Proxy and domain configuration delegation  
- System-wide state modeling  

Conduit does not directly execute infrastructure workloads. All runtime operations are delegated to licensed nodes.

Repository:  
https://github.com/Cascade-Panel/Conduit

---

### Cascadia

Cascadia is the licensed node runtime daemon written in Rust.

It is responsible for:

- VPS lifecycle management  
- Game server provisioning and supervision  
- Web application deployment  
- Database host management  
- Reverse proxy and domain execution  
- Secure communication with the control plane  

Cascadia executes all infrastructure operations locally while maintaining authenticated communication with Conduit.

Repository:  
https://github.com/Cascade-Panel/Cascadia

---

## Design Principles

- Clear separation between control and execution  
- Node-first runtime authority  
- Minimal control-plane data retention  
- Secure-by-default communication  
- Horizontally scalable architecture  
- Performance-focused engineering  

---

## Contribution

Contributions are reviewed per repository. Please refer to the individual project documentation for setup instructions and contribution guidelines.

---

## License

Unless otherwise specified, projects within the Cascade Organization are proprietary and licensed for use within the Cascade ecosystem.
