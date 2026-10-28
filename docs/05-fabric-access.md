# Microsoft Fabric Access

Configure the access required for the DPManager and Loadmaster service principals to call Microsoft Fabric REST APIs and access the deployment workspace. Coordinate changes with the customer's Fabric and Entra administrators. Apply least privilege and use the exact access model confirmed by DPSolution.

## Allow Service Principals to Use Fabric APIs

Fabric tenant settings are managed by a Fabric administrator. The setting names and available scopes can vary as Microsoft updates the portal; verify the current labels in the tenant before changing them.

1. In the Fabric portal, open **Settings > Admin portal > Tenant settings**.
2. Locate the developer/API setting that allows service principals to use Fabric APIs. Confirm the current setting name in the portal.
3. Enable it only for the approved security group or scope, where the tenant setting supports scoping. Do not enable it for the entire organization unless the customer security administrator explicitly approves that choice.
4. Add the required service principals or approved security group according to the tenant's supported configuration.
5. Save the setting and allow time for the change to take effect.
6. Record the setting scope, group, approver, and date below. Validate the required API operations with DPSolution.

| Setting | Scope/group | Applications included | Approved by/date | Status |
| --- | --- | --- | --- | --- |
| Service principals can use Fabric APIs | [Group/scope] | DPManager, Loadmaster, as confirmed | [Approver/date] | [Status] |

This tenant setting enables the service-principal scenario; it does not by itself grant access to every workspace or API operation. Some APIs may have additional requirements. Confirm endpoint-specific requirements and any separate admin API settings with DPSolution before enabling them.

## Grant Workspace Access

1. Open the target Fabric workspace and select **Manage access** (or the current equivalent in the portal).
2. Add the approved Entra security group(s) and/or service principals, using the supported identity type and assignment method for the tenant.
3. Assign only the workspace role(s) DPSolution has confirmed. Do not assume a role based solely on the examples below.
4. Confirm the DPManager and Loadmaster identities can perform only the required operations, and record the granted role and approver.

| Identity/group | Application | Workspace | Assigned role | Approved by/date | Validated? |
| --- | --- | --- | --- | --- | --- |
| [Identity or group] | DPManager | [Workspace] | [To be confirmed] | [Approver/date] | [Yes/No] |
| [Identity or group] | Loadmaster | [Workspace] | [To be confirmed] | [Approver/date] | [Yes/No] |

## Validation

- [ ] Fabric API tenant setting is enabled for the approved scope.
- [ ] Both required service principals are present in the correct tenant.
- [ ] Workspace access has been granted using the confirmed role and identity assignment method.
- [ ] Connection and API access have been tested without placing credentials in this repository.
- [ ] Customer security owner and DPSolution have reviewed the final access configuration.