# 02.01 Definition of Environment names

![Last Revision](../../assets/lastrevision.svg)

This formular will help you to define all the name for this environment

## Enviroment names

|                          | Resposable | Exampl      | Value |
| ------------------------ | ---------- | ----------- | ----- |
| Environment Name         | Customer   | Development |       |
| Environment abbreviation | Customer   | dev         |       |

The `Environment abbreviation` will be used in other parts of this documentation. It will be showed as **{env}**

## Fabric object names

|                               | Resposable | Exampl                   | Value |
| ----------------------------- | ---------- | ------------------------ | ----- |
| Fabric workspace name         | Customer   | spot-**{env}**           |       |
| Fabric lakehouse name         | Customer   | lhouse-**{env}**         |       |
| Fabric environment            | Customer   | loadmaster-**{env}**-env |       |
| Fabric SQL db loadmaster name | Customer   | loadmaster-**{env}**     |       |
| Fabric SQL db bi_man name     | Customer   | biman-**{env}**          |       |
| Fabric SQL db dpmu name       | Customer   | dpmu-**{env}**           |       |

## Entra ID object names

### Service principal names

|                             | Resposable  | Exampl                   | Value |
| --------------------------- | ----------- | ------------------------ | ----- |
| EntraID DPManager app name  | Customer IT | app-dpmanager-**{env}**  |       |
| EntraID Loadmaster app name | Customer IT | app-loadmaster-**{env}** |       |

To register the `DPManager app`, follow the steps in [Register DPManager app](02-02-EntraID-howto-dpmanager-app.md)

To register the `Loadmaster app`, follow the steps in [Register Loadmaster app](02-03-EntraID-howto-loadmaster-app.md)

### DPManager and Roles and EntraId Security Groups

It is necessary to create some EntraID Security Groups to associate the different roles that help DPManager to grant the access to specific users.  
This is the list of DPManager roles and their description:

- **DPMAdmin**: List of users that can modify the main configuration of DPManager. Also they can force the check-in of grid.
- **DPMMDataAdmin**: List of users that can manage Manual Data definitions and the columns.
- **DPMUsers**:  List of users that can access to the basic forms in DPManager.
- **DPMTutorialUsers**:  List of users that can access to the tutorial forms in DPManager.
- **DeploymentUser**:  List of users that can modify the objects to deploy in the next release.
- **DeploymentAdmin**:  List of users that can block and config the deployment procoess.
- **AzLoadMasterViewer**: List of users that can see the Execution of jobs.
- **AzLoadMasterExecuter**: List of users that can modify Loadmaster configuration and execute jobs.

This table will help you to define the name of differen

| DPManager Role       | Resposable  | Example                        | EntraID group name |
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





