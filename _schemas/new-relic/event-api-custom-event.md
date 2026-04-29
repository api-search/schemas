---
description: A custom event to record. Must include eventType. All other attributes are user-defined key-value pairs. Attribute names must not start with nr. (reserved). Values can be strings, numbers, or booleans.
layout: schema
name: CustomEvent
properties_list:
- description: The type of event. Used as the NRDB event table name. Must match the pattern [a-zA-Z0-9:_ ]+, max 255 characters.
  name: eventType
  type: string
- description: Unix epoch timestamp in seconds. If omitted, the current time is used. Cannot be more than 48 hours in the past or 24 hours in the future.
  name: timestamp
  type: integer
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/event-api-custom-event-schema.json
slug: event-api-custom-event
source_filename: event-api-custom-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/event-api-custom-event-schema.json\",\n  \"title\": \"CustomEvent\",\n  \"description\": \"A custom event to record. Must include eventType. All other attributes are user-defined key-value pairs. Attribute names must not start with nr. (reserved). Values can be strings, numbers, or booleans.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of event. Used as the NRDB event table name. Must match the pattern [a-zA-Z0-9:_ ]+, max 255 characters.\",\n      \"maxLength\": 255,\n      \"example\": \"standard\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix epoch timestamp in seconds. If omitted, the current time is used. Cannot be more than 48 hours in the past or 24 hours in the future.\"\
  ,\n      \"example\": 1718153645993\n    }\n  },\n  \"required\": [\n    \"eventType\"\n  ],\n  \"additionalProperties\": {\n    \"description\": \"Additional user-defined event attributes\",\n    \"oneOf\": [\n      {\n        \"type\": \"string\",\n        \"maxLength\": 4096\n      },\n      {\n        \"type\": \"number\"\n      },\n      {\n        \"type\": \"boolean\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/event-api-custom-event-schema.json
tags:
- Analysis
- Analytics
- APM
- DevOps
- Infrastructure
- Monitoring
- Observability
- Performance
- Platform
title: CustomEvent
---
