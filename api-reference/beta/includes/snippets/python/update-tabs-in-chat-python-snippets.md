---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = TeamsTab(
	display_name = "My Contoso Tab - updated again",
)

result = await graph_client.chats.by_chat_id('chat-id').tabs.by_teams_tab_id('teamsTab-id').patch(request_body)


```