---
description: A correlated incident from multiple alerts.
layout: schema
name: Incident
properties_list:
- description: Incident ID.
  name: id
  type: string
- description: Incident status.
  name: status
  type: string
- description: Incident severity level.
  name: severity
  type: string
- description: Incident description.
  name: description
  type: string
- description: Number of correlated alerts.
  name: alerts_count
  type: integer
- description: Unix timestamp when incident started.
  name: started_at
  type: integer
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-incident-schema.json
slug: bigpanda-incident
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Incident\",\n  \"type\": \"object\",\n  \"description\": \"A correlated incident from multiple alerts.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Incident ID.\",\n      \"example\": \"inc-abc123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Incident status.\",\n      \"enum\": [\n        \"active\",\n        \"resolved\",\n        \"acknowledged\"\n      ],\n      \"example\": \"active\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Incident severity level.\",\n      \"enum\": [\n        \"critical\",\n        \"warning\",\n        \"unknown\"\n      ],\n      \"example\": \"critical\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Incident description.\",\n      \"example\": \"CPU overload on production-database-1\"\n    },\n    \"\
  alerts_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of correlated alerts.\",\n      \"example\": 3\n    },\n    \"started_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when incident started.\",\n      \"example\": 1713000000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/json-schema/bigpanda-incident-schema.json
tags:
- Incidents
- Monitoring
- Platform
title: Incident
---
