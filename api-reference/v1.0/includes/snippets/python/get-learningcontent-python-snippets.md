---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)


result = await graph_client.employee_experience.learning_providers.by_learning_provider_id('learningProvider-id').learning_contents.by_learning_content_id('learningContent-id').get()


```