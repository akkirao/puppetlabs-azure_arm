Document: "logicAppsManagementClient"


Path: "https://github.com/Azure/azure-rest-api-specs/blob/c9269dbd9a589cd49775b3f65b87c556c2f52cce/specification/web/resource-manager/Microsoft.Web/stable/2016-06-01/logicAppsManagementClient.json")

## ConnectionGatewayDefinition

The gateway definition

```puppet
azure_connection_gateway_definition {
  api_version => "api_version",
  connection_gateway => "connectionGateway",
  connection_gateway_name => "connection_gateway_name",
  etag => "etag (optional)",
  location => "location (optional)",
  properties => "properties (optional)",
  resource_group_name => "resource_group_name",
  subscription_id => "subscription_id",
  tags => "tags (optional)",
}
```

| Name        | Type           | Required       | Description       |
| ------------- | ------------- | ------------- | ------------- |
|api_version | String | true | API Version |
|connection_gateway | Hash | true | The connection gateway |
|connection_gateway_name | String | true | The connection gateway name |
|etag | String | false | Resource ETag |
|location | String | false | Resource location |
|properties | String | false |  |
|resource_group_name | String | true | The resource group |
|subscription_id | String | true | Subscription Id |
|tags | String | false |  |



## CRUD operations

Here is a list of endpoints that we use to create, read, update and delete the ConnectionGatewayDefinition

| Operation | Path | Verb | Description | OperationID |
| ------------- | ------------- | ------------- | ------------- | ------------- |
|Create|`/subscriptions/%{subscription_id}/resourceGroups/%{resource_group_name}/providers/Microsoft.Web/connectionGateways/%{connection_gateway_name}`|Put|Creates or updates a specific gateway for under a subscription and in a specific resource group|ConnectionGateways_CreateOrUpdate|
|List - list all|`/subscriptions/%{subscription_id}/providers/Microsoft.Web/connectionGateways`|Get|Gets a list of gateways under a subscription|ConnectionGateways_List|
|List - get one|`/subscriptions/%{subscription_id}/resourceGroups/%{resource_group_name}/providers/Microsoft.Web/connectionGateways/%{connection_gateway_name}`|Get|Gets a specific gateway under a subscription and in a specific resource group|ConnectionGateways_Get|
|List - get list using params|`/subscriptions/%{subscription_id}/providers/Microsoft.Web/connectionGateways`|Get|Gets a list of gateways under a subscription|ConnectionGateways_List|
|Update|`/subscriptions/%{subscription_id}/resourceGroups/%{resource_group_name}/providers/Microsoft.Web/connectionGateways/%{connection_gateway_name}`|Put|Creates or updates a specific gateway for under a subscription and in a specific resource group|ConnectionGateways_CreateOrUpdate|
|Delete|`/subscriptions/%{subscription_id}/resourceGroups/%{resource_group_name}/providers/Microsoft.Web/connectionGateways/%{connection_gateway_name}`|Delete|Deletes a specific gateway for under a subscription and in a specific resource group|ConnectionGateways_Delete|
