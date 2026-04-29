---
description: ''
layout: schema
name: PolicyChannelsResponse
properties_list:
- description: ''
  name: policy
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-policy-channels-response-schema.json
slug: new-relic-policy-channels-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"channel_ids\": {\n          \"type\": \"array\",\n          \"example\": [\n            100\n          ],\n          \"items\": {\n            \"type\": \"integer\"\n          }\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PolicyChannelsResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-policy-channels-response-schema.json
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
title: PolicyChannelsResponse
---
