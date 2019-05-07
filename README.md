# ![LOGO](logo.png) AuthorizationManagementClient **flow**ground Connector

## Description

A generated **flow**ground connector for the AuthorizationManagementClient API (version 2018-07-01-preview).

Generated from: https://api.apis.guru/v2/specs/azure.com/authorization-authorization-DenyAssignmentGetCalls/2018-07-01-preview/swagger.json<br/>
Generated at: 2019-05-07T17:37:16+03:00

## API Description

Role based access control provides you a way to apply granular level policy administration down to individual resources or resource groups. These operations enable you to get deny assignments. A deny assignment describes the set of actions on resources that are denied for Azure Active Directory users.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Gets all deny assignments for the subscription.

*Tags:* `DenyAssignments`

#### Input Parameters
* `subscriptionId` - _required_ - The ID of the target subscription.
* `api-version` - _required_ - The API version to use for this operation.
* `$filter` - _optional_ - The filter to apply on the operation. Use $filter=atScope() to return all deny assignments at or above the scope. Use $filter=denyAssignmentName eq '{name}' to search deny assignments by name at specified scope. Use $filter=principalId eq '{id}' to return all deny assignments at, above and below the scope for the specified principal. Use $filter=gdprExportPrincipalId eq '{id}' to return all deny assignments at, above and below the scope for the specified principal. This filter is different from the principalId filter as it returns not only those deny assignments that contain the specified principal is the Principals list but also those deny assignments that contain the specified principal is the ExcludePrincipals list. Additionally, when gdprExportPrincipalId filter is used, only the deny assignment name and description properties are returned.

### Gets deny assignments for a resource group.

*Tags:* `DenyAssignments`

#### Input Parameters
* `subscriptionId` - _required_ - The ID of the target subscription.
* `resourceGroupName` - _required_ - The name of the resource group.
* `api-version` - _required_ - The API version to use for this operation.
* `$filter` - _optional_ - The filter to apply on the operation. Use $filter=atScope() to return all deny assignments at or above the scope. Use $filter=denyAssignmentName eq '{name}' to search deny assignments by name at specified scope. Use $filter=principalId eq '{id}' to return all deny assignments at, above and below the scope for the specified principal. Use $filter=gdprExportPrincipalId eq '{id}' to return all deny assignments at, above and below the scope for the specified principal. This filter is different from the principalId filter as it returns not only those deny assignments that contain the specified principal is the Principals list but also those deny assignments that contain the specified principal is the ExcludePrincipals list. Additionally, when gdprExportPrincipalId filter is used, only the deny assignment name and description properties are returned.

### Gets deny assignments for a resource.

*Tags:* `DenyAssignments`

#### Input Parameters
* `subscriptionId` - _required_ - The ID of the target subscription.
* `resourceGroupName` - _required_ - The name of the resource group.
* `resourceProviderNamespace` - _required_ - The namespace of the resource provider.
* `parentResourcePath` - _required_ - The parent resource identity.
* `resourceType` - _required_ - The resource type of the resource.
* `resourceName` - _required_ - The name of the resource to get deny assignments for.
* `api-version` - _required_ - The API version to use for this operation.
* `$filter` - _optional_ - The filter to apply on the operation. Use $filter=atScope() to return all deny assignments at or above the scope. Use $filter=denyAssignmentName eq '{name}' to search deny assignments by name at specified scope. Use $filter=principalId eq '{id}' to return all deny assignments at, above and below the scope for the specified principal. Use $filter=gdprExportPrincipalId eq '{id}' to return all deny assignments at, above and below the scope for the specified principal. This filter is different from the principalId filter as it returns not only those deny assignments that contain the specified principal is the Principals list but also those deny assignments that contain the specified principal is the ExcludePrincipals list. Additionally, when gdprExportPrincipalId filter is used, only the deny assignment name and description properties are returned.

### Gets a deny assignment by ID.

*Tags:* `DenyAssignments`

#### Input Parameters
* `denyAssignmentId` - _required_ - The fully qualified deny assignment ID. For example, use the format, /subscriptions/{guid}/providers/Microsoft.Authorization/denyAssignments/{denyAssignmentId} for subscription level deny assignments, or /providers/Microsoft.Authorization/denyAssignments/{denyAssignmentId} for tenant level deny assignments.
* `api-version` - _required_ - The API version to use for this operation.

### Gets deny assignments for a scope.

*Tags:* `DenyAssignments`

#### Input Parameters
* `scope` - _required_ - The scope of the deny assignments.
* `api-version` - _required_ - The API version to use for this operation.
* `$filter` - _optional_ - The filter to apply on the operation. Use $filter=atScope() to return all deny assignments at or above the scope. Use $filter=denyAssignmentName eq '{name}' to search deny assignments by name at specified scope. Use $filter=principalId eq '{id}' to return all deny assignments at, above and below the scope for the specified principal. Use $filter=gdprExportPrincipalId eq '{id}' to return all deny assignments at, above and below the scope for the specified principal. This filter is different from the principalId filter as it returns not only those deny assignments that contain the specified principal is the Principals list but also those deny assignments that contain the specified principal is the ExcludePrincipals list. Additionally, when gdprExportPrincipalId filter is used, only the deny assignment name and description properties are returned.

### Get the specified deny assignment.

*Tags:* `DenyAssignments`

#### Input Parameters
* `scope` - _required_ - The scope of the deny assignment.
* `denyAssignmentId` - _required_ - The ID of the deny assignment to get.
* `api-version` - _required_ - The API version to use for this operation.

## License

**flow**ground :- Telekom iPaaS / azure-com-authorization-authorization-deny-assignment-get-calls-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
