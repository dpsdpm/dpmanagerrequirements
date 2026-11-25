# 02.01 Definition of Environment names

![Last Revision](../../assets/lastrevision.svg)

This document helps you define all the names for this environment.

## Environment names

|                          | Responsible | Example     | Value |
| ------------------------ | ----------- | ----------- | ----- |
| Environment Name         | Customer    | Development |       |
| Environment abbreviation | Customer    | dev         |       |

The `Environment abbreviation` will be used throughout this documentation and is represented as **{env}**.

## Fabric object names

|                               | Responsible | Example                  | Value |
| ----------------------------- | ----------- | ------------------------ | ----- |
| Fabric workspace name         | Customer    | spot-**{env}**           |       |
| Fabric lakehouse name         | Customer    | lhouse-**{env}**         |       |
| Fabric environment            | Customer    | loadmaster-**{env}**-env |       |
| Fabric SQL db loadmaster name | Customer    | loadmaster-**{env}**     |       |
| Fabric SQL db bi_man name     | Customer    | biman-**{env}**          |       |
| Fabric SQL db dpmu name       | Customer    | dpmu-**{env}**           |       |

## Entra ID object names

### Service principal names

|                             | Responsible | Example                  | Value |
| --------------------------- | ----------- | ------------------------ | ----- |
| EntraID DPManager app name  | Customer IT | app-dpmanager-**{env}**  |       |
| EntraID Loadmaster app name | Customer IT | app-loadmaster-**{env}** |       |

To register the `DPManager app`, follow the steps in [Register DPManager app](02-02-EntraID-howto-dpmanager-app.md)

To register the `Loadmaster app`, follow the steps in [Register Loadmaster app](02-03-EntraID-howto-loadmaster-app.md)

### DPManager and Roles and EntraId Security Groups

You must create Entra ID Security Groups to associate different roles that help DPManager grant access to specific users. The following are the DPManager roles and their descriptions:

- **DPMAdmins**: Users who can modify the main configuration of DPManager and force grid check-ins.
- **DPMMDataAdmin**: Users who can manage Manual Data definitions and columns.
- **DPMUsers**: Users who can access basic forms in DPManager.
- **DPMTutorialUsers**: Users who can access tutorial forms in DPManager.
- **DeploymentUser**: Users who can modify objects scheduled for the next deployment.
- **DeploymentAdmin**: Users who can control and configure the deployment process.
- **AzLoadMasterViewer**: Users who can view job execution logs.
- **AzLoadMasterExecuter**: Users who can modify Loadmaster configuration and execute jobs.

The following table helps you define the names for these security groups:

| DPManager Role       | Responsible | Example                        | EntraID group name |
| -------------------- | ----------- | ------------------------------ | ------------------ |
| DPMAdmins            | Customer IT | DPMAdmins-**{env}**            |                    |
| DPMMDataAdmin        | Customer IT | DPMMDataAdmin-**{env}**        |                    |
| DPMUsers             | Customer IT | DPMUsers-**{env}**             |                    |
| DPMTutorialUsers     | Customer IT | DPMTutorialUsers-**{env}**     |                    |
| DeploymentUser       | Customer IT | DeploymentUser-**{env}**       |                    |
| DeploymentAdmin      | Customer IT | DeploymentAdmin-**{env}**      |                    |
| AzLoadMasterViewer   | Customer IT | AzLoadMasterViewer-**{env}**   |                    |
| AzLoadMasterExecuter | Customer IT | AzLoadMasterExecuter-**{env}** |                    |

To create all these Security Groups, follow the steps in [Create Security Groups](02-04-EntraID-howto-create-security-group.md)





