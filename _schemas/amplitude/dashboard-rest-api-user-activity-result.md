---
description: UserActivityResult schema from Amplitude Dashboard REST API
layout: schema
name: UserActivityResult
properties_list:
- description: User metadata including user_id and Amplitude ID.
  name: userData
  type: object
- description: Array of recent events for the user.
  name: events
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/dashboard-rest-api-user-activity-result-schema.json
slug: dashboard-rest-api-user-activity-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dashboard-rest-api-user-activity-result-schema.json\",\n  \"title\": \"UserActivityResult\",\n  \"description\": \"UserActivityResult schema from Amplitude Dashboard REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userData\": {\n      \"type\": \"object\",\n      \"description\": \"User metadata including user_id and Amplitude ID.\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"Array of recent events for the user.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"additionalProperties\": true\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dashboard-rest-api-user-activity-result-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: UserActivityResult
---
