---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = Organization(
	marketing_notification_emails = [
		"marketing@contoso.com",
	],
	privacy_profile = PrivacyProfile(
		contact_email = "alice@contoso.com",
		statement_url = "https://contoso.com/privacyStatement",
	),
	security_compliance_notification_mails = [
		"security@contoso.com",
	],
	security_compliance_notification_phones = [
		"(123) 456-7890",
	],
	technical_notification_mails = [
		"tech@contoso.com",
	],
)

result = await graph_client.organization.by_organization_id('organization-id').patch(request_body)


```