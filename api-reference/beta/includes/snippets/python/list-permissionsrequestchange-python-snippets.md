---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

query_params = PermissionsRequestChangesRequestBuilder.PermissionsRequestChangesRequestBuilderGetQueryParameters(
		filter = "modificationDateTime gt {t}",
)

request_configuration = PermissionsRequestChangesRequestBuilder.PermissionsRequestChangesRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)

result = await graph_client.identity_governance.permissions_management.permissions_request_changes.get(request_configuration = request_configuration)


```