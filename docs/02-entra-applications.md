# Microsoft Entra ID Applications

Register two applications in the customer's Microsoft Entra tenant. Each app registration has an associated service principal (enterprise application) in that tenant. The exact permissions and credential method must be confirmed with DPSolution before granting access.

## Applications to Register

| Application display name | Purpose | App (client) ID | Service principal created? | Status |
| --- | --- | --- | --- | --- |
| DPManager | DPManager service-to-service identity | [Enter ID after registration] | [Yes/No] | [Status] |
| Loadmaster | Loadmaster service-to-service identity | [Enter ID after registration] | [Yes/No] | [Status] |

Use the approved naming convention from [Environment naming](01-environment-naming.md). `DPManager` and `Loadmaster` are the default names; add an environment suffix only if the customer naming policy requires it and DPSolution confirms the resulting names.

## Registration Checklist

For each application:

- [ ] Confirm the target tenant and environment with the customer Entra administrator.
- [ ] Create an app registration in that tenant using the agreed display name and supported account type.
- [ ] Confirm the corresponding service principal (enterprise application) exists in the tenant.
- [ ] Record the tenant ID, app (client) ID, and service principal object ID in [Information for DPSolution](06-information-for-dpsolution.md).
- [ ] Do not grant API permissions or create credentials until DPSolution confirms the required permissions and authentication approach.
- [ ] If credentials are required, create and deliver them only through a customer-approved secrets-management channel. Never add credential values to this repository or handoff document.

## Permission Confirmation

Complete this section with DPSolution and the customer's security administrator before granting permissions.

| Application | API/resource | Permission type (delegated/application) | Permission(s) | Admin consent required? | Confirmed by/date |
| --- | --- | --- | --- | --- | --- |
| DPManager | [To be confirmed] | [To be confirmed] | [To be confirmed] | [To be confirmed] | [Pending] |
| Loadmaster | [To be confirmed] | [To be confirmed] | [To be confirmed] | [To be confirmed] | [Pending] |

> Do not infer permissions from the application name. The required permissions depend on the deployment design and the Fabric API operations in use.