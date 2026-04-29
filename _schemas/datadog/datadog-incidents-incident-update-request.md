---
description: Request body for updating an existing incident
layout: schema
name: IncidentUpdateRequest
properties_list:
- description: The incident update data
  name: data
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-incidents-incident-update-request-schema.json
slug: datadog-incidents-incident-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-update-request-schema.json\",\n  \"title\": \"IncidentUpdateRequest\",\n  \"description\": \"Request body for updating an existing incident\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"The incident update data\",\n      \"required\": [\n        \"type\",\n        \"id\",\n        \"attributes\"\n      ],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The resource type identifier\",\n          \"enum\": [\n            \"incidents\"\n          ]\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique ID of the incident to update\"\n        },\n        \"attributes\": {\n          \"$ref\": \"#/components/schemas/IncidentUpdateAttributes\"\
  \n        }\n      }\n    }\n  },\n  \"required\": [\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-update-request-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: IncidentUpdateRequest
---
