# 02.02 Microsoft Entra ID: Register Data Platform Manager application

![Last Revision](../../assets/lastrevision.svg)

For the DPManager .NET web application, you must register an application in Microsoft Entra ID (formerly Azure Active Directory). This registration establishes trust and allows Entra ID to authenticate and authorize users and applications securely.

![EntraId](../../assets/image_entraid_001.jpg)

## A. Register a new application

- Open `Microsoft Entra ID` and, in the left-hand menu, select `App registrations`, then select `New registration`.  

![EntraId-Register-App](../../assets/image_entraid_002.jpg)

- Complete the registration form:

> Remember the name of the DPManager app has been set here: [Service principal names](../02-Environment-Tasks/02-01-Environemnt-names.md#service-principal-names)

![EntraId-Register-App](../../assets/image_entraid_003.jpg)

> To complete the registration, you would need to know the Redirect URI. This information can be delivered by Data Platform Solutions AG member.  
> It is necessary to have prepared:
> - Name of the customer
> - Instance abbreviation
> 
> The URI should have have this format: `https://{instance_dpmanager_app_domain}/auth`

## B. Configure API permissions

- After the app is registered, configure the Microsoft Graph API permissions required by the application.  
  Go to `API permissions` and select `Microsoft Graph`.

![EntraId-Register-App](../../assets/image_entraid_004.jpg)

- Select the follow permissions, in Microsoft Graph:
  - `openid`
  - `profile`
  - `User.Read`
  - `User.ReadBasic.All`

![EntraId-Register-App](../../assets/image_entraid_005.jpg)

## C. Configure the token

Configure the groups claim that the application receives in the token after user authentication.

- Go to `Token configuration` and select `Add groups claim`.  

![EntraId-Register-App](../../assets/image_entraid_006.jpg)

- In the new window, select `Security groups` under **Group types**, and configure the group claims as follows:
  - **ID:** `Group ID`
  - **Access:** `Group ID`
  - **SAML:** `Group ID`

![EntraId-Register-App](../../assets/image_entraid_007.jpg)

## D. Generate an application secret

Generate a client secret to allow DPManager to identify itself as the registered application.

![EntraId-Register-App](../../assets/image_entraid_008_a.jpg)

> **Important:** The client secret value is only displayed once immediately after creation. If you navigate away, close the page, or exit your browser, you won't be able to retrieve it—you'll need to create a new secret instead. Save the value securely before proceeding.

![EntraId-Register-App](../../assets/image_entraid_009.jpg)

## E. Collect the required information

- **Tenant ID and domain:** You can find these on the Microsoft Entra ID overview page.

![EntraId-Register-App](../../assets/image_entraid_010.jpg)

- **Client ID:** You can find this on the overview page of the application you created in the previous steps.

![EntraId-Register-App](../../assets/image_entraid_011.jpg)

- **Client secret:** This was generated in step D. Remember that the secret value is only visible once.
