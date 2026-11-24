# 01.01 Customer naming convetion

![Last Revision](../../assets/lastrevision.svg)

This document will try to guide you to define all the necessary names for the different services, objects and policies to integrate DPManager with a customer's tenant.

## General names
This is the first data that needs to be defined together with the customer.

|                       | Responsable | Example only  | Value |
| --------------------- | ----------- | ------------- | ----- |
| Customer name         | Customer    | *Contoso*     |       |
| Customer abbreviation | Customer    | *cts*         |       |
| Region                | IT Customer | *eastus*      |       |
| Tenant ID             | IT Customer | *guid*        |       |
| Main domain           | IT Customer | *contoso.com* |       |

## Security Group 

Also, it would be necessary to define a EntraId Security Group to include all the Service Principal that should have the rights to Create/Modify objects in Microsoft Fabric Workspaces. Also they could trigger objects like Notebook, Pipeline and Dataflows

|                           | Resposable  | Example                     | Value |
| ------------------------- | ----------- | --------------------------- | ----- |
| LoadmasterFabricExecutors | Customer IT | *LoadmasterFabricExecutors* |       |


