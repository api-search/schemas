---
description: Request body for creating a new event in the Datadog Events Explorer
layout: schema
name: EventCreateRequest
properties_list:
- description: The event data object
  name: data
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-events-event-create-request-schema.json
slug: datadog-events-event-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-event-create-request-schema.json\",\n  \"title\": \"EventCreateRequest\",\n  \"description\": \"Request body for creating a new event in the Datadog Events Explorer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"The event data object\",\n      \"required\": [\n        \"type\",\n        \"attributes\"\n      ],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The resource type identifier for event creation\",\n          \"enum\": [\n            \"event\"\n          ]\n        },\n        \"attributes\": {\n          \"$ref\": \"#/components/schemas/EventCreateAttributes\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-event-create-request-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: EventCreateRequest
---
