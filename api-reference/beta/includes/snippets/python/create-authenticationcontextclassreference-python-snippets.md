---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = AuthenticationContextClassReference(
	id = "c1",
	display_name = "Contoso medium",
	description = "Medium protection level defined for Contoso policy",
	is_available = True,
)

result = await graph_client.identity.conditional_access.authentication_context_class_references.post(request_body)


```