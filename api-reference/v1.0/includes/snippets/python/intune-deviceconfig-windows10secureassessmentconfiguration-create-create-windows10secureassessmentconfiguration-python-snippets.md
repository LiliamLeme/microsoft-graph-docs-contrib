---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = Windows10SecureAssessmentConfiguration(
	odata_type = "#microsoft.graph.windows10SecureAssessmentConfiguration",
	description = "Description value",
	display_name = "Display Name value",
	version = 7,
	launch_uri = "Launch Uri value",
	configuration_account = "Configuration Account value",
	allow_printing = True,
	allow_screen_capture = True,
	allow_text_suggestion = True,
)

result = await graph_client.device_management.device_configurations.post(request_body)


```