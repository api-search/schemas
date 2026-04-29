---
description: PolicyChannelsResponseType schema
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
schema_file: json-schema/openapi-policy-channels-response-type-schema.json
slug: openapi-policy-channels-response-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-policy-channels-response-type-schema.json\",\n  \"title\": \"PolicyChannelsResponseType\",\n  \"description\": \"PolicyChannelsResponseType schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channel_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"example\": [\n        100\n      ]\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-policy-channels-response-type-schema.json
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
