---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = RoleDefinition(
	odata_type = "#microsoft.graph.roleDefinition",
	display_name = "Display Name value",
	description = "Description value",
	role_permissions = [
		RolePermission(
			odata_type = "microsoft.graph.rolePermission",
			resource_actions = [
				ResourceAction(
					odata_type = "microsoft.graph.resourceAction",
					allowed_resource_actions = [
						"Allowed Resource Actions value",
					],
					not_allowed_resource_actions = [
						"Not Allowed Resource Actions value",
					],
				),
			],
		),
	],
	is_built_in = True,
)

result = await graph_client.device_management.role_definitions.post(request_body)


```