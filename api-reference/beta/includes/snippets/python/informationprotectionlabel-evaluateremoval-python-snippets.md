---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = EvaluateRemovalPostRequestBody(
	content_info = ContentInfo(
		odata_type = "#microsoft.graph.contentInfo",
		format = ContentFormat.Default,
		identifier = None,
		state = ContentState.Rest,
		metadata = [
			KeyValuePair(
				odata_type = "#microsoft.graph.keyValuePair",
				name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
				value = "True",
			),
			KeyValuePair(
				odata_type = "#microsoft.graph.keyValuePair",
				name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
				value = "Standard",
			),
			KeyValuePair(
				odata_type = "#microsoft.graph.keyValuePair",
				name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
				value = "1/1/0001 12:00:00 AM",
			),
			KeyValuePair(
				odata_type = "#microsoft.graph.keyValuePair",
				name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
				value = "cfa4cf1d-a337-4481-aa99-19d8f3d63f7c",
			),
			KeyValuePair(
				odata_type = "#microsoft.graph.keyValuePair",
				name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
				value = "General",
			),
			KeyValuePair(
				odata_type = "#microsoft.graph.keyValuePair",
				name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
				value = "0",
			),
			KeyValuePair(
				odata_type = "#microsoft.graph.keyValuePair",
				name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId",
				value = "00000000-0000-0000-0000-000000000000",
			),
		],
		additional_data = {
				"format@odata_type" : "#microsoft.graph.contentFormat",
				"state@odata_type" : "#microsoft.graph.contentState",
				"metadata@odata_type" : "#Collection(microsoft.graph.keyValuePair)",
		}
	),
	downgrade_justification = DowngradeJustification(
		justification_message = "The information has been declassified.",
		is_downgrade_justified = True,
	),
)

request_configuration = EvaluateRemovalRequestBuilder.EvaluateRemovalRequestBuilderPostRequestConfiguration()
request_configuration.headers.add("User-Agent", "ContosoLOBApp/1.0")


result = await graph_client.information_protection.policy.labels.evaluate_removal.post(request_body, request_configuration = request_configuration)


```