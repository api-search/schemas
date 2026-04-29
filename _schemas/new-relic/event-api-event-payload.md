---
description: An array of custom event objects to ingest
layout: schema
name: EventPayload
properties_list: []
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/event-api-event-payload-schema.json
slug: event-api-event-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/event-api-event-payload-schema.json\",\n  \"title\": \"EventPayload\",\n  \"description\": \"An array of custom event objects to ingest\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/CustomEvent\"\n  },\n  \"maxItems\": 2000\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/event-api-event-payload-schema.json
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
