---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = PrinterShare(
	display_name = "PrinterShare Name",
	allow_all_users = False,
	additional_data = {
			"printer@odata_bind" : "https://graph.microsoft.com/v1.0/print/printers/{printerId}",
	}
)

result = await graph_client.print.shares.by_printer_share_id('printerShare-id').patch(request_body)


```