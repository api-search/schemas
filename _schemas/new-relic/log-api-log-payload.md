---
description: Array of log data batch objects
layout: schema
name: LogPayload
properties_list: []
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/log-api-log-payload-schema.json
slug: log-api-log-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/log-api-log-payload-schema.json\",\n  \"title\": \"LogPayload\",\n  \"description\": \"Array of log data batch objects\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/LogDataObject\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/log-api-log-payload-schema.json
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
title: LogPayload
---
