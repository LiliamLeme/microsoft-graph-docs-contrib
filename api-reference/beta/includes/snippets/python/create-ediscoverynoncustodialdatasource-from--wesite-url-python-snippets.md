---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = EdiscoveryNoncustodialDataSource(
	data_source = SiteSource(
		odata_type = "microsoft.graph.security.siteSource",
		site = Site(
			web_url = "https://m365x809305.sharepoint.com/sites/Design-topsecret",
		),
	),
)

result = await graph_client.security.cases.ediscovery_cases.by_ediscovery_case_id('ediscoveryCase-id').noncustodial_data_sources.post(request_body)


```