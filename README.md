# DPManager Deployment Requirements

![Last Revision](./assets/lastrevision.svg)


This document set describes the decisions, responsibilities, and setup information required before DPSolution can begin deploying DPManager in the customer’s Microsoft Azure and Fabric environment.

One of the most critical steps is agreeing with the customer on the names of all DPManager services, Azure and Fabric objects, and connections. Clear, consistent naming must be confirmed by the relevant stakeholders:

| Actor           | Responsibility                                             |
| --------------- | --------------------------------------------------------- |
| **Customer**    | Product owner representing the customer                   |
| **Customer IT** | Customer's IT team                                       |
| **Consultant**  | BI consultant team responsible for this customer         |
| **DPS**         | DPSolution is the provider delivering DPManager          |

Complete all customer-owned decisions and prerequisites, and provide the requested handoff information to your DPSolution contact before deployment begins.

## Table of Contents

### Initial Tasks
- [Tenant naming rule](./docs/01-Initial-Tasks/01-01-Tenant-naming-rule.md)
- [Tasks shared](./docs/01-Initial-Tasks/01-02-tasks-shared.md)

### Environment Tasks
- [Environment names](./docs/02-Environment-Tasks/02-01-Environemnt-names.md)
- [EntraID - How to DPManager app](./docs/02-Environment-Tasks/02-02-EntraID-howto-dpmanager-app.md)
- [EntraID - How to LoadMaster app](./docs/02-Environment-Tasks/02-03-EntraID-howto-loadmaster-app.md)
- [EntraID - How to create security group](./docs/02-Environment-Tasks/02-04-EntraID-howto-create-security-group.md)
- [Fabric preparation](./docs/02-Environment-Tasks/02-05-Fabric-preparation.md)

### Information for DPSolution
- [Information for DPSolution](./docs/06-information-for-dpsolution.md)

