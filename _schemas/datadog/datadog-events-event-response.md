---
description: Response wrapper for a single event
layout: schema
name: EventResponse
properties_list:
- description: ''
  name: data
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-events-event-response-schema.json
slug: datadog-events-event-response
source_filename: datadog-events-event-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-event-response-schema.json\",\n  \"title\": \"EventResponse\",\n  \"description\": \"Response wrapper for a single event\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"$ref\": \"#/components/schemas/Event\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-event-response-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: EventResponse
---
