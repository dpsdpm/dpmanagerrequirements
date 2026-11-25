# 01.01 Customer naming convention

![Last Revision](../../assets/lastrevision.svg)

This document guides you through defining all the necessary names for the different services, objects, and policies required to integrate DPManager with a customer's tenant.

## General names

The following are the first data points that must be defined together with the customer.

|                       | Responsable | Example only  | Value |
| --------------------- | ----------- | ------------- | ----- |
| Customer name         | Customer    | *Contoso*     |       |
| Customer abbreviation | Customer    | *cts*         |       |
| Region                | IT Customer | *eastus*      |       |
| Tenant ID             | IT Customer | *guid*        |       |
| Main domain           | IT Customer | *contoso.com* |       |

## Security Group

You must also define an Entra ID Security Group to include all Service Principals that require rights to create or modify objects in Microsoft Fabric Workspaces. These groups also enable triggering of objects such as Notebooks, Pipelines, and Dataflows.

|                           | Resposable  | Example                     | Value |
| ------------------------- | ----------- | --------------------------- | ----- |
| LoadmasterFabricExecutors | Customer IT | *LoadmasterFabricExecutors* |       |


