---
description: Response wrapper for a single incident
layout: schema
name: IncidentResponse
properties_list:
- description: ''
  name: data
  type: object
- description: Related resources included in the response based on the include query parameter
  name: included
  type: array
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-incidents-incident-response-schema.json
slug: datadog-incidents-incident-response
source_filename: datadog-incidents-incident-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-response-schema.json\",\n  \"title\": \"IncidentResponse\",\n  \"description\": \"Response wrapper for a single incident\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"$ref\": \"#/components/schemas/Incident\"\n    },\n    \"included\": {\n      \"type\": \"array\",\n      \"description\": \"Related resources included in the response based on the include query parameter\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-response-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: IncidentResponse
---
