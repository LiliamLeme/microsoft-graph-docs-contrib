---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = PinnedChatMessageInfo(
	additional_data = {
			"message@odata_bind" : "https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1616964509832",
	}
)

result = await graph_client.chats.by_chat_id('chat-id').pinned_messages.post(request_body)


```