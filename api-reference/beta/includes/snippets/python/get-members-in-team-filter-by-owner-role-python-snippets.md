---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

query_params = MembersRequestBuilder.MembersRequestBuilderGetQueryParameters(
		filter = "roles/any(r:r eq 'owner')",
)

request_configuration = MembersRequestBuilder.MembersRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)

result = await graph_client.teams.by_team_id('team-id').members.get(request_configuration = request_configuration)


```