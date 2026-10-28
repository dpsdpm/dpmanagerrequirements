# Microsoft Entra ID Groups

Create customer-managed security groups for controlling access. Agree on group names using the approved environment abbreviation. DPSolution will confirm which groups should be assigned to each application or Fabric resource.

## Group Register

| Group purpose | Proposed display name | Owner(s) | Intended members | Access to be granted | Status |
| --- | --- | --- | --- | --- | --- |
| Allow-list for service principals using Fabric APIs | [customer]-DPManager-[env]-FabricAPI | [Owner] | [Confirm whether app service principals can/should be included under tenant policy] | Fabric tenant setting scope; confirm exact applications | [Status] |
| DPManager workspace operators | [customer]-DPManager-[env]-Operators | [Owner] | [User or service-principal identities as confirmed] | Fabric workspace role to be confirmed | [Status] |
| DPManager workspace readers, if needed | [customer]-DPManager-[env]-Readers | [Owner] | [Users] | Fabric workspace role to be confirmed | [Status] |
| Additional customer support/admin group, if needed | [Enter approved name] | [Owner] | [Users] | [To be confirmed] | [Status] |

These are planning examples, not mandatory group names or a final access model. Remove groups that are not needed and add customer-required groups.

## Create a Security Group

An Entra administrator can create each approved group in the Microsoft Entra admin center:

1. Open **Identity > Groups > All groups** and select **New group**.
2. Select **Security** as the group type.
3. Enter the approved group name and description, and assign at least one customer-owned group owner.
4. Add only the members approved for that group's purpose. Do not assume service principals can be added to or used through a group in every configuration; confirm the supported assignment method with the Entra and Fabric administrators.
5. Create the group and record its object ID and status in the table below.

## Created Groups

| Display name | Group object ID | Owner confirmed? | Membership reviewed? | Status/date |
| --- | --- | --- | --- | --- |
| [Group name] | [Object ID] | [Yes/No] | [Yes/No] | [Status/date] |