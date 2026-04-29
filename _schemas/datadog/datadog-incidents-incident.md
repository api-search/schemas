---
description: A Datadog incident record representing an outage or service disruption
layout: schema
name: Incident
properties_list:
- description: The unique string identifier of the incident
  name: id
  type: string
- description: The resource type identifier (always 'incidents')
  name: type
  type: string
- description: ''
  name: attributes
  type: object
- description: Relationships to associated resources such as commander, teams, and services
  name: relationships
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-incidents-incident-schema.json
slug: datadog-incidents-incident
source_filename: datadog-incidents-incident-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-schema.json\",\n  \"title\": \"Incident\",\n  \"description\": \"A Datadog incident record representing an outage or service disruption\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique string identifier of the incident\",\n      \"example\": \"abc-123-def\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type identifier (always 'incidents')\",\n      \"example\": \"metric alert\"\n    },\n    \"attributes\": {\n      \"$ref\": \"#/components/schemas/IncidentAttributes\"\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"description\": \"Relationships to associated resources such as commander, teams, and services\",\n      \"properties\": {\n\
  \        \"commander\": {\n          \"type\": \"object\",\n          \"description\": \"The incident commander responsible for coordinating the response\",\n          \"properties\": {\n            \"data\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"id\": {\n                  \"type\": \"string\",\n                  \"description\": \"The unique ID of the commander user\"\n                },\n                \"type\": {\n                  \"type\": \"string\",\n                  \"description\": \"The resource type (users)\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: Incident
---
