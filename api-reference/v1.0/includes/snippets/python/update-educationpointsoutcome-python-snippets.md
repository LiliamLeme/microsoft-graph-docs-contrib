---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = EducationPointsOutcome(
	odata_type = "#microsoft.graph.educationPointsOutcome",
	points = EducationAssignmentPointsGrade(
		odata_type = "#microsoft.graph.educationAssignmentPointsGrade",
		points = 85.0,
	),
)

result = await graph_client.education.classes.by_education_class_id('educationClass-id').assignments.by_education_assignment_id('educationAssignment-id').submissions.by_education_submission_id('educationSubmission-id').outcomes.by_education_outcome_id('educationOutcome-id').patch(request_body)


```