---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = DelegatedAdminRelationshipRequest(
	action = DelegatedAdminRelationshipRequestAction.LockForApproval,
)

result = await graph_client.tenant_relationships.delegated_admin_relationships.by_delegated_admin_relationship_id('delegatedAdminRelationship-id').requests.post(request_body)


```