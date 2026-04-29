---
description: ''
layout: schema
name: PolicyChannelsResponseType
properties_list:
- description: ''
  name: channel_ids
  type: array
- description: ''
  name: id
  type: integer
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-policy-channels-response-type-schema.json
slug: new-relic-policy-channels-response-type
source_filename: new-relic-policy-channels-response-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"channel_ids\": {\n      \"type\": \"array\",\n      \"example\": [\n        100\n      ],\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PolicyChannelsResponseType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-policy-channels-response-type-schema.json
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
title: PolicyChannelsResponseType
---
