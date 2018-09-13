# Postman collection for Dynamics 365 WebAPI &nbsp;&nbsp;&nbsp; [![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/f50604e8e8c2e5d107fa#?env%5BDynamics%20365%20Environment%20(Online)%5D=W3siZW5hYmxlZCI6dHJ1ZSwidmFsdWUiOiIiLCJrZXkiOiJBcHBsaWNhdGlvbklkIn0seyJlbmFibGVkIjp0cnVlLCJrZXkiOiJSZWRpcmVjdFVybCIsInZhbHVlIjoiIiwiZGVzY3JpcHRpb24iOiIifSx7ImVuYWJsZWQiOnRydWUsInZhbHVlIjoiIiwia2V5IjoiUmVzb3VyY2UifSx7ImVuYWJsZWQiOnRydWUsInZhbHVlIjoie3tSZXNvdXJjZX19L2FwaS9kYXRhL3Y5LjAvIiwia2V5IjoiV2ViQVBJVXJsIn1d)

___Collection Last Updated: 13/09/2018___

This is a [Postman](https://getpostman.com) collection that covers standard API requests for Dynamics 365. The collection aims to help Dynamics 365 Developers/Power Users to create, run and test different types of Web API request by providing authentication and request templates.

## Using this Collection

### Prerequisites
1. [Download Postman](https://www.getpostman.com)
2. Dynamics 365 Organization
3. [Register Azure AD Application](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/walkthrough-register-dynamics-365-app-azure-active-directory)

### Usage

To use this collection, follow the steps below:

1. Click the 'Run in Postman' button at the top of this page to import the collection into Postman
2. Update the [appropriate environment variables](#vars) to the 'Dynamics 365 Environment (Online)' environment
3. Authenticate collection
4. Run the API requests

### Updates to collection

**Unfortunately, Postman collections are not automatically sync when they are updated.** If you found this collection useful, you should come back periodically to download the latest version and re-import it as described above. 

## <a id="vars"></a>Environment Variables

This collection makes use of [Postman environment variables](https://www.getpostman.com/docs/postman/environments_and_globals/manage_environments) to automate API requests to the greatest extent possible. These variables can be identified in URL's or request headers/body by the use of double curly brackets, for instance: `{{ApplicationId}}`

When the collection is loaded into Postman, it will also load a set of variables you'll need to update before using the request templates.

### Required Environment Variables

| **Variable** | **Description** |
| ----------- | --------------- |
| `ApplicationId` | Azure Application ID used to authenticate the user|
| `RedirectUrl` | Redirct URL configured in the Azure AD Application|
| `Resource` | Dynamics 365 Organization that has been configured in the AAD Application Delegated Permissions section. For intance, `https://yourorg.crm4.dynamics.com`|


### Other Environment Variables

| **Variable** | **Description** |
| ----------- | --------------- |
| `WebAPIUrl` | This variable holds the Web API Url (defaulted to "v9.0" but can be updated to use a different version)|
| `GlobalWebApiUrl` | This **GLOBAL** variable holds the Web API Url and it's only used for batch operations (RAW body doesn't support environment variables). It gets populated with a pre-request script based on the Environment being used so it's environment safe|

## Useful Resources

The following are some useful links to get you started or learn more about Postman or Dynamics 365 Web API.

#### Dynamics 365

- [Using Dynamics 365 Web API](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/use-microsoft-dynamics-365-web-api)

- [Authenticate to Dynamics 365 Web API](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/webapi/authenticate-web-api)

- [Web API Types and Operations](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/webapi/web-api-types-operations)

- [Web API samples](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/webapi/web-api-samples)

#### Postman

- [Download Postman](https://www.getpostman.com/postman)

- [Postman Collection](https://www.getpostman.com/docs/postman/collections/managing_collections)

- [Postman Environment](https://www.getpostman.com/docs/postman/environments_and_globals/manage_environments)
