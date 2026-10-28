# DPManager Deployment Requirements

This document set captures the information and setup required before DPSolution can begin deploying DPManager in your Microsoft Azure and Fabric environment. Complete the customer-owned decisions and prerequisites, then share the requested handoff information with your DPSolution contact.

## Start Here

1. Agree on the customer name and abbreviation with your team. Record the decision in [Environment naming](docs/01-environment-naming.md) before creating resources.
2. Agree on the environment name and abbreviation with your team. Record the decision in [Environment naming](docs/01-environment-naming.md) before creating resources.
3. Register the required applications and create the Entra ID groups in [Entra ID applications](docs/02-entra-applications.md) and [Entra ID groups](docs/03-entra-groups.md).
4. Create and configure the Fabric workspace and data assets in [Fabric workspace and data assets](docs/04-fabric-workspace-and-data.md).
5. Configure access for service principals and workspace users in [Fabric access](docs/05-fabric-access.md).
6. Complete [Information for DPSolution](docs/06-information-for-dpsolution.md) and provide it through the agreed secure channel.

## Customer Decisions

The customer owns the environment name and abbreviation. These values should be agreed before resource creation because they may be used in resource names, security groups, and deployment configuration. The customer also selects the Azure tenant, Fabric capacity/workspace, and the people who will administer access.

## Scope and Open Items

This is a preparation template, not a final permissions specification. DPSolution will confirm the exact application permissions, Fabric workspace roles, database access, connection authentication method, and any additional API-specific requirements before access is granted. Do not send passwords, client secrets, certificates, or other credentials in this document or by email.

## Prerequisite Summary

| Area | Required setup |
| --- | --- |
| Microsoft Entra ID | App registrations and service principals for `DPManager` and `Loadmaster`; agreed security groups |
| Microsoft Fabric | A workspace, one lakehouse, and SQL databases named `dpmu`, `bi_man`, and `loadmaster` |
| Fabric connections | A connection to the lakehouse and a connection to each of the three SQL databases |
| Access | Service-principal access to the required Fabric REST APIs and appropriate workspace access |
| Handoff | Environment details, tenant and resource identifiers, contacts, and confirmed setup status |

## Document Status

Use `Not started`, `In progress`, `Complete`, or `To be confirmed` for checklist items. Replace examples and bracketed placeholders with customer-approved values. Do not include secrets.
