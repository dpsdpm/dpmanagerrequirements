# Information for DPSolution

![Last Revision](../assets/lastrevision.svg)

Complete this handoff with customer-approved, non-secret information. Share it through the secure channel agreed with DPSolution. Do not include passwords, client secrets, certificates, tokens, private keys, or other credentials.

You can download this [Excel](../assets/OnboardingWorkbook.20261101.xlsx) to collect all this information

## Customer and Environment

| Parameter                 | Description              | Source                                                                              | Value |
| ------------------------- | ------------------------ | --------------------------------------------------------------------------------------- | ----- |
| DPM_CUSTOMER_NAME         | Customer name            | [General names](./01-Initial-Tasks/01-01-Tenant-naming-rule.md#general-names)           |       |
| DPM_CUSTOMER_ABBREVIATION | Customer abbreviation    | [General names](./01-Initial-Tasks/01-01-Tenant-naming-rule.md#general-names)           |       |
| DPM_AZURE_LOCATION        | Azure region             | [General names](./01-Initial-Tasks/01-01-Tenant-naming-rule.md#general-names)           |       |
| DPM_CUSTOMER_DOMAIN       | Main domain              | Home page of EntraID                                                                    |       |
| DPM_CUSTOMER_TENANT_ID    | Tenant ID                | [General names](./01-Initial-Tasks/01-01-Tenant-naming-rule.md#general-names)           |       |
| DPM_INSTANCE_NAME         | Environment name         | [Environment names](./02-Environment-Tasks/02-01-Environemnt-names.md#enviroment-names) |       |
| DPM_INSTANCE_ABREVIATION  | Environment abbreviation | [Environment names](./02-Environment-Tasks/02-01-Environemnt-names.md#enviroment-names) |       |
| DPM_INSTANCE_CODE         | Instance Code            | Data Platform Solutions team                                  |       |

## Microsoft Entra ID

### Service Principals

| Parameter               | Description                  | Source                                                                                                                    | Value |
| ----------------------- | ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------- | ----- |
| DPMANAGER_CLIENT_NAME   | DPManager app name           | [DPManager app name](./02-Environment-Tasks/02-01-Environemnt-names.md#service-principal-names)                               |       |
| DPMANAGER_CLIENT_ID     | DPManager app client_id      | [DPManager app client id](./02-Environment-Tasks/02-02-EntraID-howto-dpmanager-app.md#e-collect-the-required-information)     |       |
| DPMANAGER_CLIENT_SECRET | DPManager app client secret  | [DPManager app cliente secret](./02-Environment-Tasks/02-02-EntraID-howto-dpmanager-app.md#d-generate-an-application-secret)  |       |
| LOADMASTER_CLIENT_ID    | Loadmaster app name          | [Loadmaster app name](./02-Environment-Tasks/02-01-Environemnt-names.md#service-principal-names)                              |       |
| LOADMASTER_CLIENT_ID    | Loadmaster app client_id     | [Loadmaster app client id](./02-Environment-Tasks/02-03-EntraID-howto-loadmaster-app.md#e-collect-the-required-information)   |       |
| LOADMASTER_CLIENT_ID    | Loadmaster app client secret | [Loadmaster app client secret](./02-Environment-Tasks/02-03-EntraID-howto-loadmaster-app.md#b-generate-an-application-secret) |       |

### Security Groups

It is important to inform the information of the service principals that should be already registered in Entra ID.

| Parameter            | Source                                                                                                                    | Value |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------- | ----- |
| DPMAdmins            | [Security Group names](./02-Environment-Tasks/02-01-Environemnt-names.md#dpmanager-and-roles-and-entraid-security-groups) |       |
| DPMMDataAdmin        | [Security Group names](./02-Environment-Tasks/02-01-Environemnt-names.md#dpmanager-and-roles-and-entraid-security-groups) |       |
| DPMUsers             | [Security Group names](./02-Environment-Tasks/02-01-Environemnt-names.md#dpmanager-and-roles-and-entraid-security-groups) |       |
| DPMTutorialUsers     | [Security Group names](./02-Environment-Tasks/02-01-Environemnt-names.md#dpmanager-and-roles-and-entraid-security-groups) |       |
| DeploymentUser       | [Security Group names](./02-Environment-Tasks/02-01-Environemnt-names.md#dpmanager-and-roles-and-entraid-security-groups) |       |
| DeploymentAdmin      | [Security Group names](./02-Environment-Tasks/02-01-Environemnt-names.md#dpmanager-and-roles-and-entraid-security-groups) |       |
| AzLoadMasterViewer   | [Security Group names](./02-Environment-Tasks/02-01-Environemnt-names.md#dpmanager-and-roles-and-entraid-security-groups) |       |
| AzLoadMasterExecuter | [Security Group names](./02-Environment-Tasks/02-01-Environemnt-names.md#dpmanager-and-roles-and-entraid-security-groups) |       |

## Microsoft Fabric

| Parameter                      | Source                                                                                                              | Value |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------- | ----- |
| FABRIC_WORKSPACE_ID            | [Workspace](./02-Environment-Tasks/02-05-Fabric-preparation.md#1-create-workspace)                                  |       |
| FABRIC_ENVIRONMENT_ID          | [Environment](./02-Environment-Tasks/02-05-Fabric-preparation.md#2-create-environment)                              |       |
| FABRIC_LAKEHOUSE_NAME          | [Fabric object names](./02-Environment-Tasks/02-01-Environemnt-names.md#fabric-object-names)                        |       |
| FABRIC_LAKEHOUSE_ID            | [Lakehouse](./02-Environment-Tasks/02-05-Fabric-preparation.md#3-create-lakehouse)                                  |       |
| FABRIC_LAKEHOUSE_CONNECTION_ID | [Lakehouse connection ID](./01-Initial-Tasks/01-02-tasks-shared.md#2b-create-connection-to-fabric-lakehouse)        |       |
| FABRIC_DB_CONNECTION_ID        | [SQL Database connection ID](./01-Initial-Tasks/01-02-tasks-shared.md#2a-create-connection-to-fabric-sql-databases) |       |
| FABRIC_DB_BIMAN_NAME           | [Fabric object names](./02-Environment-Tasks/02-01-Environemnt-names.md#fabric-object-names)                        |       |
| FABRIC_DB_BIMAN_ID             | [Creation SQL database](./02-Environment-Tasks/02-05-Fabric-preparation.md#4-create-databases)                      |       |
| FABRIC_DB_BIMAN_CSTRING        | [Get SQL connection string](./02-Environment-Tasks/02-05-Fabric-preparation.md#4c-get-connection-string)            |       |
| FABRIC_DB_LOADMASTER_NAME      | [Fabric object names](./02-Environment-Tasks/02-01-Environemnt-names.md#fabric-object-names)                        |       |
| FABRIC_DB_LOADMASTER_ID        | [Creation SQL database](./02-Environment-Tasks/02-05-Fabric-preparation.md#4-create-databases)                      |       |
| FABRIC_DB_LOADMASTER_CSTRING   | [Get SQL connection string](./02-Environment-Tasks/02-05-Fabric-preparation.md#4c-get-connection-string)            |       |
| FABRIC_DB_DPMU_CSTRING         | [Get SQL connection string](./02-Environment-Tasks/02-05-Fabric-preparation.md#4c-get-connection-string)            |       |
