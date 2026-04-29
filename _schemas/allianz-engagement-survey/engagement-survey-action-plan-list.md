---
description: List of action plans for a survey
layout: schema
name: ActionPlanList
properties_list:
- description: Total number of action plans
  name: total
  type: integer
- description: List of action plan records
  name: items
  type: array
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
schema_file: json-schema/engagement-survey-action-plan-list-schema.json
slug: engagement-survey-action-plan-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-action-plan-list-schema.json\",\n  \"title\": \"ActionPlanList\",\n  \"description\": \"List of action plans for a survey\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of action plans\",\n      \"example\": 12\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"List of action plan records\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ActionPlan\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-action-plan-list-schema.json
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
title: ActionPlanList
---
