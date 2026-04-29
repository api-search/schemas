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
schema_file: json-schema/new-relic-event-custom-event-schema.json
slug: new-relic-event-custom-event
source_filename: new-relic-event-custom-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A custom event to record. Must include eventType. All other attributes are user-defined key-value pairs. Attribute names must not start with nr. (reserved). Values can be strings, numbers, or booleans.\",\n  \"properties\": {\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of event. Used as the NRDB event table name. Must match the pattern [a-zA-Z0-9:_ ]+, max 255 characters.\",\n      \"example\": \"standard\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix epoch timestamp in seconds. If omitted, the current time is used. Cannot be more than 48 hours in the past or 24 hours in the future.\",\n      \"example\": 1718153645993\n    }\n  },\n  \"required\": [\n    \"eventType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CustomEvent\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-event-custom-event-schema.json
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
