---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = AdministrativeUnit(
	display_name = "Greater Seattle District Technical Schools",
)

result = await graph_client.directory.administrative_units.by_administrative_unit_id('administrativeUnit-id').patch(request_body)


```