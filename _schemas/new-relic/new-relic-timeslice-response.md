---
description: ''
layout: schema
name: TimesliceResponse
properties_list:
- description: ''
  name: from
  type: string
- description: ''
  name: to
  type: string
- description: ''
  name: values
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-timeslice-response-schema.json
slug: new-relic-timeslice-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"from\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T14:30:00Z\"\n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T14:30:00Z\"\n    },\n    \"values\": {\n      \"type\": \"object\",\n      \"example\": {},\n      \"properties\": {}\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TimesliceResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-timeslice-response-schema.json
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
title: TimesliceResponse
---
