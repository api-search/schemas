---
description: Request body for updating an existing incident team
layout: schema
name: IncidentTeamUpdateRequest
properties_list:
- description: The incident team update data
  name: data
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-incidents-incident-team-update-request-schema.json
slug: datadog-incidents-incident-team-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-team-update-request-schema.json\",\n  \"title\": \"IncidentTeamUpdateRequest\",\n  \"description\": \"Request body for updating an existing incident team\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"The incident team update data\",\n      \"required\": [\n        \"type\",\n        \"id\",\n        \"attributes\"\n      ],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The resource type identifier for incident teams\",\n          \"enum\": [\n            \"teams\"\n          ]\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique ID of the incident team to update\"\n        },\n        \"attributes\"\
  : {\n          \"type\": \"object\",\n          \"description\": \"The updated incident team attributes\",\n          \"required\": [\n            \"name\"\n          ],\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"The updated name for the incident team\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-team-update-request-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: IncidentTeamUpdateRequest
---
