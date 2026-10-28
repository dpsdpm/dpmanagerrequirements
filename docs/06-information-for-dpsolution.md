# Information for DPSolution

Complete this handoff with customer-approved, non-secret information. Share it through the secure channel agreed with DPSolution. Do not include passwords, client secrets, certificates, tokens, private keys, or other credentials.

## Customer and Environment

| Parameter | Description | Mandatory | Value / Example |
| --- | --- | --- | --- |
| Customer name | Legal name for the customer. | yes | Contoso |
| Customer abbreviation | Customer-approved short value used in naming and configuration. | yes | cont |
| Environment name | Customer-approved name for the environment associated to this deployment. | yes | Development |
| Environment abbreviation | Customer-approved short value used in naming and configuration. | yes | dev |
| Azure region | Region selected by the customer, if applicable to the deployment. | yes | East US |
| Tenant ID | GUID of Microsoft Entra tenant identifier containing the app registrations. | yes | *guid-necessary-to-inform* |

## Microsoft Entra ID

### Service Principals

It is important to inform the information of the service principals that should be already registered in Entra ID.

| Parameter | Description | Mandatory | Value |
| --- | --- | --- | --- |
| DPManager Client ID | GUID of DPManager service principal. | yes | *guid-necessary-to-inform* |
| DPManager Client Name | Name of DPManager service principal. | yes | *necessary-to-inform* |
| DPManager Client Secret | Secret of DPManager service principal. | yes | *necessary-to-inform* |
| Loadmaster Client ID | GUID of Loadmaster service principal. | yes | *necessary-to-inform* |
| Loadmaster Client Name | Name of Loadmaster service principal. | yes | *necessary-to-inform* |
| Loadmaster Client Secret | Secret of Loadmaster service principal. | yes | *necessary-to-inform* |

### User Groups

It is important to create User groups in Entra ID to manage access and permissions for different types of users interacting with DPManager.
The tool DPManager application needs to know the GUIDs of these user groups to properly manage access and permissions.

| Role | Description | Mandatory | User Group | GUID |
| --- | --- | --- | --- | --- |
| DPM Admins | Users that can change some DPManager settings. | yes | *DPMAdmins* | *guid-necessary-to-inform* |
| DPM Users | Users that can access DPManager and access the basic forms and Manual Data | yes | *DPMUsers* | *guid-necessary-to-inform* |
| DPM ManualData | Users that can modify Manual Data definitions. | yes | *DPMManualData* | *guid-necessary-to-inform* |
| DPM TutorialUsers | Users that can access to the tutorial content in DPManager. Recommended only for Dev environments. | | *DPMTutorialUsers* | *guid-necessary-to-inform* |
| Deployment Admin | Users that can modify the status of deployment scripts. Not necessary for Productive environments. | | *DeploymentAdmin* | *guid-necessary-to-inform* |
| Deployment User | Users that can access deployment scripts and related resources. Not necessary for Productive environments. | | *DeploymentUser* | *guid-necessary-to-inform* |
| Loadmaster Executer | Users that can configure and execute jobs in Loadmaster. | yes | *LoadmasterExecuter* | *guid-necessary-to-inform* |
| Loadmaster Viewer | Users that can see the log (monitoring) of Loadmaster executions. | yes | *LoadmasterViewer* | *guid-necessary-to-inform* |

## Microsoft Fabric



| Parameter | Description | Example |
| --- | --- | --- |

FABRIC_WORKSPACE_ID
FABRIC_ENVIRONMENT_ID

FABRIC_LAKEHOUSE_ID
FABRIC_LAKEHOUSE_NAME
FABRIC_LAKEHOUSE_CONNECTION_ID

FABRIC_DB_CONNECTION_ID
FABRIC_DB_BIMAN_ID
FABRIC_DB_BIMAN_NAME
FABRIC_DB_BIMAN_CSTRING
FABRIC_DB_LOADMASTER_ID
FABRIC_DB_LOADMASTER_NAME
FABRIC_DB_LOADMASTER_CSTRING
FABRIC_DB_DPMU_CSTRING




| Fabric workspace name | Customer-approved workspace name. | `Contoso-DPManager-prod` |
| Fabric workspace ID | Workspace identifier used to locate the deployment target. | `55555555-5555-5555-5555-555555555555` |
| Workspace URL | Link to the Fabric workspace, if available. | `https://app.fabric.microsoft.com/groups/[workspace-id]` |
| Fabric capacity/region | Capacity name or identifier and region hosting the workspace. | `Contoso F64 / East US` |
| Lakehouse name and item ID | Name and identifier of the target lakehouse. | `dpm_lakehouse / [item ID]` |
| `dpmu` SQL database | Database item identifier and approved non-secret connection metadata. | `[item ID] / [server or endpoint]` |
| `bi_man` SQL database | Database item identifier and approved non-secret connection metadata. | `[item ID] / [server or endpoint]` |
| `loadmaster` SQL database | Database item identifier and approved non-secret connection metadata. | `[item ID] / [server or endpoint]` |
| Fabric connection names and IDs | Connection name/identifier for the lakehouse and each SQL database. | `DPManager-prod-lakehouse / [connection ID]` |

## Access and Contacts

| Parameter | Description | Example |
| --- | --- | --- |
| Fabric API setting scope | Whether service-principal API access is enabled and the group/scope to which it applies. | Enabled for `Contoso-DPManager-prod-FabricAPI` |
| Workspace roles granted | Confirmed role(s) for each application or group. | `[Role confirmed with DPSolution]` |
| Entra administrator | Customer contact who can manage app registrations, groups, and consent. | `admin@example.com` |
| Fabric administrator | Customer contact who can manage tenant settings and workspace access. | `fabric-admin@example.com` |
| Technical contact | Customer contact for deployment coordination and testing. | `Jane Doe / jane@example.com` |
| DPSolution contact | DPSolution contact coordinating the deployment. | `[Name / email]` |
| Target deployment date/window | Customer's preferred deployment timing and time zone. | `2026-02-10, 09:00-12:00 Eastern` |

## Readiness Confirmation

| Check | Status | Notes / owner |
| --- | --- | --- |
| Environment name and abbreviation approved | [Status] | [Notes] |
| App registrations and service principals created | [Status] | [Notes] |
| Entra groups created and reviewed | [Status] | [Notes] |
| Fabric workspace and required data assets created | [Status] | [Notes] |
| Four Fabric connections created and tested | [Status] | [Notes] |
| Fabric API access configured for approved scope | [Status] | [Notes] |
| Workspace access configured and validated | [Status] | [Notes] |
| Exact permissions and authentication method confirmed with DPSolution | [Status] | [Notes] |