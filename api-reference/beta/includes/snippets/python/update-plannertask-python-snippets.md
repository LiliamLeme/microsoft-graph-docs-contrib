---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = PlannerTask(
	assignments = PlannerAssignments(
		additional_data = {
				"fbab97d0-4932-4511-b675-204639209557" : {
						"@odata_type" : "#microsoft.graph.plannerAssignment",
						"order_hint" : "N9917 U2883!",
				},
		}
	),
	applied_categories = PlannerAppliedCategories(
		additional_data = {
				"category3" : True,
				"category4" : False,
		}
	),
	recurrence = PlannerTaskRecurrence(
		schedule = PlannerRecurrenceSchedule(
			pattern = RecurrencePattern(
				type = RecurrencePatternType.Daily,
				interval = 3,
			),
			pattern_start_date_time = "2022-02-22T02:10:33Z",
		),
	),
)

request_configuration = PlannerTaskItemRequestBuilder.PlannerTaskItemRequestBuilderPatchRequestConfiguration()
request_configuration.headers.add("Prefer", "return=representation")
request_configuration.headers.add("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")


result = await graph_client.planner.tasks.by_planner_task_id('plannerTask-id').patch(request_body, request_configuration = request_configuration)


```