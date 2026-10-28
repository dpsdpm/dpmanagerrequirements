# Microsoft Fabric Workspace and Data Assets

Create the workspace and its required data assets in the customer-selected Fabric capacity and environment. Confirm names and region/capacity requirements with the customer before creation.

## Workspace and Assets

| Item | Required name | Customer value or identifier | Owner | Status |
| --- | --- | --- | --- | --- |
| Fabric workspace | [Approved environment-specific name] | [Workspace ID / URL] | [Owner] | [Status] |
| Lakehouse | [Approved name] | [Item ID / URL] | [Owner] | [Status] |
| SQL database | `dpmu` | [Item ID / connection details shared securely] | [Owner] | [Status] |
| SQL database | `bi_man` | [Item ID / connection details shared securely] | [Owner] | [Status] |
| SQL database | `loadmaster` | [Item ID / connection details shared securely] | [Owner] | [Status] |

## Setup Checklist

- [ ] Confirm the customer has a Fabric tenant and suitable capacity/licensing for the planned deployment.
- [ ] Create a Fabric workspace in the agreed capacity and region, using the approved environment name.
- [ ] Create a lakehouse in that workspace.
- [ ] Create the `dpmu`, `bi_man`, and `loadmaster` SQL databases in that workspace.
- [ ] Confirm the customer-approved identity and authentication method for each connection with DPSolution.
- [ ] Create and test a Fabric connection to the lakehouse.
- [ ] Create and test a Fabric connection to each SQL database: `dpmu`, `bi_man`, and `loadmaster`.
- [ ] Record non-secret identifiers and connection metadata in [Information for DPSolution](06-information-for-dpsolution.md).

## Fabric Connections

Record one row for each connection. Never record passwords, tokens, private keys, or secret values here.

| Source item | Fabric connection name | Authentication method | Identity/owner | Connection ID (if available) | Test/status |
| --- | --- | --- | --- | --- | --- |
| Lakehouse | [Name] | [To be confirmed] | [Identity] | [ID] | [Status] |
| `dpmu` SQL database | [Name] | [To be confirmed] | [Identity] | [ID] | [Status] |
| `bi_man` SQL database | [Name] | [To be confirmed] | [Identity] | [ID] | [Status] |
| `loadmaster` SQL database | [Name] | [To be confirmed] | [Identity] | [ID] | [Status] |

> If a database or connection type is unavailable in the selected Fabric region or capacity, pause and confirm the supported architecture with DPSolution before substituting a different asset type.