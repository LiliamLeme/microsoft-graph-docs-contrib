---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

query_params = GroupsRequestBuilder.GroupsRequestBuilderGetQueryParameters(
		search = "\"displayName:Video\" OR \"description:prod\"",
		orderby = ["displayName"],
		count = True,
)

request_configuration = GroupsRequestBuilder.GroupsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)
request_configuration.headers.add("ConsistencyLevel", "eventual")


result = await graph_client.groups.get(request_configuration = request_configuration)


```