# Customer naming convetion



## Naming Decision

This is the first data that needs to be defined together with the customer.

| Field                 | Responsable   | Customer value        | Example only  |
| ---                   | ---           | ---                   | ---           |
| Customer name         | Customer      |                       | *Contoso*     |
| Customer abbreviation | Customer      |                       | *Production*  |
| Region                | IT Customer   |                       | *eastus*      |

Complete this page first. The customer chooses and approves the environment name and abbreviation used for the DPManager deployment.

## Rules for environemnt objects

Define the rules that will define the name of the different objects/resources in the different environments

**{env}** : abbreviation of the enviroment: `dev`, `qual`, `test`, `prod`, etc.  
**{role}** : name of user role to define the different accesses level on DPManager  

| Resource type                 | Responsable                | Rule            | Example using the approved environment    |
| ---                           | ---                        | ---             | ---                                       |
| Entra ID app DPManager        | IT Customer                |                 | DPManager-**{env}**                       |
| Entra ID app Loadmaster       | IT Customer                |                 | Loadmaster-**{env}**                      |
| Entra ID security groups      | IT Customer                |                 | DPM-**{env}**-{role}                      |
| Fabric workspace              | Consultant and IT Customer |                 | {Lakehouse/BI}-**{env}**                  |
| Fabric lakehouse              | Consultant and IT Customer |                 | lakehouse-**{env}**                       |
| Fabric SQL db loadmaster      | Consultant and IT Customer |                 | loadmaster-**{env}**                      |
| Fabric SQL db bi_man          | Consultant and IT Customer |                 | bi_man-**{env}**                          |
| Fabric SQL db dpmu            | Consultant and IT Customer |                 | dpmu-**{env}**                            |

## Confirmation

- [ ] Environment name and abbreviation are approved by the customer.
- [ ] Naming convention is compatible with customer policies and naming limits.
- [ ] The approved values will be used consistently in the remaining setup and handoff pages.

> Examples are illustrative only. Confirm all final names with the customer's platform and security teams.