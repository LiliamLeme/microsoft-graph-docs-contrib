---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = Bookmark(
	description = "Book a fancy vacation in Tuscany or browse museums in Florence.",
)

result = await graph_client.search.bookmarks.by_bookmark_id('bookmark-id').patch(request_body)


```