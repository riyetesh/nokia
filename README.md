# CIVINET
### Resilient connectivity for connected communities

**CIVINET is a civic connectivity concept designed to help communities stay informed, connected and coordinated when conventional communication infrastructure becomes unreliable.**

It explores how telecom network intelligence, public infrastructure and local communities could work together to keep essential information moving during network disruptions and emergencies.

## The problem

When communication infrastructure is disrupted, communities can become isolated. Even when parts of a network remain operational:

- People may not know which communication routes are still available.
- Responders may lack visibility into disconnected communities.
- Public facilities with power and connectivity may remain underutilised.
- Critical messages may be sent without confirmation that they reached their recipients.
- Local resources can be difficult to coordinate across organisations.

Many emergency notification systems focus on broadcasting alerts. CIVINET explores a broader approach: making civic communication more adaptive, resource-aware and verifiable.

## The proposed approach

CIVINET brings network intelligence together with local civic infrastructure. It aims to identify available connectivity, discover alternative routes and help essential information reach communities through participating gateways and facilities.

### Core capabilities

| Capability | Description |
|---|---|
| **Connectivity intelligence** | Identifies network disruptions, weak coverage and potentially isolated communities. |
| **Community network map** | Visualises communication links, public facilities and local resources. |
| **Adaptive message routing** | Routes priority messages through available communication paths and participating gateways. |
| **Civic resource coordination** | Connects residents, volunteers, responders and institutions to coordinate essential resources. |
| **Delivery verification** | Tracks message delivery and acknowledgement to identify communities that remain unreached. |

## How it works

The concept follows a four-stage response process:

1. **Detect disruption** — Identify communication disruptions and determine which connections remain operational.
2. **Assess available resources** — Evaluate nearby facilities, participating gateways and alternative connectivity options.
3. **Reroute critical messages** — Prioritise essential information and route it through available communication paths.
4. **Verify community reach** — Monitor delivery acknowledgements and identify locations or communities that remain disconnected.

## Interactive demonstration

The website includes a browser-based simulation of how CIVINET could respond to a network disruption.

The demonstration includes:

- A visual network topology.
- Simulated network outages and changing node states.
- A staged response workflow with automatic progression.
- Pause, next-stage and reset controls.
- A system activity feed showing simulated events.

**The current demonstration uses simulated data. It does not connect to live telecom infrastructure or real Nokia network APIs.**

## Proposed technical architecture

CIVINET is envisioned as five cooperating layers:

1. **Network intelligence layer** — Receives network status and connectivity information from participating telecom operators.
2. **Infrastructure intelligence layer** — Integrates information about participating public facilities, power availability and communication gateways.
3. **Routing and orchestration layer** — Evaluates available communication paths and selects routes based on message priority and network conditions.
4. **Community coordination layer** — Provides interfaces for residents, volunteers, emergency responders and public institutions.
5. **Verification and monitoring layer** — Tracks message delivery, acknowledgements and communities that remain unreachable.

## Potential Nokia integration

Nokia's expertise in telecommunications infrastructure, network orchestration and programmable network capabilities could provide a foundation for parts of CIVINET.

Potential integration opportunities include:

- Nokia Network as Code and supported operator APIs.
- Quality-on-Demand capabilities, where available.
- Network location and presence capabilities, where supported and permitted.
- Network monitoring and connectivity intelligence.

Access to operator APIs, public infrastructure data and community gateways would depend on technical availability, permissions and partner agreements. These are proposed integration directions, not implemented integrations in the current prototype.

## Technology direction

The current prototype is a standalone browser-based interface. A future implementation could explore the following technologies:

| Component | Potential technology |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Network API integration | Nokia Network as Code / operator APIs |
| Backend services | Python / FastAPI or Node.js |
| Real-time communication | WebSockets, MQTT |
| Geospatial visualisation | Map-based visualisation tools |
| Alternative connectivity | Participating gateways, mesh and store-and-forward mechanisms |
| Data management | PostgreSQL / PostGIS |

These are possible implementation choices, not a claim that every component is currently deployed.

## Getting started

Clone the repository:

```bash
git clone https://github.com/riyetesh/nokia.git
cd nokia
```

Open `index.html` in a modern browser.

Alternatively, run a local development server:

```bash
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000).

No backend or API credentials are required to explore the current simulation.

## Project status

**Current stage: Interactive concept prototype**

| Feature | Status |
|---|---|
| CIVINET website | Implemented |
| Network topology visualisation | Implemented |
| Simulated disruption scenarios | Implemented |
| Staged response simulation | Implemented |
| Simulated message-routing workflow | Demonstrated |
| Live telecom network integration | Not implemented |
| Real message delivery and acknowledgement | Not implemented |
| Physical mesh / gateway deployment | Not implemented |

## Vision

Communication resilience should not depend on a single network, platform or institution.

CIVINET explores how telecommunications infrastructure and local communities could work together to create a more adaptive civic communication ecosystem.

**When one connection fails, the community should not disappear from the network.**

---

**Repository:** [github.com/riyetesh/nokia](https://github.com/riyetesh/nokia)  
**Project:** CIVINET  
**Context:** Nokia hackathon concept prototype
