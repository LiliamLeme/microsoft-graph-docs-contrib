---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = DismissPostRequestBody(
	user_ids = [
		"04487ee0-f4f6-4e7f-8999-facc5a30e232",
		"13387ee0-f4f6-4e7f-8999-facc5120e345",
	],
)

await graph_client.risky_users.dismiss.post(request_body)


```