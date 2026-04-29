---
description: An array of custom event objects to ingest
layout: schema
name: EventPayload
properties_list: []
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-event-event-payload-schema.json
slug: new-relic-event-event-payload
source_json: "{\n  \"type\": \"array\",\n  \"description\": \"An array of custom event objects to ingest\",\n  \"items\": {\n    \"type\": \"object\",\n    \"description\": \"A custom event to record. Must include eventType. All other attributes are user-defined key-value pairs. Attribute names must not start with nr. (reserved). Values can be strings, numbers, or booleans.\",\n    \"properties\": {\n      \"eventType\": {\n        \"type\": \"string\",\n        \"description\": \"The type of event. Used as the NRDB event table name. Must match the pattern [a-zA-Z0-9:_ ]+, max 255 characters.\",\n        \"example\": \"standard\"\n      },\n      \"timestamp\": {\n        \"type\": \"integer\",\n        \"description\": \"Unix epoch timestamp in seconds. If omitted, the current time is used. Cannot be more than 48 hours in the past or 24 hours in the future.\",\n        \"example\": 1718153645993\n      }\n    },\n    \"required\": [\n      \"eventType\"\n    ]\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"EventPayload\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-event-event-payload-schema.json
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
title: EventPayload
---
