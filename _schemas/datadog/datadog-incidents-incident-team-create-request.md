---
description: Request body for creating a new incident team
layout: schema
name: IncidentTeamCreateRequest
properties_list:
- description: The incident team creation data
  name: data
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-incidents-incident-team-create-request-schema.json
slug: datadog-incidents-incident-team-create-request
source_filename: datadog-incidents-incident-team-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-team-create-request-schema.json\",\n  \"title\": \"IncidentTeamCreateRequest\",\n  \"description\": \"Request body for creating a new incident team\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"The incident team creation data\",\n      \"required\": [\n        \"type\",\n        \"attributes\"\n      ],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The resource type identifier for incident teams\",\n          \"enum\": [\n            \"teams\"\n          ]\n        },\n        \"attributes\": {\n          \"type\": \"object\",\n          \"description\": \"The incident team attributes\",\n          \"required\": [\n            \"name\"\n          ],\n\
  \          \"properties\": {\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"The name of the incident team for display and identification\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-team-create-request-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: IncidentTeamCreateRequest
---
