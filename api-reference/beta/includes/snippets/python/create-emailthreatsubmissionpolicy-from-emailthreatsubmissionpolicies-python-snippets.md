---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = EmailThreatSubmissionPolicy(
	is_report_to_microsoft_enabled = True,
)

result = await graph_client.security.threat_submission.email_threat_submission_policies.post(request_body)


```