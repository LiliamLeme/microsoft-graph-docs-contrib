---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

query_params = DeltaRequestBuilder.DeltaRequestBuilderGetQueryParameters(
		select = ["displayName"],
)

request_configuration = DeltaRequestBuilder.DeltaRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)
request_configuration.headers.add("Prefer", "odata.maxpagesize=2")


result = await graph_client.me.contact_folders.by_contact_folder_id('contactFolder-id').contacts.delta.get(request_configuration = request_configuration)


```