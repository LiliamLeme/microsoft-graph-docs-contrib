---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

query_params = IdentityUserFlowAttributeAssignmentItemRequestBuilder.IdentityUserFlowAttributeAssignmentItemRequestBuilderGetQueryParameters(
		expand = ["userAttribute"],
)

request_configuration = IdentityUserFlowAttributeAssignmentItemRequestBuilder.IdentityUserFlowAttributeAssignmentItemRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)

result = await graph_client.identity.b2c_user_flows.by_b2c_identity_user_flow_id('b2cIdentityUserFlow-id').user_attribute_assignments.by_identity_user_flow_attribute_assignment_id('identityUserFlowAttributeAssignment-id').get(request_configuration = request_configuration)


```