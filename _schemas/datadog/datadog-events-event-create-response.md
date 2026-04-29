---
description: Response indicating an event was accepted for processing
layout: schema
name: EventCreateResponse
properties_list:
- description: The status of the event creation request
  name: status
  type: string
- description: The unique numeric identifier assigned to the created event
  name: event_id
  type: integer
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-events-event-create-response-schema.json
slug: datadog-events-event-create-response
source_filename: datadog-events-event-create-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-event-create-response-schema.json\",\n  \"title\": \"EventCreateResponse\",\n  \"description\": \"Response indicating an event was accepted for processing\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the event creation request\",\n      \"enum\": [\n        \"ok\"\n      ],\n      \"example\": \"ok\"\n    },\n    \"event_id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The unique numeric identifier assigned to the created event\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-event-create-response-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: EventCreateResponse
---
