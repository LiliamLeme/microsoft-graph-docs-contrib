---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

query_params = NamedLocationsRequestBuilder.NamedLocationsRequestBuilderGetQueryParameters(
		filter = "createdDateTime ge 2019-09-01T00:00:00Z",
)

request_configuration = NamedLocationsRequestBuilder.NamedLocationsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)

result = await graph_client.identity.conditional_access.named_locations.get(request_configuration = request_configuration)


```