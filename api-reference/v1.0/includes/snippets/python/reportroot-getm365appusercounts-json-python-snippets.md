---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

query_params = GetM365AppUserCountsWithPeriodRequestBuilder.GetM365AppUserCountsWithPeriodRequestBuilderGetQueryParameters(
		format = "application/json",
)

request_configuration = GetM365AppUserCountsWithPeriodRequestBuilder.GetM365AppUserCountsWithPeriodRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)

await graph_client.reports.get_m365_app_user_counts_with_period("{period}").get(request_configuration = request_configuration)


```