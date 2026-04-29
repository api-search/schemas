---
description: EventListResult schema from Amplitude Dashboard REST API
layout: schema
name: EventListResult
properties_list:
- description: Array of event type objects with names and volumes.
  name: data
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/dashboard-rest-api-event-list-result-schema.json
slug: dashboard-rest-api-event-list-result
source_filename: dashboard-rest-api-event-list-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dashboard-rest-api-event-list-result-schema.json\",\n  \"title\": \"EventListResult\",\n  \"description\": \"EventListResult schema from Amplitude Dashboard REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of event type objects with names and volumes.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the event type.\"\n          },\n          \"totals\": {\n            \"type\": \"integer\",\n            \"description\": \"The total number of times this event was fired in the last 30 days.\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dashboard-rest-api-event-list-result-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: EventListResult
---
