---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = InferenceClassificationOverride(
	classify_as = InferenceClassificationType.Focused,
	sender_email_address = EmailAddress(
		name = "Samantha Booth",
		address = "samanthab@adatum.onmicrosoft.com",
	),
)

result = await graph_client.me.inference_classification.overrides.post(request_body)


```