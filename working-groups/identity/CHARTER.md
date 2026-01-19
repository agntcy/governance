# AGNTCY Identity Working Group Charter

## Mission

The mission of this working group is to contribute to the definition of standards focused on identity in multi-agentic systems.

## Goals

The goals of this working group can be summarized as follows:

- Defining mechanisms enabling the assignment and onboarding of identities for agents, resources, and tools in an open way.

- Ensuring collision-free assignment and use of identities in multi-agentic systems.

- Defining methods enabling trustworthy assignment, onboarding, presentation, verification, and utilization of identities, including mechanisms to authenticate identifiers and their provenance.

- Addressing identity-centric requirements and standardization needs involving human-to-agent, agent-to-tool, agent-to-agent, and agent-to-human interactions.

- Promoting openness and interoperability across multi-agentic systems and ecosystems, including seamless integration with Identity Providers (IdPs), Auth Servers and standard AuthN/AuthZ flows.

- Enabling fine-grained, access controls for agents and tools, ensuring that permissions are scoped, time-bound, and auditable across multi-agentic interactions.

## Scope

This working group would be responsible of everything that is related to identity in multi-agentic systems, and will mainly contribute to the [identity](https://github.com/agntcy/identity) and [identity-service](https://github.com/agntcy/identity-service) repositories.

## Resources

- Meetings: [See AGNTCY Calendar](https://calendar.google.com/calendar/embed?src=admin%40ops.agntcy.org&ctz=America%2FNew_York)

- Repos:

    - [identity-spec](https://github.com/agntcy/identity-spec)
    - [identity](https://github.com/agntcy/identity)
    - [identity-service](https://github.com/agntcy/identity-service) 

- Discussion Channel: AGNTCY slack #wg-identity

- Roadmap: TBD

- Active Workstreams


| Sub Streams                    | Details                          | Leads             | GitHub ProfileMonth |
| ------------------------------ | -------------------------------- | ----------------- | ------------------- |
| 1. Dynamic client ID metadata integration | Exploring mechanisms for agents, MCP servers, and tools to dynamically register themselves, such as: (a) Dynamic Client Registration (DCR) as defined in OAuth 2.0 and OpenID Connect specifications; (b) Client ID Metadata (OAuth Client ID Metadata Document). This would reduce manual configuration and improve interoperability in distributed environments. | Ankit Agarwal (Skyfire) | https://github.com/skyfire-ankit |
| 2. Context Sharing | This Subgroup (SG) addresses subject context transfers and bindings enabling policy decisions across a delegated chain that may involve users, agents, and tools. Issues like how such contexts should be embedded into tokens and leveraged to inform policy decision points, enable fine-grained authorization, traceability, and compliance are within the scope of this SG. This SG will also identify relevant standards, other ongoing initiatives, and push for new specs for the gaps identified. | Marcelo Yannuzzi (Outshift by Cisco) | https://github.com/mayannuz |
| 3. Audit Logs Authorization | Defining standards for audit logging to capture critical data points such as intent, tasks, delegation chains, and related metadata. This would improve transparency, accountability, and support compliance or forensic analysis. Include privacy implications on what can be captured and should not be captured. | Alan Pinkert (Duo) | https://github.com/alanisaac |
| 4. Agentic Identity Interconnect | Establish liaisons and collaborative interplays with other ongoing initiatives within the Linux Foundation (LF) to ensure alignment and shared progress.Strengthen relationships, avoid duplication, and foster joint innovation across LF projects. | Sarah Evans (Dell) |  |
| 5. Brokered Identity Gateways | Enabling secure, seamless authentication across platforms through brokered identity and gateway integrations. | Manish Singh (Datum.net) |  |
| 6. Design Principles for Agentic Identity | Defining the design principles for trustable and interoperable digital Identities for Human and Agentic AI. | Debora Comparin (Thales) |  |