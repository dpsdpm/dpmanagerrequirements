# Microsoft Entra ID Groups

The necessary groups 





| [customer]-DPManager-[env]-FabricAPI | [Owner]  | Fabric tenant setting scope; confirm exact applications | [Status] |
| [customer]-DPManager-[env]-Operators | [Owner]  | Fabric workspace role to be confirmed                   | [Status] |
| [customer]-DPManager-[env]-Readers   | [Owner]  | Fabric workspace role to be confirmed                   | [Status] |
| [Enter approved name]                | [Owner]  | [To be confirmed]                                       | [Status] |

These are planning examples, not mandatory group names or a final access model. Remove groups that are not needed and add customer-required groups.

## Create a Security Group

An Entra administrator can create each approved group in the Microsoft Entra admin center:

1. Open **Identity > Groups > All groups** and select **New group**.
2. Select **Security** as the group type.
3. Enter the approved group name and description, and assign at least one customer-owned group owner.
4. Add only the members approved for that group's purpose. Do not assume service principals can be added to or used through a group in every configuration; confirm the supported assignment method with the Entra and Fabric administrators.
5. Create the group and record its object ID and status in the table below.

## Created Groups

| Display name | Group object ID | Owner confirmed? | Membership reviewed? | Status/date   |
| ------------ | --------------- | ---------------- | -------------------- | ------------- |
| [Group name] | [Object ID]     | [Yes/No]         | [Yes/No]             | [Status/date] |