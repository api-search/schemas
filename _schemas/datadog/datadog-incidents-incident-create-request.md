---
description: Request body for creating a new incident
layout: schema
name: IncidentCreateRequest
properties_list:
- description: The incident creation data
  name: data
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-incidents-incident-create-request-schema.json
slug: datadog-incidents-incident-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-create-request-schema.json\",\n  \"title\": \"IncidentCreateRequest\",\n  \"description\": \"Request body for creating a new incident\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"The incident creation data\",\n      \"required\": [\n        \"type\",\n        \"attributes\"\n      ],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The resource type identifier for incidents\",\n          \"enum\": [\n            \"incidents\"\n          ]\n        },\n        \"attributes\": {\n          \"$ref\": \"#/components/schemas/IncidentCreateAttributes\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-create-request-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: IncidentCreateRequest
---
