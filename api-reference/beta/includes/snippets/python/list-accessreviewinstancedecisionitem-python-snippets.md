---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

query_params = DecisionsRequestBuilder.DecisionsRequestBuilderGetQueryParameters(
		top = 100,
		skip = 0,
)

request_configuration = DecisionsRequestBuilder.DecisionsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)

result = await graph_client.identity_governance.access_reviews.definitions.by_access_review_schedule_definition_id('accessReviewScheduleDefinition-id').instances.by_access_review_instance_id('accessReviewInstance-id').decisions.get(request_configuration = request_configuration)


```