---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

query_params = TabsRequestBuilder.TabsRequestBuilderGetQueryParameters(
		expand = ["teamsApp"],
)

request_configuration = TabsRequestBuilder.TabsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)

result = await graph_client.teams.by_team_id('team-id').channels.by_channel_id('channel-id').tabs.get(request_configuration = request_configuration)


```