---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = User(
	custom_security_attributes = CustomSecurityAttributeValue(
		additional_data = {
				"engineering" : {
						"@odata_type" : "#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
						"project_date" : None,
				},
		}
	),
)

result = await graph_client.users.by_user_id('user-id').patch(request_body)


```