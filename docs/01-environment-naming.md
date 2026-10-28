# Environment Naming

Complete this page first. The customer chooses and approves the environment name and abbreviation used for the DPManager deployment.

## Naming Decision

| Field | Customer value | Example only |
| --- | --- | --- |
| Customer name | [Enter value] | Contoso |
| Customer abbreviation | [Enter value] | Production |
| Environment name | [Enter value] | Production |
| Environment abbreviation | [Enter value] | prod |
| Region, if included in names | [Enter value or N/A] | eastus |

## Naming Convention

Document any naming rules the deployment must follow.

| Resource type | Pattern or rule | Example using the approved environment |
| --- | --- | --- |
| Entra ID app registrations | [Enter rule or use the standard names] | DPManager - prod |
| Entra ID security groups | [Enter rule] | [customer]-DPManager-prod-Operators |
| Fabric workspace | [Enter rule] | [customer]-DPManager-prod |
| Fabric lakehouse and SQL databases | [Enter rule or confirm the required names] | dpmu, bi_man, loadmaster |

## Confirmation

- [ ] Environment name and abbreviation are approved by the customer.
- [ ] Naming convention is compatible with customer policies and naming limits.
- [ ] The approved values will be used consistently in the remaining setup and handoff pages.

> Examples are illustrative only. Confirm all final names with the customer's platform and security teams.