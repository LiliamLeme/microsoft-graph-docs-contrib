---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = AuthenticationContextClassReference(
	display_name = "Contoso medium",
	description = "Medium protection level defined for Contoso policy",
	is_available = True,
)

result = await graph_client.identity.conditional_access.authentication_context_class_references.by_authentication_context_class_reference_id('authenticationContextClassReference-id').patch(request_body)


```