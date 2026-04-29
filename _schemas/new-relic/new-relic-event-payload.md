---
description: Schema for custom event data payloads submitted to the New Relic Event API. Represents an array of custom event objects, each with a required eventType and any number of user-defined attribute key-value pairs. Events are stored in NRDB and queryable via NRQL.
layout: schema
name: New Relic Event API Payload
properties_list: []
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-event-payload-schema.json
slug: new-relic-event-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.newrelic.com/schemas/telemetry/event-payload.json\",\n  \"title\": \"New Relic Event API Payload\",\n  \"description\": \"Schema for custom event data payloads submitted to the New Relic Event API. Represents an array of custom event objects, each with a required eventType and any number of user-defined attribute key-value pairs. Events are stored in NRDB and queryable via NRQL.\",\n  \"type\": \"array\",\n  \"maxItems\": 2000,\n  \"items\": {\n    \"$ref\": \"#/$defs/CustomEvent\"\n  },\n  \"$defs\": {\n    \"CustomEvent\": {\n      \"type\": \"object\",\n      \"description\": \"A single custom event. Must include eventType. All other keys are user-defined attributes stored as event fields in NRDB.\",\n      \"required\": [\"eventType\"],\n      \"properties\": {\n        \"eventType\": {\n          \"type\": \"string\",\n          \"description\": \"The event type name used as\
  \ the NRDB table. Must match [a-zA-Z0-9:_ ]+ and not exceed 255 characters. Cannot start with nr. (reserved).\",\n          \"maxLength\": 255,\n          \"pattern\": \"^[a-zA-Z0-9:_ ]+$\"\n        },\n        \"timestamp\": {\n          \"type\": \"integer\",\n          \"description\": \"Unix epoch timestamp in seconds when the event occurred. If omitted, the ingestion time is used. Cannot be more than 48 hours in the past or 24 hours in the future.\",\n          \"examples\": [1645564509]\n        }\n      },\n      \"additionalProperties\": {\n        \"description\": \"User-defined event attribute. Keys must not start with nr. (reserved). String values are limited to 4096 characters.\",\n        \"oneOf\": [\n          {\n            \"type\": \"string\",\n            \"maxLength\": 4096\n          },\n          {\n            \"type\": \"number\"\n          },\n          {\n            \"type\": \"boolean\"\n          }\n        ]\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-event-payload-schema.json
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
title: New Relic Event API Payload
---
