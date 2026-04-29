---
description: A single event from the Datadog Events Explorer
layout: schema
name: Event
properties_list:
- description: The unique string identifier of the event
  name: id
  type: string
- description: The resource type identifier (always 'event')
  name: type
  type: string
- description: ''
  name: attributes
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-events-event-schema.json
slug: datadog-events-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-event-schema.json\",\n  \"title\": \"Event\",\n  \"description\": \"A single event from the Datadog Events Explorer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique string identifier of the event\",\n      \"example\": \"abc-123-def\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type identifier (always 'event')\",\n      \"example\": \"metric alert\"\n    },\n    \"attributes\": {\n      \"$ref\": \"#/components/schemas/EventAttributes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-event-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: Event
---
